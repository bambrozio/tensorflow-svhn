```
/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/bin/python /Applications/PyCharm.app/Contents/helpers/pydev/pydevconsole.py --mode=client --port=58528
/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/lib/python2.7/site-packages/IPython/core/interactiveshell.py:726: UserWarning: Attempting to work in a virtualenv. If you encounter problems, please install IPython inside the virtualenv.
  warn("Attempting to work in a virtualenv. If you encounter problems, please "
import sys; print('Python %s on %s' % (sys.version, sys.platform))
sys.path.extend(['/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn'])
Python 2.7.10 (default, Feb 22 2019, 21:17:52) 
Type "copyright", "credits" or "license" for more information.
IPython 5.8.0 -- An enhanced Interactive Python.
?         -> Introduction and overview of IPython's features.
%quickref -> Quick reference.
help      -> Python's own help system.
object?   -> Details about 'object', use 'object??' for extra details.
PyDev console: using IPython 5.8.0
Python 2.7.10 (default, Feb 22 2019, 21:17:52) 
[GCC 4.2.1 Compatible Apple LLVM 10.0.1 (clang-1001.0.37.14)] on darwin
runfile('/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/train_classifier.py', wdir='/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn')
WARNING:tensorflow:From /Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/lib/python2.7/site-packages/tensorflow/python/framework/op_def_library.py:263: colocate_with (from tensorflow.python.framework.ops) is deprecated and will be removed in a future version.
Instructions for updating:
Colocations handled automatically by placer.
Starting without Saved Weights.
Training (65931, 32, 32, 3)
Valid (7326, 32, 32, 3)
Test (26032, 32, 32, 3)
Using drop out
WARNING:tensorflow:From /Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/svhn_model.py:123: calling dropout (from tensorflow.python.ops.nn_ops) with keep_prob is deprecated and will be removed in a future version.
Instructions for updating:
Please use `rate` instead of `keep_prob`. Rate should be set to `rate = 1 - keep_prob`.
WARNING:tensorflow:From /Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/train_classifier.py:71: softmax_cross_entropy_with_logits (from tensorflow.python.ops.nn_ops) is deprecated and will be removed in a future version.
Instructions for updating:
Future major versions of TensorFlow will allow gradients to flow
into the labels input on backprop by default.
See `tf.nn.softmax_cross_entropy_with_logits_v2`.
Not using dropout
WARNING:tensorflow:From /Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/lib/python2.7/site-packages/tensorflow/python/util/tf_should_use.py:193: initialize_all_variables (from tensorflow.python.ops.variables) is deprecated and will be removed after 2017-03-02.
Instructions for updating:
Use `tf.global_variables_initializer` instead.
2019-05-12 22:28:52.172558: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2 FMA
Validation Accuracy: 0.11%
Training Accuracy: 0.13%
Adding run metadata for 0
2019-05-12 22:28:53.707826: step 0, loss = 2.29  learning rate = 0.075000  (335.3 examples/sec; 0.76 sec/batch)
Mini-Batch Accuracy: 0.09%
(...)
```