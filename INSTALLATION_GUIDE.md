# Installation Guide - KEF LSX EasyEffects Presets

## 🔍 Quick Start

### 1. Determine Your EasyEffects Installation Type

**Check if you have Flatpak version:**
```bash
flatpak list | grep easyeffects
```

**Check if you have system version:**
```bash
which easyeffects
```

### 2. Find Your Preset Directory

**For Flatpak (most common):**
```bash
~/.var/app/com.github.wwmm.easyeffects/config/easyeffects/output/
```

**For System Installation:**
```bash
~/.config/easyeffects/output/
```

**For Package Manager Installation:**
```bash
~/.config/easyeffects/output/
```

## 📥 Installation Methods

### Method A: Direct Download (Recommended)

1. **Create preset directory if it doesn't exist:**
```bash
# For Flatpak:
mkdir -p ~/.var/app/com.github.wwmm.easyeffects/config/easyeffects/output/

# For System:
mkdir -p ~/.config/easyeffects/output/
```

2. **Download presets:**
```bash
# Navigate to your preset directory first, then:
wget https://raw.githubusercontent.com/[YOUR-USERNAME]/KEF-LSX-EasyEffects-Presets/main/Runlvl.json
wget https://raw.githubusercontent.com/[YOUR-USERNAME]/KEF-LSX-EasyEffects-Presets/main/Runlvl_Cinema.json
```

### Method B: Git Clone

1. **Clone the repository:**
```bash
git clone https://github.com/[YOUR-USERNAME]/KEF-LSX-EasyEffects-Presets.git
cd KEF-LSX-EasyEffects-Presets
```

2. **Copy presets to EasyEffects:**
```bash
# For Flatpak:
cp *.json ~/.var/app/com.github.wwmm.easyeffects/config/easyeffects/output/

# For System:
cp *.json ~/.config/easyeffects/output/
```

### Method C: Manual Copy

1. Download the JSON files from the repository
2. Copy them to your EasyEffects output presets folder
3. Restart EasyEffects

## 🔧 Post-Installation Setup

### 1. Restart EasyEffects
```bash
# For Flatpak:
flatpak kill com.github.wwmm.easyeffects
flatpak run com.github.wwmm.easyeffects

# For System:
pkill easyeffects
easyeffects
```

### 2. Load the Preset
1. Open EasyEffects
2. Go to the "Output" tab
3. Click the preset dropdown menu
4. Select either "Runlvl" or "Runlvl_Cinema"

### 3. Verify Installation
- You should see both presets in the dropdown
- Audio should sound immediately different (more bass, clearer highs)
- No error messages should appear

## 🎯 Optimization for Your Setup

### Initial Settings Recommendations

**For Desktop Setup:**
- Use "Runlvl" preset as default
- Switch to "Runlvl_Cinema" for movies
- Keep EasyEffects running in background

**Volume Levels:**
- Set system volume to comfortable level first
- Don't increase preset output gains unless necessary
- Use hardware volume controls on KEF LSX when possible

### Common Adjustments

**If bass is too strong:**
```
Reduce 28Hz and 64Hz gains by 1-2dB in the EQ
```

**If highs are too bright:**
```
Reduce 7kHz and 14kHz gains by 0.5-1dB
```

**If vocals are unclear:**
```
Increase 3.5kHz gain by 0.5-1dB
```

## 🐛 Troubleshooting

### Presets Don't Appear
1. **Check file location:**
   ```bash
   ls ~/.var/app/com.github.wwmm.easyeffects/config/easyeffects/output/
   ```

2. **Verify JSON syntax:**
   ```bash
   python3 -m json.tool Runlvl.json
   ```

3. **Check file permissions:**
   ```bash
   chmod 644 *.json
   ```

### Audio Distortion
1. **Lower system volume first**
2. **Check for multiple audio effects running**
3. **Verify KEF LSX volume settings**
4. **Use "Runlvl" instead of "Runlvl_Cinema" for less aggressive processing**

### No Audio Output
1. **Verify EasyEffects is set as audio device**
2. **Check PulseAudio/PipeWire compatibility**
3. **Restart audio service:**
   ```bash
   systemctl --user restart pipewire
   # or
   pulseaudio -k && pulseaudio --start
   ```

### Preset Loads But No Effect
1. **Check that EasyEffects is enabled (toggle on/off)**
2. **Verify output device is correct**
3. **Check if bypass is enabled**

## 🔄 Updating Presets

### Manual Update
1. **Download new versions**
2. **Replace existing files**
3. **Restart EasyEffects**

### Git Update
```bash
cd KEF-LSX-EasyEffects-Presets
git pull origin main
cp *.json ~/.var/app/com.github.wwmm.easyeffects/config/easyeffects/output/
```

## 🗑️ Uninstallation

To remove the presets:
```bash
# Navigate to your preset directory
rm Runlvl.json Runlvl_Cinema.json
```

## 📋 System Requirements

- **EasyEffects:** Version 6.0 or newer
- **Audio System:** PulseAudio or PipeWire
- **Linux Distribution:** Any modern distribution
- **Speakers:** KEF LSX (optimal), or similar bookshelf speakers

## 🆘 Getting Help

**Before asking for help, please provide:**
1. Your Linux distribution and version
2. EasyEffects installation method (Flatpak/system/package manager)
3. EasyEffects version (`easyeffects --version`)
4. Audio system (PulseAudio/PipeWire)
5. Error messages or symptoms

**Where to get help:**
- GitHub Issues in this repository
- EasyEffects official GitHub discussions
- Linux audio forums and communities

---

**Happy listening!** 🎵