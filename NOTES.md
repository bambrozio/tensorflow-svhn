Classifier (BATCH_SIZE = 256 and NUM_EPOCHS = 10)
```
/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/bin/python /Applications/PyCharm.app/Contents/helpers/pydev/pydevconsole.py --mode=client --port=58574
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
2019-05-12 22:35:50.348072: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2 FMA
Validation Accuracy: 0.11%
Training Accuracy: 0.13%
Adding run metadata for 0
2019-05-12 22:35:51.796044: step 0, loss = 2.28  learning rate = 0.075000  (352.2 examples/sec; 0.73 sec/batch)
Mini-Batch Accuracy: 0.05%

(...)

Mini-Batch Accuracy: 0.95%
2019-05-12 22:45:06.387072: step 1900, loss = 0.30  learning rate = 0.052375  (8.9 examples/sec; 28.79 sec/batch)
Mini-Batch Accuracy: 0.93%
Validation Accuracy: 0.90%
Training Accuracy: 0.96%
Adding run metadata for 2000
2019-05-12 22:45:35.745231: step 2000, loss = 0.16  learning rate = 0.052375  (8.9 examples/sec; 28.76 sec/batch)
Mini-Batch Accuracy: 0.95%
2019-05-12 22:46:04.535938: step 2100, loss = 0.22  learning rate = 0.049757  (8.9 examples/sec; 28.79 sec/batch)
Mini-Batch Accuracy: 0.95%
2019-05-12 22:46:33.176015: step 2200, loss = 0.24  learning rate = 0.049757  (8.9 examples/sec; 28.64 sec/batch)
Mini-Batch Accuracy: 0.93%
2019-05-12 22:47:01.718892: step 2300, loss = 0.34  learning rate = 0.049757  (9.0 examples/sec; 28.54 sec/batch)
Mini-Batch Accuracy: 0.93%
2019-05-12 22:47:30.538166: step 2400, loss = 0.37  learning rate = 0.047269  (8.9 examples/sec; 28.82 sec/batch)
Mini-Batch Accuracy: 0.89%
2019-05-12 22:47:59.338596: step 2500, loss = 0.25  learning rate = 0.047269  (8.9 examples/sec; 28.80 sec/batch)
Mini-Batch Accuracy: 0.93%
Model saved in file: classifier.ckpt
Test Accuracy: 0.91406%
```

Regression: (BATCH_SIZE = 32 and NUM_EPOCHS = 10)
```
/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/bin/python /Applications/PyCharm.app/Contents/helpers/pydev/pydevconsole.py --mode=client --port=58743
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
runfile('/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/train_regressor.py', wdir='/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn')
WARNING:tensorflow:From /Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/lib/python2.7/site-packages/tensorflow/python/framework/op_def_library.py:263: colocate_with (from tensorflow.python.framework.ops) is deprecated and will be removed in a future version.
Instructions for updating:
Colocations handled automatically by placer.
Starting without Saved Weights.
TrainData (30061, 64, 64, 3)
Valid Data (3341, 64, 64, 3)
Test Data (13068, 64, 64, 3)
2019-05-12 23:33:18.994250: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2 FMA
WARNING:tensorflow:From /Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/lib/python2.7/site-packages/tensorflow/python/util/tf_should_use.py:193: initialize_all_variables (from tensorflow.python.ops.variables) is deprecated and will be removed after 2017-03-02.
Instructions for updating:
Use `tf.global_variables_initializer` instead.
Model restored.
Validation Accuracy: 0.61
Training Set Accuracy: 0.44
Adding run metadata for 0
2019-05-12 23:33:43.875866: step 100, loss = 5.80  learning rate = 0.07  (1.3 examples/sec; 24.651 sec/batch)
Minibatch accuracy2: 0.62

(...)

2019-05-13 00:04:44.315360: step 8500, loss = 5.53  learning rate = 0.05  (1.5 examples/sec; 21.415 sec/batch)
Minibatch accuracy2: 0.62
2019-05-13 00:05:05.967146: step 8600, loss = 6.39  learning rate = 0.05  (1.5 examples/sec; 21.436 sec/batch)
Minibatch accuracy2: 0.59
2019-05-13 00:05:27.639811: step 8700, loss = 6.07  learning rate = 0.05  (1.5 examples/sec; 21.458 sec/batch)
Minibatch accuracy2: 0.62
2019-05-13 00:05:49.304660: step 8800, loss = 6.80  learning rate = 0.05  (1.5 examples/sec; 21.446 sec/batch)
Minibatch accuracy2: 0.58
2019-05-13 00:06:10.933294: step 8900, loss = 5.91  learning rate = 0.05  (1.5 examples/sec; 21.414 sec/batch)
Minibatch accuracy2: 0.62
Validation Accuracy: 0.63
Training Set Accuracy: 0.60
Adding run metadata for 9000
2019-05-13 00:06:54.628490: step 9100, loss = 5.85  learning rate = 0.05  (0.7 examples/sec; 43.481 sec/batch)
Minibatch accuracy2: 0.61
2019-05-13 00:07:16.316061: step 9200, loss = 6.41  learning rate = 0.05  (1.5 examples/sec; 21.472 sec/batch)
Minibatch accuracy2: 0.60
2019-05-13 00:07:37.976779: step 9300, loss = 5.84  learning rate = 0.05  (1.5 examples/sec; 21.437 sec/batch)
Minibatch accuracy2: 0.64
Test accuracy: 0.66
Model saved in file: regression.ckpt
```