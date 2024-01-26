AI notes
========

## 25-Jan

After a basic implementation of AI using DICY2 to output rearranged segments of the source text ("[À ma mère](../Working_files/à_ma_mère.txt)"), I've pondered how to leverage AI to do something more interesting than essentially function as a random generator. 

So, let's go with the low-hanging fruit and see what ChatGPT can give us? 

> **ChatGPT**: Here are some creative suggestions on how to use AI to generate sequencing for dance based on a poem:
> 
> 1. Semantic Analysis for Movement Dynamics:
>    - Use Natural Language Processing (NLP) techniques to perform semantic analysis on the poem. Identify key emotions, themes, and concepts expressed in the text.
>    - Translate these identified elements into corresponding movement dynamics for the dancers. For example, intense emotions might translate into fast and dynamic movements, while more serene parts of the poem could be interpreted as slower and graceful motions.
> 2. Rhythmic Pattern Extraction:
>    - Analyze the rhythm and cadence of the poem to generate a rhythmic pattern. This could involve identifying stressed and unstressed syllables, sentence structures, or overall pacing.
>    - Translate the rhythmic pattern into a musical score for the musicians. Experiment with different time signatures, tempos, and instruments to reflect the nuances of the poem.
> 3. Melodic Generation from Text Sentiments:
>    - Use sentiment analysis to determine the emotional tone of different sections of the poem.
>    - Assign musical motifs and melodies to specific sentiments. Positive sentiments might be expressed through uplifting and major-key melodies, while darker emotions could be represented by dissonant or minor-key compositions.
> 4. Interactive AI Collaboration:
>    - Develop an interactive system where the dancers' movements influence the music and vice versa. Utilize motion sensors to capture the dancers' gestures and use this data to dynamically alter the musical composition in real-time.
>    - Allow for improvisation by the performers, with the AI system adapting and responding to their movements and expressions.
> 5. Generative Visuals based on Poetic Imagery:
>    - Extract vivid imagery and descriptive elements from the poem.
>    - Use this textual information to generate visual elements, perhaps through generative art techniques. Project these visuals in real-time during the performance to enhance the overall experience.
> 6. Collaborative AI Composition:
>    - Employ a collaborative AI system that involves both musicians and dancers in the creative process. The AI can suggest musical and dance elements, and the human performers can provide feedback, creating a dynamic back-and-forth collaboration.
> 7. Narrative Structure Mapping:
>    - Analyze the narrative structure of the poem (if applicable) and use it as a basis for structuring the performance. Design different sections or acts, each corresponding to a specific part of the narrative.

So, I had ChatGPT do a semantic analysis of the poem, which are on Sheet 3 of the [spreadsheet](../Working_files/A%20ma%20mère%20-%20labeling.ods). The analysis identified 9 themes:

1. Nostalgia
2. Childhood and personal growth
3. Love and devotion
4. Connection
5. Ambiguity and divinity
6. Sacrifice
7. Dependence
8. Yearning for innocence
9. Journey and homecoming

So compositionally this could demarcate 9 modules for the piece. 

This can be used as a labeling schema for lines of the poem and fed to the textual example of Dicy2. But it seems like this is not really effective for Dicy2, which really needs several layers of magnitude more data to really do something interesting (read, audio rate streaming data or similar...). So that is what I am currently working on. 


