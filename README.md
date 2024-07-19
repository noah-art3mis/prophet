# Prophet

## TODO

-   we might need very long sentences because most of it is nonsense
    -   'It was in this connection that I constructed the images of the technique of the upholsterer, of the buttoning point, since it is necessary that some point of the fabric of one should attach itself to the fabric of the other.'
    -   'If the signs are valid for all, in principle this should give us a society which functions in a perfectly ideal fashion.'
    -   'It is not a question of course of a real space, but it is a question of something in which homologues can be delineated.'
    -   'This ceremony consisted in doing what was necessary, they probably knew it, to get the gods of the others on their side.'

## Tech

1. manual cleanup with pypdf loader
1. hires unstructured serverless api ($1 per 100 pages)
1. unstructured for MTG? epubloader

https://unstructured.io/blog/chunking-for-rag-best-practices
https://unstructured.io/blog/unstructured-s-preprocessing-pipelines-enable-enhanced-rag-performance
https://unstructured.io/blog/understanding-what-matters-for-llm-ingestion-and-preprocessing
https://unstructured.io/blog/building-reliable-genai-applications-with-unstructured-and-vectara
https://unstructured.io/blog/how-to-process-pdf-in-python
https://unstructured.io/blog/fine-tuning-gpt-3-5
https://unstructured.io/blog/how-to-build-an-end-to-end-rag-pipeline-with-unstructured-s-api
https://unstructured.io/blog/effortless-document-extraction-a-guide-to-using-unstructured-api-and-data-connectors

### pdf

-   [langchain pdf loaders](https://python.langchain.com/v0.1/docs/modules/data_connection/document_loaders/pdf)
    -   [unstructured api](https://docs.unstructured.io/api-reference/api-services/overview)
        -   [UnstructuredAPIFileLoader](https://api.python.langchain.com/en/latest/document_loaders/langchain_community.document_loaders.unstructured.UnstructuredAPIFileLoader.html)
        -   https://docs.unstructured.io/api-reference/api-services/sdk
    -   [unstructured open source](https://docs.unstructured.io/open-source/introduction/quick-start)
        -   [UnstructuredFileLoader](https://api.python.langchain.com/en/latest/document_loaders/langchain_community.document_loaders.unstructured.UnstructuredFileLoader.html)
        -   ~~[UnstructuredPDFLoader](https://api.python.langchain.com/en/latest/document_loaders/langchain_community.document_loaders.pdf.UnstructuredPDFLoader.html)~~
    -   tesseract
    -   pdf2text
    -   pypdfium2
-   https://github.com/VikParuchuri/surya
-   https://github.com/VikParuchuri/marker

### models

-   https://llm.extractum.io/model/TheBloke%2FWizard-Vicuna-13B-Uncensored-GGUF,1k3iyhbgYQh8rGHyBU4AqD
-   https://platform.openai.com/docs/guides/fine-tuning/use-a-fine-tuned-model

    -   gpt-3.5-turbo-0125
    -   davinci-002

-   tune with a word
-   tune with empty space
-   run a tdidf
-   write a blog post - making an AI oracle: finetuning for prophecy
-   write a blog post - findings on NLP like number of sentences and so on

### ideas

-   completely randomly
-   empty finetune
-   convert questino into word -> finetune word-sentence
-   rag questino into sentence -> finetune one sentence to the next

### preprocessing

-   unstructured open source
-   unstructured api
