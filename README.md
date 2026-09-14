# FRAME Pre-Beta Build 02

AI-assisted photography decision engine for photographers.

Based on the locked FRAME v1.18 UX baseline.

## What is real

- iPhone camera preview and image capture
- AI-powered scene understanding
- Structured AI scene analysis
- Profile selection
- Profile-aware recommendation engine
- Deterministic camera-setting decisions
- Verified camera and lens selection
- Gear compatibility validation
- Persistent settings and profiles
- Light / Dark / Automatic appearance
- Haptic feedback layer
- PWA shell
- Developer feedback system
- Engine Test Lab

## How FRAME works

FRAME separates scene understanding from camera-setting decisions.

1. **IMAGE**
   The photographer captures the scene.

2. **AI SCENE UNDERSTANDING**
   AI analyzes the image and identifies relevant scene characteristics such as movement, light level, depth, environment and color temperature.

3. **STRUCTURED SCENE DATA**
   The AI returns structured scene information.

4. **FRAME ENGINE**
   The deterministic engine combines the scene data with the selected profile.

5. **GEAR VALIDATION**
   The recommendation is checked against the selected camera and lens.

6. **RECOMMENDATION**
   FRAME presents a photography-plausible starting point.

**FRAME recommends. The photographer decides.**

## AI architecture

AI is used for scene understanding only.

AI does **not** directly choose the final camera settings.

This separation allows FRAME to evolve its scene-understanding capabilities independently from the deterministic decision engine.

If AI analysis is unavailable, FRAME can fall back to the local engine recommendation.

## Profiles

Current profiles:

- Portrait
- Street
- Wildlife
- Landscape

Each profile influences how FRAME prioritizes the scene when producing its recommendation.

## Gear

FRAME supports a growing catalog of verified cameras and lenses.

The selected gear is used to validate whether a recommendation is physically compatible with the photographer's equipment.

Current development gear includes:

- Canon EOS R5
- Canon RF 50mm F1.2 L USM
- Fujifilm X-T30 II
- Fujinon XF18-55mmF2.8-4 R LM OIS
- Viltrox AF 56mm F1.7 Air

The gear catalog is expandable and is not limited to the developer's own equipment.

## Engine Test Lab

The built-in Engine Test Lab is used to evaluate how FRAME responds to different combinations of:

- Scene
- Profile
- Gear

The current test environment contains:

- 10 demo scenes
- 4 profiles
- 40 scene/profile combinations

The test lab is a development and validation tool and does not replace physical camera testing.

## Developer feedback

Pre-beta testers can send feedback directly from FRAME.

Feedback includes relevant app context such as:

- Build version
- Screen
- Test scene
- Profile
- Camera
- Lens
- Timestamp

Captured images are not included in developer feedback.

## Privacy

The FRAME backend uses the OpenAI Responses API with `store: false`.

Captured image data is not written to FRAME application logs.

The developer feedback system does not send captured images.

## Pre-beta status

This build is intended for controlled beta testing.

The primary goals are to validate:

- AI scene understanding
- Recommendation quality
- Profile behaviour
- Gear compatibility
- User experience
- Engine decisions under real-world conditions

Feedback from testing will be used to refine FRAME before moving toward a production engine.

---

**FRAME recommends.  
The photographer decides.**
