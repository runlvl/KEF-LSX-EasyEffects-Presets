# Project Context & Development History

## 📋 Complete Project State Documentation

### 🎯 Project Overview
**Repository:** https://github.com/runlvl/KEF-LSX-EasyEffects-Presets
**Purpose:** Professional EasyEffects presets for KEF LSX speakers and AirPods Pro 2
**Developer:** Runlvl (GitHub user)
**AI Assistant:** Claude Code

### 📁 Current File Structure
```
/home/runlvl/easyeffects_presets/
├── KEF_LSX.json                    # Balanced KEF LSX preset
├── KEF_LSX_Cinema.json             # Cinematic KEF LSX preset
├── AirPods_Pro_2.json              # Conservative AirPods preset
├── AirPods_Pro_2_Ultimate.json     # Maximum AirPods preset
├── README.md                       # Main documentation
├── INSTALLATION_GUIDE.md           # Setup instructions
├── TECHNICAL_DETAILS.md            # Engineering specs
└── PROJECT_CONTEXT.md              # This file

Local EasyEffects presets:
/home/runlvl/.var/app/com.github.wwmm.easyeffects/config/easyeffects/output/
├── KEF_LSX.json
├── KEF_LSX_Cinema.json
├── AirPods_Pro_2.json
└── AirPods_Pro_2_Ultimate.json
```

### 🏷️ GitHub Releases
- **v1.0.0** - Initial release with all presets
- **v1.0.1** - Critical bass oversteering fix for AirPods Ultimate
- **v1.1.0** - Renamed Runlvl presets to KEF_LSX for clarity
- **v1.2.0** - Added comprehensive AirPods documentation

### 🎵 Preset Details & User Feedback

#### KEF LSX Speakers
**KEF_LSX.json (formerly Runlvl.json):**
- Purpose: Balanced daily driver for desktop setup
- Target: KEF LSX speakers behind monitors at ear level
- Status: ✅ User approved ("So ist es akzeptabel")
- Key features: 28Hz +8.5dB, 64Hz +9dB, 7kHz +9dB
- Plugin chain: EQ → Bass Enhancer → Exciter → Stereo Tools

**KEF_LSX_Cinema.json (formerly Runlvl_Cinema.json):**
- Purpose: Cinematic V-curve for movies
- Status: ✅ User approved after multiple bass oversteering fixes
- Key features: 25Hz +3dB, aggressive limiting, wide stereo base
- Plugin chain: EQ → Bass Enhancer → Exciter → Stereo Tools → Limiter

#### AirPods Pro 2
**AirPods_Pro_2.json:**
- Purpose: Conservative enhancement for daily use
- Status: ✅ Working well
- Key features: Gentle corrections, 4-plugin chain
- Plugin chain: EQ → Bass Enhancer → Exciter → Stereo Tools

**AirPods_Pro_2_Ultimate.json:**
- Purpose: Maximum performance for audiophiles
- Status: ✅ Fixed bass oversteering in v1.0.1 ("Das ist viel besser")
- Original issue: "die Bässe übersteuern massiv"
- Fix applied: Reduced bass gains, increased headroom, adjusted limiting
- Plugin chain: EQ → Compressor → Bass Enhancer → Exciter → Stereo Tools → Limiter

### 🔧 Technical Implementation Details

#### Key Corrections Made During Development:
1. **Bass Oversteering Fix (AirPods Ultimate):**
   - EQ input gain: -4dB → -6dB
   - Bass frequencies: 20Hz (3.0→1.5dB), 40Hz (2.5→1.0dB), 80Hz (1.0→0.5dB)
   - Bass enhancer: amount 4.5→2.0, harmonics 7.0→4.0
   - EQ output gain: +2dB→0dB
   - Limiter threshold: -2dB→-3dB

2. **Naming Convention Change:**
   - Runlvl.json → KEF_LSX.json
   - Runlvl_Cinema.json → KEF_LSX_Cinema.json
   - Reason: "deutlich wird das diese für diese Lautsprecher gedacht sind"

#### User Setup Context:
- **Hardware:** KEF LSX speakers on desktop behind monitors
- **OS:** openSUSE Tumbleweed
- **EasyEffects:** Flatpak version
- **Use case:** Desktop near-field listening, occasional cinema

### 🗣️ User Feedback History (German)
Key user quotes that shaped development:
- "Ist immer noch sehr seicht und flach" → Led to more aggressive EQ
- "wieder etwas bass-lastiger und dumpfer" → Simplified plugin chains
- "Die Bässe übersteuern heftig" → Cinema preset bass fixes
- "So ist es akzeptabel" → Final KEF LSX approval
- "die Bässe übersteuern massiv" → AirPods Ultimate bass fix
- "Das ist viel besser" → AirPods fix confirmation

### 🛠️ Development Environment
- **Working Directory:** /home/runlvl/easyeffects_presets
- **Git Status:** Clean, all commits pushed
- **Authentication:** GitHub CLI configured with classic token
- **Platform:** Linux (openSUSE Tumbleweed)

### 📊 Current GitHub State
- **Repository:** Public, fully documented
- **Stars:** Not tracked yet
- **Topics:** audio, easyeffects, kef, lsx, equalizer, presets, linux, opensuse, audiophile, desktop-audio
- **License:** CC0 Public Domain
- **Documentation:** Complete for both device types

### 🎯 Known Working Configurations
1. **KEF LSX Desktop Setup:**
   - Speakers: Behind monitors, ear level, on isolation
   - Distance: 0.5-1.5m
   - Preset: KEF_LSX.json for daily, KEF_LSX_Cinema.json for movies
   - Status: User approved, no oversteering

2. **AirPods Pro 2 Setup:**
   - Connection: Bluetooth or wired via Linux
   - iOS Settings: EQ off, Adaptive EQ off, Transparency mode
   - Preset: AirPods_Pro_2.json for daily, Ultimate for critical listening
   - Status: Bass oversteering fixed, working well

### 🔮 Future Considerations
- Community sharing strategy documented but not yet executed
- Potential expansion to other KEF models
- Measurement-based preset development
- Additional device support

### 🤖 AI Assistant Context
- **Assistant:** Claude Code (Anthropic)
- **Session:** Extensive audio engineering conversation
- **Capabilities Used:** File editing, git management, GitHub CLI, technical analysis
- **Approach:** Scientific, measurement-based, user feedback driven
- **Result:** Professional-grade audio presets with comprehensive documentation

---

**This document serves as complete project context for future AI assistants or developers.**