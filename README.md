# KEF LSX EasyEffects Presets by KEF_LSX

Premium-quality EasyEffects presets specifically tuned for **KEF LSX** wireless speakers, optimized for desktop/near-field listening environments.

## 🎵 Presets Overview

### **KEF_LSX.json** - Daily Driver Excellence
Perfect for all-day listening with balanced, natural sound:
- ✅ Controlled sub-bass extension (28Hz +8.5dB)
- ✅ Punchy but clean bass (64Hz +9dB, 125Hz +6dB)
- ✅ Clear midrange separation (-3/-2dB at 500/1000Hz)
- ✅ Crystal-clear highs (3.5-14kHz optimized)
- ✅ Natural stereo imaging (+15% stereo base)

### **KEF_LSX_Cinema.json** - IMAX Experience
Calibrated for movies and cinematic content:
- 🎬 Deep sub-bass impact (25Hz +3dB, 50Hz +3.5dB)
- 🎬 Cinema V-curve with enhanced dynamics
- 🎬 Dialogue clarity (3.2kHz +6dB)
- 🎬 Explosive highs (6.4kHz +8dB)
- 🎬 Advanced limiting for distortion-free peaks
- 🎬 Wider soundstage (+25% stereo base)

## 🎯 Hardware Compatibility

**Primary Target:** KEF LSX (Original & LSX II)
- Optimized for desktop placement
- Corrects inherent LSX frequency response issues
- Compensates for near-field listening position

**May also benefit:**
- KEF LS50 Wireless
- Other small bookshelf speakers with similar characteristics
- Coaxial driver designs

## 📍 Optimal Setup

**Positioning:**
- Desktop placement at ear level
- Behind/between computer monitors
- 0.5-1.5m listening distance
- Speakers on isolation pads/books

**Room Treatment:**
- Hard surfaces (desk, wall reflections) accounted for
- No additional room correction required

## 🔧 Technical Details

### KEF_LSX (Balanced)
```
Sub-Bass (28Hz): +8.5dB, Q=0.9
Bass (64Hz): +9.0dB, Q=1.1
Mid-Bass (125Hz): +6.0dB, Q=1.0
Lower-Mid (500Hz): -3.0dB, Q=0.6
Upper-Mid (1kHz): -2.0dB, Q=0.8
Presence (3.5kHz): +8.0dB, Q=0.8
Brilliance (7kHz): +9.0dB, Q=0.9
Air (14kHz): +7.5dB, Q=1.0

Effects Chain:
EQ → Bass Enhancer (+6.5dB) → Exciter (+7dB) → Stereo Tools
```

### KEF_LSX_Cinema (Cinematic)
```
Sub-Bass (25Hz): +3.0dB, Q=1.2
Bass (50Hz): +3.5dB, Q=1.2
Impact (100Hz): +2.5dB, Q=1.2
Warmth (200Hz): +3.0dB, Q=0.9
Mid-Cut (400Hz): -4.0dB, Q=0.5
Clarity Cut (800Hz): -3.5dB, Q=0.6
Dialogue (3.2kHz): +6.0dB, Q=0.6
Presence (6.4kHz): +8.0dB, Q=0.7
Air (12.8kHz): +6.0dB, Q=0.8

Effects Chain:
EQ → Bass Enhancer (+3dB) → Exciter (+9dB) → Stereo Tools → Limiter
```

## 📥 Installation

### Method 1: Manual Installation
1. Download the preset files
2. Copy to your EasyEffects output presets folder:
   ```bash
   # For system installation:
   ~/.config/easyeffects/output/
   
   # For Flatpak installation:
   ~/.var/app/com.github.wwmm.easyeffects/config/easyeffects/output/
   ```
3. Restart EasyEffects
4. Select preset from the dropdown menu

### Method 2: Command Line Installation
```bash
# For Flatpak users (most common):
cd ~/.var/app/com.github.wwmm.easyeffects/config/easyeffects/output/
wget https://raw.githubusercontent.com/[YOUR-REPO]/KEF-LSX-Presets/main/KEF_LSX.json
wget https://raw.githubusercontent.com/[YOUR-REPO]/KEF-LSX-Presets/main/KEF_LSX_Cinema.json

# For system installation:
cd ~/.config/easyeffects/output/
wget https://raw.githubusercontent.com/[YOUR-REPO]/KEF-LSX-Presets/main/KEF_LSX.json
wget https://raw.githubusercontent.com/[YOUR-REPO]/KEF-LSX-Presets/main/KEF_LSX_Cinema.json
```

## 🎛️ Usage Recommendations

### **KEF_LSX (Daily)**
Perfect for:
- Music listening (all genres)
- Video calls/meetings
- General computer use
- Podcast/audiobook listening
- Gaming

### **KEF_LSX_Cinema**
Ideal for:
- Movies and TV shows
- Gaming with cinematic audio
- YouTube/streaming content
- Music with dynamic range (orchestral, film scores)
- Testing speaker capabilities

## ⚙️ Customization Tips

### Fine-tuning for your room:
- **Too much bass?** Reduce gains at 28Hz/64Hz by 1-2dB
- **Harsh highs?** Slightly reduce 7kHz/14kHz by 0.5-1dB
- **Not enough presence?** Increase 3.5kHz by 0.5-1dB
- **Too wide stereo?** Reduce stereo-base to 0.1 (KEF_LSX) or 0.2 (Cinema)

### Volume considerations:
- Both presets include input gain reduction for headroom
- If too quiet: Increase system volume rather than preset output-gain
- If distortion occurs: Reduce input material volume first

## 🔬 Development Process

These presets were developed through:
1. **Frequency Response Analysis** - Based on Stereophile KEF LSX measurements
2. **Room Acoustic Compensation** - Desktop placement considerations
3. **Iterative Testing** - Extensive listening tests across content types
4. **Precision Tuning** - Q-values and gains optimized for clarity
5. **Overload Protection** - Limiting and gain staging for clean dynamics

## 📊 Frequency Response Targets

**KEF LSX Known Issues Addressed:**
- Weak sub-bass below 50Hz → Enhanced with controlled boost
- Mid-range boxiness around 500-1000Hz → Precisely notched
- Treble rolloff above 10kHz → Extended with careful enhancement
- Near-field reflections → Compensated with EQ adjustments

## 🎤 Feedback & Support

**Tested Environment:**
- openSUSE Tumbleweed Linux
- EasyEffects (Flatpak version)
- KEF LSX original
- Desktop setup behind dual monitors
- Various music genres and movie content

**Community:**
- Share your experience in GitHub Issues
- Suggest improvements or variations
- Report compatibility with other speakers

## 📜 License

These presets are released under **Creative Commons CC0** - Public Domain.
Use, modify, and share freely. Attribution appreciated but not required.

## 🙏 Credits

**Created by:** KEF_LSX  
**Developed with:** Claude Code AI Assistant  
**Based on:** KEF LSX frequency response measurements from Stereophile  
**Inspired by:** Cinema audio engineering principles and audiophile listening standards

---

### 💡 Pro Tip
Start with **KEF_LSX** for daily use, switch to **KEF_LSX_Cinema** for movies. Both presets are designed to be used at your normal listening volume - no need to adjust gain settings unless you have specific room acoustic issues.

**Enjoy your transformed KEF LSX experience!** 🎵✨