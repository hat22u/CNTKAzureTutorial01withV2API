# CNTK Web Deploy Sample

You can deploy CNTK evaluation API solution with models trained via Python.

The [Azure evaluation tutorial](https://github.com/Microsoft/CNTK/tree/master/Examples/Evaluation/CNTKAzureTutorial01) is still referencing Eval V1 API.


However, we need to use CNTK Library API for models trained via Python.
The Microsoft.MSR.CNTK.Extensibility.Managed.IEvaluateModelManaged is part of Eval V1 API, and can only evaluate models trained via BrainScript.

Therefore, I revised [the tutorial](https://github.com/Microsoft/CNTK/tree/master/Examples/Evaluation/CNTKAzureTutorial01) to deploy Web API models trained via Python.

To run this project, please take a look at [this document](https://docs.microsoft.com/en-us/cognitive-toolkit/Evaluate-a-model-in-an-Azure-WebApi). The procedure is exactly same as the document.

This sample code resolves these issues.
- [Error while using TransferLearning model for evaluation (deploying model in Azure) #1933](https://github.com/Microsoft/CNTK/issues/1933)
- [How to deploy TransferLearning.model ? #1934](https://github.com/Microsoft/CNTK/issues/1934)

Perhaps, the tutorial will be updated in the future. However CNTK repository has over 700 issues now, and I suppose the priority of the tutorial project may be low.
I hope this code helps someone who want to deploy API solution with models trained via Python.

Yuki 
