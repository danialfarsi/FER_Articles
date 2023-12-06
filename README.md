# Emotion Detection Type

## Emotion Detection Type

| Detection Type                    | Objective                                               | Methods                                              | Challenges                                           |
|------------------------------------|---------------------------------------------------------|------------------------------------------------------|------------------------------------------------------|
| Discrete Emotion Detection         | Classifies emotions into categories                     | Machine learning on various modalities               | Requires labeled training data                        |
| Categorical Emotion Recognition    | Classifies emotions into categories                     | Machine learning on various modalities               | Requires labeled training data                        |
| Facial Expression Analysis         | Analyzes facial expressions for emotions                | Computer vision and deep learning                   | Limited to observable facial expressions             |
| Speech Emotion Recognition          | Identifies emotions in spoken language                   | Analyzes acoustic features using ML or DL models     | Variability in speech patterns, need for datasets     |
| Continuous Emotion Detection        |                                                       |                                                      |                                                      |
| Dimensional Affect Detection      | Captures emotions on continuous scales                   | Regression models, e.g., LSTM-RNN, CCRF             | Requires continuous annotations, complex models      |
| Multimodal Emotion Recognition      | Integrates information from multiple sources            | Fusion of features from different modalities        | Requires synchronization of data from sources         |
| Implicit Tagging                    | Identifies emotional metadata from spontaneous reactions| Analyzes physiological signals, facial expressions   | Inferring emotions indirectly from user reactions    |

## Model Concepts

| Model | Main Concept | Example Emotions |
|-------|--------------|------------------|
| Discrete Model | Distinct, separate emotions | Joy, Sadness, Anger, Fear, Disgust |
| Dimensional Model | Valence (positive/negative) and Arousal (intensity) dimensions | Valence: Pleasant to Unpleasant Arousal: Low to High |


# Emotion Dataset

## Database Comparison

| Database | Participants | Individual vs. Group | Purpose | Modalities | Annotations | Weaknesses | Suitable for Discrete Model | Suitable for Dimensional Model |
|----------|--------------|-----------------------|---------|------------|-------------|------------|-----------------------------|--------------------------------|
| SEMAINE | 150 | Individual | Emotion recognition based on facial expressions | Audio and Visual | Valence, arousal, and FACS | Limited sample size, may not generalize well to diverse populations. | ✔️ | ✔️ |
| AM-FED | 242 | Individual | Spontaneous facial expression recognition "In-the-Wild" | Visual | 14 AUs, 2 head movements, smile, expressiveness, and 22 landmark points. Self-assessment of familiarity, liking, and desire to watch again. | Limited diversity in facial expressions captured in the wild. | ✔️ | ❌ |
| DISFA | 27 | Individual | Spontaneous facial action recognition | Visual | 12 AUs | Small dataset size may limit the model's generalizability. | ✔️ | ❌ |
| MAHNOB-HCI | 27 | Individual | Emotion recognition and implicit tagging | Visual, Audio, Eye Gaze, ECG, GSR, Respiration Amplitude, Skin temperature, EEG | Self-assessment of valence, dominance, predictability, and emotional keywords. Agreement/disagreement with tags. | Multiple modalities may introduce complexity and potential noise in annotations. | ❌ | ✔️ |
| DEAP | 32 | Individual | Implicit affective tagging from EEG and peripheral physiological signals | EEG, GSR, Respiration Amplitude, Skin Temperature, Blood Volume, Electromyogram, and Electrooculogram | Visual for 22 participants. Self-assessment of arousal, valence, liking, dominance, and familiarity. | Limited number of participants may not represent a wide range of population responses. | ❌ | ✔️ |
| DECAF | 30 | Individual | Affect recognition | MEG, Near-infra-red facial video, horizontal Electrooculogram, ECG, and trapezius-Electromyogram | Self-assessment of valence, arousal, and dominance. Continuous annotation of valence and arousal of the stimuli. | Complexity of modalities may require advanced processing and may be resource-intensive. | ❌ | ✔️ |
| Zhang et al corpus | 140 | Individual | Emotional behavior research | 3D dynamic imaging, Visual, Thermal sensing, EDA, Respiration, Blood Pressure, and Hearth Rate | Occurrence and intensity of AUs. Features from 3D, 2D, and Infra-red sensors. | The use of various sensors may result in challenges in data synchronization and integration. | ❌ | ❌ |
| Mission Survival II | 16 | 4 people group | Personality states research | Audio and Visual | Personality states by the Ten Item Personality Inventory. | Limited group size may not capture the dynamics of larger social interactions. | ❌ | ❌ |
| ASCERTAIN | 58 | Individual | Personality and Affect | EEG, ECG, GSR, and Visual | Big-Five personality traits, self-assessment of valence and arousal. | Limited modalities may not capture the full spectrum of affective states. | ❌ | ✔️ |
| AMIGOS | 40 Individual & 4 people group | Affect, personality, mood, and social context recognition | Audio, Visual, Depth, EEG, GSR, and ECG | Big-Five personality traits and PANAS. Self-assessment of valence, arousal, dominance, liking, familiarity, and basic emotions. | Combining individual and group data may introduce complexities in modeling and interpretation. | ❌ | ✔️ |
