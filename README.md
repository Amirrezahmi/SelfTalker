<h1 align="center" style="color: red;">${\color{red}\text{Self Talker AI}}$</h1>

## ${\color{cyan}\text{Project Overview}}$

Imagine being able to converse with a version of yourself that can provide answers to any question you may have. This project aimed to achieve just that!

You can now engage in a conversation with yourself and seek answers to questions that may have previously eluded you.

Using cutting-edge machine learning techniques such as NLP, voice cloning, computer vision, etc., we have created a virtual version of you that can seamlessy communicate with you. This AI-powered version of yourself is capable of understanding the nuances of human language and can provide insightful and accurate responses to your queries.

Upon receiving the input prompt, the program initiates the answer generation process. Subsequently, it proceeds to extract relevant keywords and phrases from the generated response. Also the program summarize the generated answer to improve the quality of the final text. After obtaining the final answer, the Styleformer feature is applied, allowing you to switch between formal and casual styles seamlessly.

To enhance the understanding of the content, the program creates two images: the first image is generated using the extracted keywords, while the second image utilizes the extracted phrases from the generated text. Additionally, leveraging the aforementioned keywords and phrases, the program generates two videos. Next, employing voice cloning techniques and utilizing a dataset of your recorded voice in `.wav` format, the program synthesizes the text into speech, employing your unique vocal characteristics. Furthermore, by utilizing your $256 \times 256$ input image in `.jpg` format, the program automatically generates a talking-head video, employing your input image as a base, and synchronized with the cloned voice.

<div align="center">
  <img src="https://github.com/Amirrezahmi/SelfTalker/assets/89692207/282e2d9c-de0f-44eb-bb7f-326489d77a8b" width="700" />
</div>




So, whether you're seeking advice on a personal matter, looking for guidance in your career, or simply curious about the world around you, this AI-powered version of yourself is always at your disposal.

With this project, the possibilities are endless. Your AI-powered virtual self is ready for conversation at any time.


# ${\color{cyan}\text{Features}}$
Welcome to the Features section!

We've numbered the features below to highlight their specific order and importance. This helps you understand the logical progression of our product's capabilities, making it easier to grasp the underlying flow and prioritize accordingly. Enjoy exploring the exciting features we have in store for you!
   1. Text generation powered by fine-tuned GPT-2
   2. Keyword Extraction with KeyBERT
   3. Text summarization
   4. Styleformer Integration: Seamless Style Switching in Conversations
   5. AI Text-to-Image with minimal DALL-E Mini
   6. Text-to-video with Diffusers
   7. Voice Cloning
   8. MakeItTalk: Speaker-Aware Talking-Head Animation

# ${\color{cyan}\text{Prerequisites}}$


   - Python 3.x
   - Google Colab or Jupyter
   - As this is a Jupyter Notebook file, It's not OS-specific and can be run on any operating system that supports Python, including Windows, macOS, and Linux.
   - If you want to convert the Jupyter notebook (`.ipynb`) into a standalone web application with a user interface (UI), you can use `Anvil`.

# ${\color{cyan}\text{Getting Started}}$

## ${\color{pink}\text{Clone the repository}}$


  1. Clone the repository:

```bash
git clone https://github.com/Amirrezahmi/SelfTalker.git
```

## ${\color{pink}\text{Usage}}$
  2. However I've told everything in `Self_Talker.ipynb`, but let me summarize it here one more time! First of all download my fine-tuned GPT-2 model from <a href="https://drive.google.com/drive/folders/11W-KNm_lFtqAu0Kw7ANw-PcefkpD0aCP"> here</a> or if you have your own dataset and you want to fine-tune your own GPT-2 model, I've provided my both jupyter notebok and dataset in `fine-tune GPT2` directory. This folder contains my code which used to fine-tune GPT-2 on my own dataset.
  3. The sixth step of `Self_Talker.ipynb` is related to voice cloning, so a dataset of your voice is required. Please note that the files should be formated in `.wav`. Ten files of 10-15 seconds are enough for your dataset.
  4. The last step of `Self_Talker.ipynb` asks you for a $256 \times 256$ picture of yourself which is formated in `.jpg` file.
  5. After going through the previous steps, it's time to run cell's from the `Self_Talker.ipynb` jupyter note book. All you need to run this project is a colab        or jupyter account. By running "requirements" section from this notebook, you will simply install all requirements. Please note that you should change your run time type to GPU and import the fine-tuned GPT-2 model or even the voice dataset of yours if you're using google colab.

# ${\color{cyan}\text{Example}}$

Here's a sample example:

${\color{red}\text{Prompt:}}$

${\color{orange}\text{\quad \quad \quad How to become a rich guy?}}$

${\color{red}\text{Generated Response:}}$

If you want to be rich, you need to have a lot of money. If you don't have enough money, it will be difficult for you to achieve your goals, because you will not be able to buy the things that you really want. The only way to make money is by investing. Investing in stocks, bonds, real estate, and other assets is one of the best ways to get rich. There are many methods of investing, but the most important is to invest your money in the stock market. For example, if you invest \$ 10,000 in a mutual fund, the fund will give you a return of 10% per year for the next 10 years. This is called a compound annual growth rate (CAGR). The more money you put into a fund the greater the return.

${\color{red}\text{The top 3 keywords:}}$


${\color{orange}\text{\quad \quad \quad 'rich', 'investing' and 'invest'}}$

