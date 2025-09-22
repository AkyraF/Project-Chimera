# Project Chimera

**Project Chimera** is a custom fork/extension of OpenUtau focused on bridging traditional UTAU rendering with modern AI-based voice conversion (RVC).  
The goal is to create a hybrid environment where UTAU’s sequencing power can be combined with RVC’s flexibility, without requiring external pipelines or manual conversions.

---

## ✨ Core Features (Planned)

- **Dual Render Mode**  
  In addition to UTAU’s existing rendering, a new “RVC Mode” will be available.  
  - User selects RVC as the render option.  
  - UTAU handles pitch, timing, and note sequencing.  
  - RVC processes the audio into the target voice.  

- **Track-Specific RVC Settings**  
  Each track can store its own RVC model, feature index, and settings, including:  
  - Index ratio slider  
  - Protect voiceless consonants slider  
  - Median filtering slider  
  - Algorithm tick boxes (PM, Harvest, Crepe, RMVPE)  

- **Non-Blocking Rendering ("Baking")**  
  Rendering is handled track-by-track.  
  - UTAU renders → passes audio to RVC → waits for output.  
  - Playback is only possible after baking completes.  
  - The UI stays responsive (user can still edit notes while baking runs).  

- **Flexible Piano Roll Layout**  
  Two UI modes will be available:  
  - **OpenUtau Style** (floating piano roll window)  
  - **Chimera Style** (integrated piano roll below track list, like Vocaloid/SynthV)  

---

## 🚀 Philosophy

Chimera follows the principle:  
**“First make it exist. Figure out how to make it better later.”**  
The project focuses on building a working foundation before optimizing or polishing.

---

## 🔧 Roadmap

1. Add preferences option to connect to an RVC backend.  
2. Implement RVC render mode.  
3. Add per-track RVC settings UI.  
4. Attach baking + progress bar system.  
5. Add Chimera-style piano roll integration toggle.  
6. Future iterations: performance tweaks, caching, advanced controls.

---

## 📜 License

This project inherits its license from [OpenUtau](https://github.com/stakira/OpenUtau).

---

## 🤝 Contributing

Contributions, feature requests, and testing feedback are welcome!  
