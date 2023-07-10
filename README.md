# A Systematic Study and Comprehensive Evaluation of ChatGPT on Benchmark Datasets

This is the repository of Our ACL'23 findings paper, [A Systematic Study and Comprehensive Evaluation of ChatGPT on Benchmark Datasets](https://arxiv.org/pdf/2305.18486.pdf).

![eval_benchmarks](https://github.com/ntunlp/ChatGPT_Eval/blob/main/eval.jpg)

All the data can be downloaded from [here](https://drive.google.com/drive/folders/1eC2zEpq_7zxG4l3BSdt8THzzIu_mGnBa?usp=sharing).


Yet another ChatGPT evaluation !!!! What's new ? This time not automatic, human in a loop. 
Our ACL'23 paper covers FULL eval on benchmarks that actually MATTERS !!!

We cover the largest ChatGPT evaluation so far (255K responses) on 140 tasks.

![datasets](https://github.com/ntunlp/ChatGPT_Eval/blob/main/figures/17.PNG)


Please consider citing if you use the data or results from this paper.

```
@misc{laskar2023systematic,
      title={A Systematic Study and Comprehensive Evaluation of ChatGPT on Benchmark Datasets}, 
      author={Md Tahmid Rahman Laskar and M Saiful Bari and Mizanur Rahman and Md Amran Hossen Bhuiyan and Shafiq Joty and Jimmy Xiangji Huang},
      year={2023},
      eprint={2305.18486},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```


Here is a short summary of the findings from the paper, 

- As a general purpose instruction following multitask model, ChatGPT performs worse than the SOTA single task fine-tuned models. For targeted tasks, the fine-tuned model may still be preferable.

![super_glue](https://github.com/ntunlp/ChatGPT_Eval/blob/main/figures/1.PNG)

- The evaluation of ChatGPT-like LLMs should include human intervention instead of fully automatic evaluation.

![human_in_a_loop](https://github.com/ntunlp/ChatGPT_Eval/blob/main/figures/16.PNG)

- ChatGPT can often perform on par with an average human in *Algorithmic Tasks*.

![bigbench](https://github.com/ntunlp/ChatGPT_Eval/blob/main/figures/3.PNG)

- For the same input prompt, different versions of ChatGPT may yield significantly different results.

- Though the basic reasoning capability of ChatGPT is exceptional with *Chain-of-thought* (CoT) prompting, ChatGPT *sometimes* faces severe catastrophic forgetting in newly defined reasoning tasks when *CoT* prompting is not used..

![inverse](https://github.com/ntunlp/ChatGPT_Eval/blob/main/figures/2.PNG)

- We also identify an interesting capability. There is a SHARP trend of this features at different scale !!!! ChatGPT can attend to multiple questions in a query and respond accordingly. However, adding many questions may reduce the model's performance. We name if as **PolyQuery Synthesis**.

![polyquery](https://github.com/ntunlp/ChatGPT_Eval/blob/main/figures/4.PNG)
![polyquery_res](https://github.com/ntunlp/ChatGPT_Eval/blob/main/figures/5.PNG)

- Though ChatGPT has multilingual capability, its performance in underrepresented languages is very low.

![polyquery_res](https://github.com/ntunlp/ChatGPT_Eval/blob/main/figures/6.PNG)

- Though ChatGPT's open-domain knowledge capability is extremely high, it often suffers in several Commonsense Reasoning tasks (e.g., PIQA, SIQA, HellaSwag, WinoGrande) compared to the competing models, such as, PaLM 540B and LLaMA 65B .

![polyquery_res](https://github.com/ntunlp/ChatGPT_Eval/blob/main/figures/7.PNG)
![polyquery_res](https://github.com/ntunlp/ChatGPT_Eval/blob/main/figures/8.PNG)

- For text summarization, the ChatGPT cannot outperform the current SOTA models based on the ROGUE metric. However, our annotators prefer ChatGPT's generated summaries over the SOTA models. This suggests that we may need a new summarization metric to evaluate ChatGPT like instruction-tuned LLMs.

![summarization](https://github.com/ntunlp/ChatGPT_Eval/blob/main/figures/9.PNG)

- ChatGPT has a very strong Zero-shot mathematical and coding capability in comparison to other LLMs.

![math](https://github.com/ntunlp/ChatGPT_Eval/blob/main/figures/12.PNG)

- ChatGPT is found to be more ethical  than prior SOTA models, while being less biased and more truthful.

![truthfulqa](https://github.com/ntunlp/ChatGPT_Eval/blob/main/figures/11.PNG)
![ethics](https://github.com/ntunlp/ChatGPT_Eval/blob/main/figures/13.PNG)

- ChatGPT sometimes considers *utilitarian morality* and can respond to ethical dilemma-related queries (Section \ref{par:ethical_dilemma}).

![utilitarian](https://github.com/ntunlp/ChatGPT_Eval/blob/main/figures/15.PNG)