${\color{red}\text{The top 3 phrases:}}$

${\color{orange}\text{\quad \quad \quad 'want rich', 'ways rich' and 'invest money'}}$

${\color{red}\text{Text summarization:}}$

If you want to be rich, you need to have a lot of money. The only way to make money is by investing. Investing in stocks, bonds, real estate, and other assets is one of the best ways to get rich. For example, if you invest $10,000 in a mutual fund, the fund will give you a return of 10% per year for the next 10 years.

> **_NOTE:_** The final text comprises the generated response combined with our summarized text.

${\color{red}\text{Switching between formal and casual language styles:}}$

> **_NOTE:_** Using Styleformer we convert our generated response and summarized text from formal to casual language style. Please note that the genereated text from our fine-tuned GPT-2 model is primarily formal in nature. Visit `Self_Talker.ipynb` for more details.

  - **_Changing generated response language style to casual:_**

if you want to be rich, you have to have money. You will have a hard time achieving your goals if you're not rich enough to buy what you really want. Investing is the only way to make money. investing in stocks, bonds, real estate and other assets is one of the best ways to get rich. there are many ways to invest, but the most important is to invest your money in the stock market. like if you invest $ 10,000 in a mutual fund, that mutual will return you 10% each year for the next 10 years. it's called a compound annual growth rate. the more money you put into a fund the better the return.

- **_Changing summarized text language style to casual:_**

if you want to be rich, you have to have money. You can only make money by investing. Investing stocks, bonds, real estate is one of the best ways to get rich. like if you invest $10,000 in a mutual fund, the fund will give you a return of 10% per year for the next 10 years.

> **_NOTE:_** In this example, I continued with the formal text but in your case it's all up to you.

${\color{red}\text{Generating our first Text-to-Image. The prompt is our keywords variable:}}$

<div align="center">
  <img src="https://github.com/Amirrezahmi/SelfTalker/assets/89692207/39e0594a-2338-4e33-ad68-e09df7ee2e21" alt="20230617_123525_0000" width="300" />
</div>



${\color{red}\text{Generating our second Text-to-Image. The prompt is our phrases variable:}}$

<div align="center">
  <img src="https://github.com/Amirrezahmi/SelfTalker/assets/89692207/d7e202ca-7be0-42cb-9b0d-64f0986f4758" alt="20230617_123525_0000" width="300" />
</div>


${\color{red}\text{Generating our first video. The prompt is our keywords variable:}}$

https://github.com/Amirrezahmi/SelfTalker/assets/89692207/f2e3e59f-9dd3-4bf9-815a-801b9a89f1c4



${\color{red}\text{Generating our second video. The prompt is our phrases variable:}}$



https://github.com/Amirrezahmi/SelfTalker/assets/89692207/7b76ce01-531b-4db8-bdf2-11ec1fe47ca2


${\color{red}\text{Voice Cloning:}}$

In this remarkable process, we have successfully cloned Elon Musk's voice using a dataset of his own recordings. The result of our text-to-speech synthesis can be found in the following `.mov` file:



https://github.com/Amirrezahmi/SelfTalker/assets/89692207/ddb84548-5014-428e-b8f8-b46375bac940


Our text here is the abridged text of the generated response.

${\color{red}256 \times 256}$ ${\color{red} \text{ Input Image:}}$

<div align="center">
  <img src="https://github.com/Amirrezahmi/SelfTalker/assets/89692207/51224db3-4aa6-458b-8644-aeb978d6b719" alt="20230617_123525_0000" width="200" />
</div>

${\color{red} \text{Speaker-Aware Talking-Head Animation:}}$




https://github.com/Amirrezahmi/SelfTalker/assets/89692207/3a076a6d-6fe4-4e30-b9b1-f2cb9a9d11f7





${\color{red} \text{Final video:}}$



https://github.com/Amirrezahmi/SelfTalker/assets/89692207/7506c5ca-f3d4-4c0a-a31d-73b0dad0a3e6



# ${\color{cyan}\text{Contributing}}$ 

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1.  Fork the repository.
2. Create a new branch: git checkout -b my-new-branch.
3. Make your changes and commit them: git commit -m 'Add some feature'.
4. Push to the branch: git push origin my-new-branch.
5. Submit a pull request.
    
# ${\color{cyan}\text{License}}$

This project is licensed under the [MIT License](https://opensource.org/license/mit/).


# ${\color{cyan}\text{Credits}}$

  - [GPT-2](https://github.com/openai/gpt-2)- For Text generation step.
  - [KeyBERT](https://github.com/MaartenGr/KeyBERT)- For Keyword Extraction step.
  - [Styleformer](https://github.com/PrithivirajDamodaran/Styleformer)- For Style Switching in Conversations.
  - [DALL·E Mini](https://github.com/borisdayma/dalle-mini)- For AI Text-to-Image step.
  - [Diffusers](https://huggingface.co/damo-vilab/text-to-video-ms-1.7b)- For Text-to-Video step
  - [TorToiSe](https://github.com/jnordberg/tortoise-tts)- For voice cloning step.
  - [MakeItTalk](https://github.com/yzhou359/MakeItTalk)- For Speaker-Aware Talking-Head Animation step.

# ${\color{cyan}\text{Contact}}$

For any questions or inquiries, please contact amirrezahmi2002@gmail.com




