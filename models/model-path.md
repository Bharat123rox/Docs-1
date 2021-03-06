# Default Model path

For an experiment to output a model in the Gradient system the resulting model files need to be written to the specified or default model path.

### PS\_MODEL\_PATH

Using the PS\_MODEL\_PATH environment variable is the easiest way to make sure you are outputting to the correct location. 

```python
model_dir = os.path.abspath(os.environ.get('PS_MODEL_PATH'))
# You can also use gradient_sdk:
from gradient_sdk.utils import model_dir
```

### Default paths

**Singlenode**: `--modelPath /artifacts` is currently the default for singlenode experiments. Output your model files there to appear in your Model Repository so that you can deploy it using Deployments

**Multinode:** The default model path for multinode experiments is /storage/models/&lt;experiment\_id&gt;/ 

{% hint style="info" %}
When in an on-premise/vpc environment, the default model path will be /shared/models/&lt;experiment\_id&gt;
{% endhint %}

