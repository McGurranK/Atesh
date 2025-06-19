# Atesh (or Ate, or Atesh)

_A chaotic, unstable, and corrupted distortion plugin._

Atesh is a reimagining of my very first (and very broken) distortion plugin—something I originally made while tinkering with circuit-bent pedals for birthday presents. This project leans hard into ideas of instability, unpredictability, and noise, turning a flawed concept into a tool I genuinely enjoy using.

---

## 🎛️ What is Atesh?

Atesh is a plugin designed to behave in strange and unpredictable ways. Its key tenets are:

- **Unstable**
- **Volatile**
- **Corrupted**

This isn't meant to be clean or precise—it's meant to be wild.

---

## 🧠 Background

My creative roots are in improvisation, rock, and noise. For a time, mixer feedback was my favorite "instrument"—used on drum machines, in solo setups, or as part of chaotic live ensembles. I love the feeling of wrestling with something unstable, and that ethos is deeply baked into Atesh.

I also wanted to bring in ideas from my interest in accessibility. The interface is intentionally curated to support keyboard navigation, and while I’m not visually impaired myself, I’d love to hear feedback from anyone who is.

---

## ♿ Accessibility

Some accessibility features are inherited from JUCE (like keyboard focus and navigation), and while there’s no direct value input yet, keyboard users might find it surprisingly usable. I’m open to all feedback on how to improve the interface further.

---

## 🎨 UI Design (Why so ugly?)

I'll be honest: UI design isn’t my strength. The visuals are deliberately simple and raw—partly due to time constraints, partly due to the theme. It’s functional, but far from polished. That said, the interface is meant to reflect the chaos behind the sound.

---

## 🛠️ Setup & Building Atesh

Atesh can be built using either **CMake** (recommended) or **Projucer**. JUCE is included as a submodule.

### ✅ Recommended: Building with CMake

CMake provides a modern, IDE-agnostic build system.

#### Prerequisites

- CMake (3.15+)
- A C++17-compatible compiler
- JUCE (included via submodule)

#### Steps

1. Clone the repository with submodules:  
   `git clone --recurse-submodules https://github.com/yourname/atesh.git`  
   `cd atesh`

   If you forgot `--recurse-submodules`:  
   `git submodule update --init --recursive`

2. Create a build directory:  
   `mkdir build && cd build`

3. Generate the project:  
   `cmake ..`

   You can specify options like:  
   `-DCMAKE_BUILD_TYPE=Release`  
   or a generator:  
   `-G "Visual Studio 17 2022"`

4. Build the plugin:  
   `cmake --build .`

5. Locate the output plugin file in `build/Debug/` or `build/Release/`.

---

### 🧪 Alternative: Building with Projucer

1. Clone the repository with submodules:  
   `git clone --recurse-submodules https://github.com/yourname/atesh.git`  
   `cd atesh`

2. Build the Projucer:  
   Navigate to `JUCE/extras/Projucer/Builds/` and build the appropriate version for your platform.

3. Open `Atesh.jucer` with Projucer.

4. Configure plugin formats and settings as needed.

5. Export to your IDE (Xcode, Visual Studio, etc.) and build the project.

---

### 🔍 Troubleshooting

- **JUCE not found?**  
  Run:  
  `git submodule update --init --recursive`

- **Plugin doesn't appear in your DAW?**  
  Make sure you’re building the correct format (e.g. VST3, AU) and copying it to your system’s plugin folder.

- **On Windows?**  
  Use a CMake generator like:  
  `cmake -G "Visual Studio 17 2022" ..`

---

## ⚠️ Notes & Disclaimers

- Currently tested **only on macOS**
- No automated testing (or manual QA!) yet
- This is still a work in progress
- Use at your own risk and feel free to open issues if you break it—or it breaks you

---

## 📬 Feedback

If you’re using a screen reader or encounter UX challenges, I’m especially keen to hear from you. I want this to be fun, weird, and *usable*.

---

## 🚧 Future Plans

- Better UI design (maybe)
- MIDI control mapping
- Full cross-platform testing
- Preset saving/loading
- More chaos knobs


