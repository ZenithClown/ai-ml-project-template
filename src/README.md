<h1 align = "center">Information about <code>src</code> Directory</h1>

<div align = "justify">

A "_heart_" of any project is the `src` which contains the "source" files for the project. As a *production level* code template,
the directory provides three important directories as follows (I) `agents` : typically contains agent definations for a RNN
application; (II) `engine` : provides a suit of machine learning analytic functions to perform model training and analytics on
your dataset without giving up end-to-end performance; and (III) `models` : typically contains model definations.

## Logging Setup

In a *production server* it is recommended to use a [**`logger`**](https://docs.python.org/3/library/logging.html) instead of a
print statement. This allows robust controls in a flexible manner. A template logger configuration file is available in the
[config](../config/logging.yaml) directory.

```python
import yaml
import logging
import logging.config

...

def loggerConfig(filename : str):
  config = yaml.safe_load(open(filename, "r").read())
  logging.config.dictConfig(config)
  return

if __name__ == "__main__":
  loggerConfig("../config/logging.yaml")
  logger = logging.getLogger(__name__)
  ...
```

An advanced user may also use [**`structlog`**](https://www.structlog.org/en/stable/index.html) which acts as a wrapper to
generate logs in an asyncronous system. The minimalistic logging setup provides a seamless integration.

</div>
