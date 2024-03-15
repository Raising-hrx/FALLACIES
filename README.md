# FALLACIES

This is the data for [A Closer Look at the Self-Verification Abilities of Large Language Models in Logical Reasoning](https://arxiv.org/abs/2311.07954)



- ```step_fallacy.test.jsonl```: The FALLACIES Dataset.
Each row is a sample containing the reasoning step ("step"), the label ("label", 0 for correct step and 1 for fallcious step), the corresponding fallacy type ("fallacy"), and the corresponding topic ("entity").

    {
        "step": "Since [I am wearing a necklace made of hemalyke] and [I either wear jewelry made of gold or hemalyke], therefore, [I do not wear jewelry made of gold].", 
        "entity": "hemalyke", 
        "fallacy": "Affirming a Disjunct", 
        "label": 1
    }

- ```fallacies.json```: The names of 232 fallacies as well as their definitions.

- ```fallacy_taxonomy.json```: The hierarchical taxonomy of fallacies.

- ```license.txt```: CC BY-NC-SA 4.0.
