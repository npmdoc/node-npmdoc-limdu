# api documentation for  [limdu (v0.9.2)](https://github.com/erelsgl/limdu#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-limdu.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-limdu) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-limdu.svg)](https://travis-ci.org/npmdoc/node-npmdoc-limdu)
#### A machine learning framework for Node.js. Supports multi-level classification and online learning.

[![NPM](https://nodei.co/npm/limdu.png?downloads=true)](https://www.npmjs.com/package/limdu)

[![apidoc](https://npmdoc.github.io/node-npmdoc-limdu/build/screenCapture.buildApidoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-limdu%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-limdu/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-limdu/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-limdu/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Erel Segal-haLevi",
        "email": "erelsgl@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/erelsgl/limdu/issues"
    },
    "contributors": [
        {
            "name": "Erel Segal-Halevi",
            "email": "erelsgl@gmail.com"
        },
        {
            "name": "Vasily Konovalov",
            "email": "vasili.konov@gmail.com"
        },
        {
            "name": "Mikkel Oscar Lyderik"
        },
        {
            "name": "junchaowu"
        }
    ],
    "dependencies": {
        "async": "*",
        "brain": "*",
        "graph-paths": "latest",
        "languagemodel": "latest",
        "sprintf": "*",
        "svm": "*",
        "temp": "*",
        "underscore": "*",
        "wordsworth": "*"
    },
    "description": "A machine learning framework for Node.js. Supports multi-level classification and online learning.",
    "devDependencies": {
        "mocha": ">=1.0.0",
        "should": ">=0.6.0"
    },
    "directories": {},
    "dist": {
        "shasum": "0b949760fb0c43c60d90a2c3d67b522f911f7916",
        "tarball": "https://registry.npmjs.org/limdu/-/limdu-0.9.2.tgz"
    },
    "engines": {
        "node": ">=0.12"
    },
    "gitHead": "686cff4dcede4b1277ae20730d83acbfc40381ed",
    "homepage": "https://github.com/erelsgl/limdu#readme",
    "keywords": [
        "classifier",
        "classification",
        "categorization",
        "text classification",
        "natural lanaguage understanding",
        "machine learning",
        "multi label",
        "multilabel",
        "multi class",
        "multiclass",
        "online learning",
        "naive bayes",
        "winnow",
        "perceptron",
        "SVM",
        "Linear SVM",
        "binary relevance",
        "one vs all"
    ],
    "license": "LGPL",
    "maintainers": [
        {
            "name": "erelsgl",
            "email": "erelsgl@gmail.com"
        }
    ],
    "name": "limdu",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/erelsgl/limdu.git"
    },
    "scripts": {
        "test": "mocha"
    },
    "version": "0.9.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module limdu](#apidoc.module.limdu)
1.  [function <span class="apidocSignatureSpan">limdu.</span>EnhancedClassifier_2014 (opts)](#apidoc.element.limdu.EnhancedClassifier_2014)
1.  [function <span class="apidocSignatureSpan">limdu.</span>EnhancedClassifier_2015 (opts)](#apidoc.element.limdu.EnhancedClassifier_2015)
1.  [function <span class="apidocSignatureSpan">limdu.</span>classifiers.Bayesian (options)](#apidoc.element.limdu.classifiers.Bayesian)
1.  [function <span class="apidocSignatureSpan">limdu.</span>classifiers.DecisionTree (opts)](#apidoc.element.limdu.classifiers.DecisionTree)
1.  [function <span class="apidocSignatureSpan">limdu.</span>classifiers.EnhancedClassifier (opts)](#apidoc.element.limdu.classifiers.EnhancedClassifier)
1.  [function <span class="apidocSignatureSpan">limdu.</span>classifiers.NeuralNetwork (options)](#apidoc.element.limdu.classifiers.NeuralNetwork)
1.  [function <span class="apidocSignatureSpan">limdu.</span>classifiers.Perceptron (opts)](#apidoc.element.limdu.classifiers.Perceptron)
1.  [function <span class="apidocSignatureSpan">limdu.</span>classifiers.SvmJs (opts)](#apidoc.element.limdu.classifiers.SvmJs)
1.  [function <span class="apidocSignatureSpan">limdu.</span>classifiers.SvmLinear (opts)](#apidoc.element.limdu.classifiers.SvmLinear)
1.  [function <span class="apidocSignatureSpan">limdu.</span>classifiers.SvmPerf (opts)](#apidoc.element.limdu.classifiers.SvmPerf)
1.  [function <span class="apidocSignatureSpan">limdu.</span>classifiers.Winnow (opts)](#apidoc.element.limdu.classifiers.Winnow)
1.  [function <span class="apidocSignatureSpan">limdu.</span>classifiers.kNN (opts)](#apidoc.element.limdu.classifiers.kNN)
1.  [function <span class="apidocSignatureSpan">limdu.</span>features.FeatureLookupTable ()](#apidoc.element.limdu.features.FeatureLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.</span>utils.PrecisionRecall ()](#apidoc.element.limdu.utils.PrecisionRecall)
1.  object <span class="apidocSignatureSpan">limdu.</span>EnhancedClassifier_2014.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>EnhancedClassifier_2015.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>arff
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.Bayesian.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.DecisionTree.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.EnhancedClassifier.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.NeuralNetwork.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.Perceptron.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.SvmJs.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.SvmLinear.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.SvmPerf.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.Winnow.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.kNN.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.multilabel
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.multilabel.Adaboost.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.multilabel.BinaryRelevance.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.multilabel.BinarySegmentation.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.multilabel.CrossLanguageModel.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.multilabel.Homer.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.multilabel.MetaLabeler.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.multilabel.MulticlassSegmentation.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.multilabel.PartialClassification.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.multilabel.PassiveAggressive.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>classifiers.multilabel.ThresholdClassifier.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>features
1.  object <span class="apidocSignatureSpan">limdu.</span>features.FeatureLookupTable.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>formats
1.  object <span class="apidocSignatureSpan">limdu.</span>hamming
1.  object <span class="apidocSignatureSpan">limdu.</span>json
1.  object <span class="apidocSignatureSpan">limdu.</span>list
1.  object <span class="apidocSignatureSpan">limdu.</span>svmlight
1.  object <span class="apidocSignatureSpan">limdu.</span>tsv
1.  object <span class="apidocSignatureSpan">limdu.</span>utils
1.  object <span class="apidocSignatureSpan">limdu.</span>utils.PrecisionRecall.prototype
1.  object <span class="apidocSignatureSpan">limdu.</span>utils.hash
1.  object <span class="apidocSignatureSpan">limdu.</span>utils.partitions

#### [module limdu.EnhancedClassifier_2014](#apidoc.module.limdu.EnhancedClassifier_2014)
1.  [function <span class="apidocSignatureSpan">limdu.</span>EnhancedClassifier_2014 (opts)](#apidoc.element.limdu.EnhancedClassifier_2014.EnhancedClassifier_2014)

#### [module limdu.EnhancedClassifier_2014.prototype](#apidoc.module.limdu.EnhancedClassifier_2014.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>backClassify (theClass)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.backClassify)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>classify (sample, explain, continuous_output, original, classifier_compare)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>classifyPart (sample, explain, continuous_output)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.classifyPart)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>correctFeatureSpelling (sample)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.correctFeatureSpelling)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>countFeatures (features)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.countFeatures)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>editFeatureValues (features, remove_unknown_features)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.editFeatureValues)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>featuresToArray (features)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.featuresToArray)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>fromJSON (json)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>getAllClasses ()](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.getAllClasses)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>instanceFilter (data)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.instanceFilter)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>normalizedSample (sample)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.normalizedSample)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>outputToFormat (data)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.outputToFormat)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>retrain ()](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.retrain)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>sampleToFeatures (sample, featureExtractor)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.sampleToFeatures)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>setFeatureExtractor (featureExtractor)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.setFeatureExtractor)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>setFeatureExtractorForClassification (featureExtractorForClassification)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.setFeatureExtractorForClassification)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.setFeatureLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>setLabelLookupTable (labelLookupTable)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.setLabelLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>setNormalizer (normalizer)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.setNormalizer)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>toJSON (callback)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>trainOnline (sample, classes)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.trainOnline)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>trainSpellChecker (features)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.trainSpellChecker)

#### [module limdu.EnhancedClassifier_2015](#apidoc.module.limdu.EnhancedClassifier_2015)
1.  [function <span class="apidocSignatureSpan">limdu.</span>EnhancedClassifier_2015 (opts)](#apidoc.element.limdu.EnhancedClassifier_2015.EnhancedClassifier_2015)

#### [module limdu.EnhancedClassifier_2015.prototype](#apidoc.module.limdu.EnhancedClassifier_2015.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>applyFeatureExpansion ()](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.applyFeatureExpansion)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>backClassify (theClass)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.backClassify)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>classify (sample, explain)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>classifyAsync (sample, explain, callback_global)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.classifyAsync)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>classifyBatch (testSet)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.classifyBatch)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>classifyPart (sample, explain, continuous_output)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.classifyPart)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>classifyPartAsync (sample, explain, callback)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.classifyPartAsync)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>correctFeatureSpelling (sample)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.correctFeatureSpelling)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>countFeatures (features)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.countFeatures)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>editFeatureValues (features, remove_unknown_features)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.editFeatureValues)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>featuresToArray (features)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.featuresToArray)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>fromJSON (json)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>getAllClasses ()](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.getAllClasses)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>instanceFilterRun (data)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.instanceFilterRun)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>normalizedSample (sample)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.normalizedSample)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>retrain ()](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.retrain)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>sampleToFeatures (sample, featureExtractor)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.sampleToFeatures)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>sampleToFeaturesAsync (sample, featureExtractor, callback)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.sampleToFeaturesAsync)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>setFeatureExpansion (featureExpansion)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.setFeatureExpansion)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>setFeatureExtractor (featureExtractor)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.setFeatureExtractor)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>setFeatureExtractorForClassification (featureExtractorForClassification)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.setFeatureExtractorForClassification)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.setFeatureLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>setInstanceFilter (instanceFilter)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.setInstanceFilter)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>setLabelLookupTable (labelLookupTable)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.setLabelLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>setNormalizer (normalizer)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.setNormalizer)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>toJSON (callback)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>trainBatchAsync (dataset, callbackg)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.trainBatchAsync)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>trainOnline (sample, classes)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.trainOnline)
1.  [function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>trainSpellChecker (features)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.trainSpellChecker)

#### [module limdu.arff](#apidoc.module.limdu.arff)
1.  [function <span class="apidocSignatureSpan">limdu.arff.</span>toARFF (dataset, relationName, featureExtractor)](#apidoc.element.limdu.arff.toARFF)
1.  [function <span class="apidocSignatureSpan">limdu.arff.</span>toARFFs (outputFolder, mapFileNameToDataset, featureExtractor)](#apidoc.element.limdu.arff.toARFFs)

#### [module limdu.classifiers](#apidoc.module.limdu.classifiers)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>Bayesian (options)](#apidoc.element.limdu.classifiers.Bayesian)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>DecisionTree (opts)](#apidoc.element.limdu.classifiers.DecisionTree)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>EnhancedClassifier (opts)](#apidoc.element.limdu.classifiers.EnhancedClassifier)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>NeuralNetwork (options)](#apidoc.element.limdu.classifiers.NeuralNetwork)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>Perceptron (opts)](#apidoc.element.limdu.classifiers.Perceptron)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>SvmJs (opts)](#apidoc.element.limdu.classifiers.SvmJs)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>SvmLinear (opts)](#apidoc.element.limdu.classifiers.SvmLinear)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>SvmPerf (opts)](#apidoc.element.limdu.classifiers.SvmPerf)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>Winnow (opts)](#apidoc.element.limdu.classifiers.Winnow)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>kNN (opts)](#apidoc.element.limdu.classifiers.kNN)
1.  object <span class="apidocSignatureSpan">limdu.classifiers.</span>multilabel

#### [module limdu.classifiers.Bayesian](#apidoc.module.limdu.classifiers.Bayesian)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>Bayesian (options)](#apidoc.element.limdu.classifiers.Bayesian.Bayesian)

#### [module limdu.classifiers.Bayesian.prototype](#apidoc.module.limdu.classifiers.Bayesian.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>bestMatch (pairs)](#apidoc.element.limdu.classifiers.Bayesian.prototype.bestMatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>classify (document, explain)](#apidoc.element.limdu.classifiers.Bayesian.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.Bayesian.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>fromJSON (json, callback)](#apidoc.element.limdu.classifiers.Bayesian.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>getCatProbs (cats, document, counts)](#apidoc.element.limdu.classifiers.Bayesian.prototype.getCatProbs)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>getCats (callback)](#apidoc.element.limdu.classifiers.Bayesian.prototype.getCats)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>getProbsSync (document)](#apidoc.element.limdu.classifiers.Bayesian.prototype.getProbsSync)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>getWordCounts (words, cats, callback)](#apidoc.element.limdu.classifiers.Bayesian.prototype.getWordCounts)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>incDocCounts (samples, callback)](#apidoc.element.limdu.classifiers.Bayesian.prototype.incDocCounts)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>setThresholds (thresholds)](#apidoc.element.limdu.classifiers.Bayesian.prototype.setThresholds)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>toJSON (callback)](#apidoc.element.limdu.classifiers.Bayesian.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>trainBatch (data)](#apidoc.element.limdu.classifiers.Bayesian.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>trainOnline (document, category)](#apidoc.element.limdu.classifiers.Bayesian.prototype.trainOnline)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>wordProb (word, cat, cats, wordCounts)](#apidoc.element.limdu.classifiers.Bayesian.prototype.wordProb)

#### [module limdu.classifiers.DecisionTree](#apidoc.module.limdu.classifiers.DecisionTree)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>DecisionTree (opts)](#apidoc.element.limdu.classifiers.DecisionTree.DecisionTree)

#### [module limdu.classifiers.DecisionTree.prototype](#apidoc.module.limdu.classifiers.DecisionTree.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>classify (features, explain, continuous_output)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>count (a, l)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.count)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>createTree (dataset, features)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.createTree)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>entropy (vals)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.entropy)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>extractFeatures (dataset)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.extractFeatures)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>gain (dataset, feature)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.gain)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>log2 (n)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.log2)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>maxGain (dataset, features)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.maxGain)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>mostCommon (l)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.mostCommon)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>prob (val, vals)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.prob)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>randomTag ()](#apidoc.element.limdu.classifiers.DecisionTree.prototype.randomTag)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.setFeatureLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>toJSON (folder)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.trainBatch)

#### [module limdu.classifiers.EnhancedClassifier](#apidoc.module.limdu.classifiers.EnhancedClassifier)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>EnhancedClassifier (opts)](#apidoc.element.limdu.classifiers.EnhancedClassifier.EnhancedClassifier)

#### [module limdu.classifiers.EnhancedClassifier.prototype](#apidoc.module.limdu.classifiers.EnhancedClassifier.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>backClassify (theClass)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.backClassify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>classify (sample, explain, continuous_output, original, classifier_compare)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>classifyPart (sample, explain, continuous_output)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.classifyPart)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>correctFeatureSpelling (sample)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.correctFeatureSpelling)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>countFeatures (features)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.countFeatures)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>editFeatureValues (features, remove_unknown_features)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.editFeatureValues)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>featuresToArray (features)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.featuresToArray)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.getAllClasses)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>instanceFilter (data)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.instanceFilter)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>normalizedSample (sample)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.normalizedSample)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>outputToFormat (data)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.outputToFormat)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>retrain ()](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.retrain)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>sampleToFeatures (sample, featureExtractor)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.sampleToFeatures)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>setFeatureExtractor (featureExtractor)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.setFeatureExtractor)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>setFeatureExtractorForClassification (featureExtractorForClassification)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.setFeatureExtractorForClassification)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.setFeatureLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>setLabelLookupTable (labelLookupTable)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.setLabelLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>setNormalizer (normalizer)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.setNormalizer)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>toJSON (callback)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>trainOnline (sample, classes)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.trainOnline)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>trainSpellChecker (features)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.trainSpellChecker)

#### [module limdu.classifiers.NeuralNetwork](#apidoc.module.limdu.classifiers.NeuralNetwork)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>NeuralNetwork (options)](#apidoc.element.limdu.classifiers.NeuralNetwork.NeuralNetwork)

#### [module limdu.classifiers.NeuralNetwork.prototype](#apidoc.module.limdu.classifiers.NeuralNetwork.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>adjustWeights (learningRate)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.adjustWeights)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>calculateDeltas (target)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.calculateDeltas)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>classify (input)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>createTrainStream (opts)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.createTrainStream)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>formatData (data)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.formatData)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>initialize (sizes)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>run (input)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.run)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>runInput (input)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.runInput)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>test (data)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.test)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>toFunction ()](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.toFunction)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>train (data, options)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.train)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>trainOnline ()](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.trainOnline)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>trainPattern (input, target, learningRate)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.trainPattern)

#### [module limdu.classifiers.Perceptron](#apidoc.module.limdu.classifiers.Perceptron)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>Perceptron (opts)](#apidoc.element.limdu.classifiers.Perceptron.Perceptron)

#### [module limdu.classifiers.Perceptron.prototype](#apidoc.module.limdu.classifiers.Perceptron.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>adjust (result, expected, input, feature)](#apidoc.element.limdu.classifiers.Perceptron.prototype.adjust)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>classify (features, explain, continuous_output)](#apidoc.element.limdu.classifiers.Perceptron.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.Perceptron.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.Perceptron.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>normalized_features (features, remove_unknown_features)](#apidoc.element.limdu.classifiers.Perceptron.prototype.normalized_features)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>perceive_features (features, continuous_output, weights_for_classification, explain)](#apidoc.element.limdu.classifiers.Perceptron.prototype.perceive_features)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.Perceptron.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.Perceptron.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>trainOnline (features, expected)](#apidoc.element.limdu.classifiers.Perceptron.prototype.trainOnline)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>train_features (features, expected)](#apidoc.element.limdu.classifiers.Perceptron.prototype.train_features)

#### [module limdu.classifiers.SvmJs](#apidoc.module.limdu.classifiers.SvmJs)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>SvmJs (opts)](#apidoc.element.limdu.classifiers.SvmJs.SvmJs)

#### [module limdu.classifiers.SvmJs.prototype](#apidoc.module.limdu.classifiers.SvmJs.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmJs.prototype.</span>classify (features, explain, continuous_output)](#apidoc.element.limdu.classifiers.SvmJs.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmJs.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.SvmJs.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmJs.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.SvmJs.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmJs.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.SvmJs.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmJs.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.SvmJs.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmJs.prototype.</span>trainOnline (features, label)](#apidoc.element.limdu.classifiers.SvmJs.prototype.trainOnline)

#### [module limdu.classifiers.SvmLinear](#apidoc.module.limdu.classifiers.SvmLinear)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>SvmLinear (opts)](#apidoc.element.limdu.classifiers.SvmLinear.SvmLinear)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.</span>isInstalled ()](#apidoc.element.limdu.classifiers.SvmLinear.isInstalled)

#### [module limdu.classifiers.SvmLinear.prototype](#apidoc.module.limdu.classifiers.SvmLinear.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>classify (features, explain, continuous_output)](#apidoc.element.limdu.classifiers.SvmLinear.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.SvmLinear.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>classifyBatch (trainset)](#apidoc.element.limdu.classifiers.SvmLinear.prototype.classifyBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.SvmLinear.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>getModelWeights ()](#apidoc.element.limdu.classifiers.SvmLinear.prototype.getModelWeights)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.SvmLinear.prototype.setFeatureLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>setModel (modelFileString)](#apidoc.element.limdu.classifiers.SvmLinear.prototype.setModel)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.SvmLinear.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.SvmLinear.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>trainOnline (features, expected)](#apidoc.element.limdu.classifiers.SvmLinear.prototype.trainOnline)

#### [module limdu.classifiers.SvmPerf](#apidoc.module.limdu.classifiers.SvmPerf)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>SvmPerf (opts)](#apidoc.element.limdu.classifiers.SvmPerf.SvmPerf)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.</span>isInstalled ()](#apidoc.element.limdu.classifiers.SvmPerf.isInstalled)

#### [module limdu.classifiers.SvmPerf.prototype](#apidoc.module.limdu.classifiers.SvmPerf.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>classify (features, explain, continuous_output)](#apidoc.element.limdu.classifiers.SvmPerf.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.SvmPerf.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.SvmPerf.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>getFeatures ()](#apidoc.element.limdu.classifiers.SvmPerf.prototype.getFeatures)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>getModelWeights ()](#apidoc.element.limdu.classifiers.SvmPerf.prototype.getModelWeights)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.SvmPerf.prototype.setFeatureLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>setModel (modelString)](#apidoc.element.limdu.classifiers.SvmPerf.prototype.setModel)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.SvmPerf.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.SvmPerf.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>trainOnline (features, expected)](#apidoc.element.limdu.classifiers.SvmPerf.prototype.trainOnline)

#### [module limdu.classifiers.Winnow](#apidoc.module.limdu.classifiers.Winnow)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>Winnow (opts)](#apidoc.element.limdu.classifiers.Winnow.Winnow)

#### [module limdu.classifiers.Winnow.prototype](#apidoc.module.limdu.classifiers.Winnow.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>classify (features, explain, continuous_output)](#apidoc.element.limdu.classifiers.Winnow.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.Winnow.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>editFeatureValues (features, remove_unknown_features)](#apidoc.element.limdu.classifiers.Winnow.prototype.editFeatureValues)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.Winnow.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>perceive_features (features, continuous_output, positive_weights_for_classification, negative_weights_for_classification, explain)](#apidoc.element.limdu.classifiers.Winnow.prototype.perceive_features)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>toJSON (folder)](#apidoc.element.limdu.classifiers.Winnow.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.Winnow.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>trainOnline (features, expected)](#apidoc.element.limdu.classifiers.Winnow.prototype.trainOnline)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>train_features (features, expected)](#apidoc.element.limdu.classifiers.Winnow.prototype.train_features)

#### [module limdu.classifiers.kNN](#apidoc.module.limdu.classifiers.kNN)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.</span>kNN (opts)](#apidoc.element.limdu.classifiers.kNN.kNN)

#### [module limdu.classifiers.kNN.prototype](#apidoc.module.limdu.classifiers.kNN.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>classify (sample, explain)](#apidoc.element.limdu.classifiers.kNN.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.kNN.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>complement (input)](#apidoc.element.limdu.classifiers.kNN.prototype.complement)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.kNN.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.kNN.prototype.getAllClasses)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.kNN.prototype.setFeatureLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>stringifyClass (aClass)](#apidoc.element.limdu.classifiers.kNN.prototype.stringifyClass)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.kNN.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.kNN.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>trainOnline (sample, labels)](#apidoc.element.limdu.classifiers.kNN.prototype.trainOnline)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>translaterow (row)](#apidoc.element.limdu.classifiers.kNN.prototype.translaterow)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>translatetrain (input)](#apidoc.element.limdu.classifiers.kNN.prototype.translatetrain)

#### [module limdu.classifiers.multilabel](#apidoc.module.limdu.classifiers.multilabel)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>Adaboost (opts)](#apidoc.element.limdu.classifiers.multilabel.Adaboost)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>BinaryRelevance (opts)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>BinarySegmentation (opts)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>CrossLanguageModel (opts)](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>Homer (opts)](#apidoc.element.limdu.classifiers.multilabel.Homer)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>MetaLabeler (opts)](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>MulticlassSegmentation (opts)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>PartialClassification (opts)](#apidoc.element.limdu.classifiers.multilabel.PartialClassification)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>PassiveAggressive (opts)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>ThresholdClassifier (opts)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier)

#### [module limdu.classifiers.multilabel.Adaboost.prototype](#apidoc.module.limdu.classifiers.multilabel.Adaboost.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>classify (sample, explain)](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.getAllClasses)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.setFeatureLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>stringifyClass (aClass)](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.stringifyClass)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>trainOnline (sample, labels)](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.trainOnline)

#### [module limdu.classifiers.multilabel.BinaryRelevance.prototype](#apidoc.module.limdu.classifiers.multilabel.BinaryRelevance.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>classify (sample, explain, withScores)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>classifyBatch (testSet)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.classifyBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.getAllClasses)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>makeSureClassifierExists (label)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.makeSureClassifierExists)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.setFeatureLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>trainOnline (sample, labels)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.trainOnline)

#### [module limdu.classifiers.multilabel.BinarySegmentation.prototype](#apidoc.module.limdu.classifiers.multilabel.BinarySegmentation.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>bestClassOfSegment (segment, explain)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.bestClassOfSegment)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>cheapestSegmentSplitStrategy (words, accumulatedClasses, explain, explanations)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.cheapestSegmentSplitStrategy)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>classify (sentence, explain)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>classifySegment (segment, explain)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.classifySegment)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>fromJSON (json, callback)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>longestSegmentSplitStrategy (words, accumulatedClasses, explain, explanations)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.longestSegmentSplitStrategy)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.setFeatureLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>shortestSegmentSplitStrategy (words, accumulatedClasses, explain, explanations)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.shortestSegmentSplitStrategy)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>toJSON (callback)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>trainOnline (sample, classes)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.trainOnline)

#### [module limdu.classifiers.multilabel.CrossLanguageModel.prototype](#apidoc.module.limdu.classifiers.multilabel.CrossLanguageModel.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.CrossLanguageModel.prototype.</span>classify (features, explain, withScores)](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.CrossLanguageModel.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.CrossLanguageModel.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.CrossLanguageModel.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.getAllClasses)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.CrossLanguageModel.prototype.</span>labelsToFeatures (labels)](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.labelsToFeatures)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.CrossLanguageModel.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.CrossLanguageModel.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.CrossLanguageModel.prototype.</span>trainOnline (features, labels)](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.trainOnline)

#### [module limdu.classifiers.multilabel.Homer.prototype](#apidoc.module.limdu.classifiers.multilabel.Homer.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>classify (sample, explain)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>classifyRecursive (sample, explain, treeNode, depth)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.classifyRecursive)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>fromJSONRecursive (treeNodeJson)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.fromJSONRecursive)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.getAllClasses)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>newMultilabelClassifier ()](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.newMultilabelClassifier)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.setFeatureLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>setFeatureLookupTableRecursive (featureLookupTable, treeNode)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.setFeatureLookupTableRecursive)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>toJSONRecursive (treeNode)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.toJSONRecursive)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>trainBatchRecursive (dataset, treeNode)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.trainBatchRecursive)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>trainOnline (sample, labels)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.trainOnline)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>trainOnlineRecursive (sample, splitLabels, treeNode)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.trainOnlineRecursive)

#### [module limdu.classifiers.multilabel.MetaLabeler.prototype](#apidoc.module.limdu.classifiers.multilabel.MetaLabeler.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MetaLabeler.prototype.</span>classify (sample, explain)](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MetaLabeler.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MetaLabeler.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MetaLabeler.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.getAllClasses)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MetaLabeler.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.setFeatureLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MetaLabeler.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MetaLabeler.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MetaLabeler.prototype.</span>trainOnline (sample, labels)](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.trainOnline)

#### [module limdu.classifiers.multilabel.MulticlassSegmentation.prototype](#apidoc.module.limdu.classifiers.multilabel.MulticlassSegmentation.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>bestClassOfSegment (segment)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.bestClassOfSegment)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>cheapestSegmentSplitStrategy (words, accumulatedClasses, explain, explanations)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.cheapestSegmentSplitStrategy)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>classify (sentence, explain)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>classifySegment (segment, explain)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.classifySegment)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>sampleToFeatures (sample, featureExtractor)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.sampleToFeatures)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>trainOnline (sample, classes)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.trainOnline)

#### [module limdu.classifiers.multilabel.PartialClassification.prototype](#apidoc.module.limdu.classifiers.multilabel.PartialClassification.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>classify (sample, explain, continuous_output)](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.getAllClasses)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>intializeClassifiers (numberofclassifiers, multilabelClassifierType)](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.intializeClassifiers)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.setFeatureLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>trainOnline (sample, labels)](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.trainOnline)

#### [module limdu.classifiers.multilabel.PassiveAggressive.prototype](#apidoc.module.limdu.classifiers.multilabel.PassiveAggressive.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>addClasses (classes)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.addClasses)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>classify (features, explain, withScores)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>editFeatureValues (features, remove_unknown_features)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.editFeatureValues)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>fromJSON (json, callback)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.getAllClasses)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>predict (features, averaging, explain)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.predict)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>toJSON (callback)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>trainOnline (features, classes)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.trainOnline)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>update (sample, classes)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.update)

#### [module limdu.classifiers.multilabel.ThresholdClassifier.prototype](#apidoc.module.limdu.classifiers.multilabel.ThresholdClassifier.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>CalculatePerformance (list_of_scores, testSet, FN)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.CalculatePerformance)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>classify (sample, explain)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.classify)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.classifyAndLog)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.getAllClasses)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>receiveScores (dataset)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.receiveScores)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.setFeatureLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.trainBatch)
1.  [function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>trainOnline (sample, labels)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.trainOnline)

#### [module limdu.features](#apidoc.module.limdu.features)
1.  [function <span class="apidocSignatureSpan">limdu.features.</span>CollectionOfExtractors (extractors)](#apidoc.element.limdu.features.CollectionOfExtractors)
1.  [function <span class="apidocSignatureSpan">limdu.features.</span>FeatureLookupTable ()](#apidoc.element.limdu.features.FeatureLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.features.</span>Hypernyms (hypernyms)](#apidoc.element.limdu.features.Hypernyms)
1.  [function <span class="apidocSignatureSpan">limdu.features.</span>LowerCaseNormalizer (sample)](#apidoc.element.limdu.features.LowerCaseNormalizer)
1.  [function <span class="apidocSignatureSpan">limdu.features.</span>NGramsFromArray (numOfWords, gap, grams, features)](#apidoc.element.limdu.features.NGramsFromArray)
1.  [function <span class="apidocSignatureSpan">limdu.features.</span>NGramsOfLetters (numOfLetters, caseSensitive)](#apidoc.element.limdu.features.NGramsOfLetters)
1.  [function <span class="apidocSignatureSpan">limdu.features.</span>NGramsOfWords (numOfWords, gap)](#apidoc.element.limdu.features.NGramsOfWords)
1.  [function <span class="apidocSignatureSpan">limdu.features.</span>RegexpNormalizer (normalizations)](#apidoc.element.limdu.features.RegexpNormalizer)
1.  [function <span class="apidocSignatureSpan">limdu.features.</span>RegexpSplitter (regexpString, delimitersToInclude)](#apidoc.element.limdu.features.RegexpSplitter)
1.  [function <span class="apidocSignatureSpan">limdu.features.</span>call (featureExtractor, sample)](#apidoc.element.limdu.features.call)
1.  [function <span class="apidocSignatureSpan">limdu.features.</span>normalize (featureExtractorOrArray)](#apidoc.element.limdu.features.normalize)

#### [module limdu.features.FeatureLookupTable](#apidoc.module.limdu.features.FeatureLookupTable)
1.  [function <span class="apidocSignatureSpan">limdu.features.</span>FeatureLookupTable ()](#apidoc.element.limdu.features.FeatureLookupTable.FeatureLookupTable)

#### [module limdu.features.FeatureLookupTable.prototype](#apidoc.module.limdu.features.FeatureLookupTable.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>addFeature (feature)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.addFeature)
1.  [function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>addFeatures (hash)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.addFeatures)
1.  [function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>addFeaturess (hashes)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.addFeaturess)
1.  [function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>arrayToHash (array)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.arrayToHash)
1.  [function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>arraysToHashes (arrays)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.arraysToHashes)
1.  [function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>featureToNumber (feature)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.featureToNumber)
1.  [function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>fromJSON (json)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>hashToArray (hash)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.hashToArray)
1.  [function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>hashesToArrays (hashes)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.hashesToArrays)
1.  [function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>numberToFeature (number)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.numberToFeature)
1.  [function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>toJSON ()](#apidoc.element.limdu.features.FeatureLookupTable.prototype.toJSON)

#### [module limdu.hamming](#apidoc.module.limdu.hamming)
1.  [function <span class="apidocSignatureSpan">limdu.hamming.</span>hammingDistance (a, b)](#apidoc.element.limdu.hamming.hammingDistance)

#### [module limdu.json](#apidoc.module.limdu.json)
1.  [function <span class="apidocSignatureSpan">limdu.json.</span>toJSON (dataset)](#apidoc.element.limdu.json.toJSON)

#### [module limdu.list](#apidoc.module.limdu.list)
1.  [function <span class="apidocSignatureSpan">limdu.list.</span>average (list)](#apidoc.element.limdu.list.average)
1.  [function <span class="apidocSignatureSpan">limdu.list.</span>clonedataset (set)](#apidoc.element.limdu.list.clonedataset)
1.  [function <span class="apidocSignatureSpan">limdu.list.</span>listembed (label)](#apidoc.element.limdu.list.listembed)
1.  [function <span class="apidocSignatureSpan">limdu.list.</span>median (values)](#apidoc.element.limdu.list.median)
1.  [function <span class="apidocSignatureSpan">limdu.list.</span>variance (list)](#apidoc.element.limdu.list.variance)

#### [module limdu.svmlight](#apidoc.module.limdu.svmlight)
1.  [function <span class="apidocSignatureSpan">limdu.svmlight.</span>toSvmLight (dataset, bias, binarize, firstFeatureNumber)](#apidoc.element.limdu.svmlight.toSvmLight)

#### [module limdu.tsv](#apidoc.module.limdu.tsv)
1.  [function <span class="apidocSignatureSpan">limdu.tsv.</span>toTSV (dataset, separator)](#apidoc.element.limdu.tsv.toTSV)

#### [module limdu.utils](#apidoc.module.limdu.utils)
1.  [function <span class="apidocSignatureSpan">limdu.utils.</span>PrecisionRecall ()](#apidoc.element.limdu.utils.PrecisionRecall)
1.  [function <span class="apidocSignatureSpan">limdu.utils.</span>hammingDistance (a, b)](#apidoc.element.limdu.utils.hammingDistance)
1.  object <span class="apidocSignatureSpan">limdu.utils.</span>hash
1.  object <span class="apidocSignatureSpan">limdu.utils.</span>partitions

#### [module limdu.utils.PrecisionRecall](#apidoc.module.limdu.utils.PrecisionRecall)
1.  [function <span class="apidocSignatureSpan">limdu.utils.</span>PrecisionRecall ()](#apidoc.element.limdu.utils.PrecisionRecall.PrecisionRecall)

#### [module limdu.utils.PrecisionRecall.prototype](#apidoc.module.limdu.utils.PrecisionRecall.prototype)
1.  [function <span class="apidocSignatureSpan">limdu.utils.PrecisionRecall.prototype.</span>addCase (expected, actual)](#apidoc.element.limdu.utils.PrecisionRecall.prototype.addCase)
1.  [function <span class="apidocSignatureSpan">limdu.utils.PrecisionRecall.prototype.</span>addCases (expectedClasses, actualClasses, logTruePositives)](#apidoc.element.limdu.utils.PrecisionRecall.prototype.addCases)
1.  [function <span class="apidocSignatureSpan">limdu.utils.PrecisionRecall.prototype.</span>addCasesHash (expectedClasses, actualClasses, logTruePositives )](#apidoc.element.limdu.utils.PrecisionRecall.prototype.addCasesHash)
1.  [function <span class="apidocSignatureSpan">limdu.utils.PrecisionRecall.prototype.</span>calculateStats ()](#apidoc.element.limdu.utils.PrecisionRecall.prototype.calculateStats)
1.  [function <span class="apidocSignatureSpan">limdu.utils.PrecisionRecall.prototype.</span>retrieveLabels ()](#apidoc.element.limdu.utils.PrecisionRecall.prototype.retrieveLabels)

#### [module limdu.utils.hash](#apidoc.module.limdu.utils.hash)
1.  [function <span class="apidocSignatureSpan">limdu.utils.hash.</span>add (target, source)](#apidoc.element.limdu.utils.hash.add)
1.  [function <span class="apidocSignatureSpan">limdu.utils.hash.</span>addtimes (target, scalar, source)](#apidoc.element.limdu.utils.hash.addtimes)
1.  [function <span class="apidocSignatureSpan">limdu.utils.hash.</span>fromString (string)](#apidoc.element.limdu.utils.hash.fromString)
1.  [function <span class="apidocSignatureSpan">limdu.utils.hash.</span>inner_product (features, weights)](#apidoc.element.limdu.utils.hash.inner_product)
1.  [function <span class="apidocSignatureSpan">limdu.utils.hash.</span>inner_product_matrix (features, weights)](#apidoc.element.limdu.utils.hash.inner_product_matrix)
1.  [function <span class="apidocSignatureSpan">limdu.utils.hash.</span>multiply (target, source)](#apidoc.element.limdu.utils.hash.multiply)
1.  [function <span class="apidocSignatureSpan">limdu.utils.hash.</span>multiply_scalar (target, source)](#apidoc.element.limdu.utils.hash.multiply_scalar)
1.  [function <span class="apidocSignatureSpan">limdu.utils.hash.</span>normalize_sum_of_squares_to_1 (features)](#apidoc.element.limdu.utils.hash.normalize_sum_of_squares_to_1)
1.  [function <span class="apidocSignatureSpan">limdu.utils.hash.</span>normalize_sum_of_values_to_1 (features)](#apidoc.element.limdu.utils.hash.normalize_sum_of_values_to_1)
1.  [function <span class="apidocSignatureSpan">limdu.utils.hash.</span>normalized (object)](#apidoc.element.limdu.utils.hash.normalized)
1.  [function <span class="apidocSignatureSpan">limdu.utils.hash.</span>stringify_sorted (weights, separator)](#apidoc.element.limdu.utils.hash.stringify_sorted)
1.  [function <span class="apidocSignatureSpan">limdu.utils.hash.</span>sum_of_absolute_values (weights)](#apidoc.element.limdu.utils.hash.sum_of_absolute_values)
1.  [function <span class="apidocSignatureSpan">limdu.utils.hash.</span>sum_of_square_values (weights)](#apidoc.element.limdu.utils.hash.sum_of_square_values)
1.  [function <span class="apidocSignatureSpan">limdu.utils.hash.</span>sum_of_values (weights)](#apidoc.element.limdu.utils.hash.sum_of_values)

#### [module limdu.utils.partitions](#apidoc.module.limdu.utils.partitions)
1.  [function <span class="apidocSignatureSpan">limdu.utils.</span>partitions (dataset, numOfPartitions, callback)](#apidoc.element.limdu.utils.partitions.partitions)
1.  [function <span class="apidocSignatureSpan">limdu.utils.partitions.</span>partition (dataset, testSetStart, testSetCount)](#apidoc.element.limdu.utils.partitions.partition)
1.  [function <span class="apidocSignatureSpan">limdu.utils.partitions.</span>partitions_consistent (dataset, numOfPartitions, callback)](#apidoc.element.limdu.utils.partitions.partitions_consistent)
1.  [function <span class="apidocSignatureSpan">limdu.utils.partitions.</span>partitions_consistent_by_fold (dataset, numOfPartitions, partitionIndex)](#apidoc.element.limdu.utils.partitions.partitions_consistent_by_fold)
1.  [function <span class="apidocSignatureSpan">limdu.utils.partitions.</span>partitions_hash (datasetor, numOfPartitions, callback)](#apidoc.element.limdu.utils.partitions.partitions_hash)
1.  [function <span class="apidocSignatureSpan">limdu.utils.partitions.</span>partitions_hash_fold (datasetor, numOfPartitions, fold )](#apidoc.element.limdu.utils.partitions.partitions_hash_fold)
1.  [function <span class="apidocSignatureSpan">limdu.utils.partitions.</span>partitions_reverese (dataset, numOfPartitions, callback)](#apidoc.element.limdu.utils.partitions.partitions_reverese)



# <a name="apidoc.module.limdu"></a>[module limdu](#apidoc.module.limdu)

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014"></a>[function <span class="apidocSignatureSpan">limdu.</span>EnhancedClassifier_2014 (opts)](#apidoc.element.limdu.EnhancedClassifier_2014)
- description and source-code
```javascript
EnhancedClassifier_2014 = function (opts) {
	if (!opts.classifierType) {
		console.dir(opts);
		throw new Error("opts must contain classifierType");
	}

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
    	this.tfidf = new opts.TfIdfImpl
		this.featureDocumentFrequency = {};
		}
	this.bias = opts.bias;

	this.spellChecker = opts.spellChecker;
	this.tokenizer = opts.tokenizer;
	this.instanceFilterRule = opts.instanceFilter

	// this.spellChecker =  [require('wordsworth').getInstance(), require('wordsworth').getInstance()],
	// this.pastTrainingSamples = opts.pastTrainingSamples;
	// TODO: it looks like the method with creating an array at the definition
	// create an array with the same pointer for every classifier of the given class
	
	this.pastTrainingSamples = []

	this.InputSplitLabel = opts.InputSplitLabel
	this.OutputSplitLabel = opts.OutputSplitLabel
	this.TestSplitLabel = opts.TestSplitLabel
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015"></a>[function <span class="apidocSignatureSpan">limdu.</span>EnhancedClassifier_2015 (opts)](#apidoc.element.limdu.EnhancedClassifier_2015)
- description and source-code
```javascript
EnhancedClassifier_2015 = function (opts) {
	if (!opts.classifierType) {
		console.dir(opts);
		throw new Error("opts must contain classifierType");
	}

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	// this.setFeatureLookupTable(opts.featureLookupTable);
	this.setFeatureLookupTable(new ftrs.FeatureLookupTable());

	this.setLabelLookupTable(opts.labelLookupTable);
	this.setInstanceFilter(opts.instanceFilter);

	this.setFeatureExpansion(opts.featureExpansion);
	this.featureExpansionScale = opts.featureExpansionScale;
	this.featureExpansionPhrase = opts.featureExpansionPhrase;
	this.featureFine = opts.featureFine;

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
    	this.tfidf = new opts.TfIdfImpl
		this.featureDocumentFrequency = {};
		}
	this.bias = opts.bias;

	this.spellChecker = opts.spellChecker;
	this.tokenizer = opts.tokenizer;

	// this.spellChecker =  [require('wordsworth').getInstance(), require('wordsworth').getInstance()],
	// this.pastTrainingSamples = opts.pastTrainingSamples;
	// TODO: it looks like the method with creating an array at the definition
	// create an array with the same pointer for every classifier of the given class
	
	this.pastTrainingSamples = []

	this.preProcessor = opts.preProcessor
	this.postProcessor = opts.postProcessor
	// this.TestSplitLabel = opts.TestSplitLabel
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.Bayesian"></a>[function <span class="apidocSignatureSpan">limdu.</span>classifiers.Bayesian (options)](#apidoc.element.limdu.classifiers.Bayesian)
- description and source-code
```javascript
classifiers.Bayesian = function (options) {
	options = options || {}
	this.thresholds = options.thresholds || {};
	this.globalThreshold = options.globalThreshold || 1;
	this.default = options.default || 'unclassified';
	this.weight = options.weight || 1;
	this.assumed = options.assumed || 0.5;
	this.normalizeOutputProbabilities = options.normalizeOutputProbabilities||false;
	this.calculateRelativeProbabilities = options.calculateRelativeProbabilities||false;

	var backend = options.backend || { type: 'memory' };
	switch(backend.type.toLowerCase()) {
		case 'redis':
			//this.backend = new (require("./backends/redis").RedisBackend)(backend.options);
			throw new Error("Redis backend support was dropped, in order to remove dependencies");
			break;
		case 'localstorage':
			this.backend = new (require("./backends/localStorage")
										 .LocalStorageBackend)(backend.options);
			break;
		default:
			this.backend = new (require("./backends/memory").MemoryBackend)();
	}
}
```
- example usage
```shell
...
'''

### Explanations

Some classifiers can return "explanations" - additional information that explains how the classification result has been derived
:

'''js
var colorClassifier = new limdu.classifiers.Bayesian();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 'black'},
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 'white'},
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 'white'},
	]);
...
```

#### <a name="apidoc.element.limdu.classifiers.DecisionTree"></a>[function <span class="apidocSignatureSpan">limdu.</span>classifiers.DecisionTree (opts)](#apidoc.element.limdu.classifiers.DecisionTree)
- description and source-code
```javascript
function DecisionTree(opts) {
	if (!opts) opts = {}
	// this.debug = opts.debug || false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier"></a>[function <span class="apidocSignatureSpan">limdu.</span>classifiers.EnhancedClassifier (opts)](#apidoc.element.limdu.classifiers.EnhancedClassifier)
- description and source-code
```javascript
classifiers.EnhancedClassifier = function (opts) {
	if (!opts.classifierType) {
		console.dir(opts);
		throw new Error("opts must contain classifierType");
	}

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
    	this.tfidf = new opts.TfIdfImpl
		this.featureDocumentFrequency = {};
		}
	this.bias = opts.bias;

	this.spellChecker = opts.spellChecker;
	this.tokenizer = opts.tokenizer;
	this.instanceFilterRule = opts.instanceFilter

	// this.spellChecker =  [require('wordsworth').getInstance(), require('wordsworth').getInstance()],
	// this.pastTrainingSamples = opts.pastTrainingSamples;
	// TODO: it looks like the method with creating an array at the definition
	// create an array with the same pointer for every classifier of the given class
	
	this.pastTrainingSamples = []

	this.InputSplitLabel = opts.InputSplitLabel
	this.OutputSplitLabel = opts.OutputSplitLabel
	this.TestSplitLabel = opts.TestSplitLabel
}
```
- example usage
```shell
...
var WordExtractor = function(input, features) {
	input.split(" ").forEach(function(word) {
		features[word]=1;
	});
};

// Initialize a classifier with the base classifier type and the feature extractor:
var intentClassifier = new limdu.classifiers.EnhancedClassifier({
	classifierType: TextClassifier,
	featureExtractor: WordExtractor
});

// Train and test:
intentClassifier.trainBatch([
	{input: "I want an apple", output: "apl"},
...
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork"></a>[function <span class="apidocSignatureSpan">limdu.</span>classifiers.NeuralNetwork (options)](#apidoc.element.limdu.classifiers.NeuralNetwork)
- description and source-code
```javascript
classifiers.NeuralNetwork = function (options) {
  options = options || {};
  this.learningRate = options.learningRate || 0.3;
  this.momentum = options.momentum || 0.1;
  this.hiddenSizes = options.hiddenLayers;

  this.binaryThresh = options.binaryThresh || 0.5;
}
```
- example usage
```shell
...
## Binary Classification

### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);
...
```

#### <a name="apidoc.element.limdu.classifiers.Perceptron"></a>[function <span class="apidocSignatureSpan">limdu.</span>classifiers.Perceptron (opts)](#apidoc.element.limdu.classifiers.Perceptron)
- description and source-code
```javascript
classifiers.Perceptron = function (opts) {
	if (!opts) opts = {};
	
	this.debug = opts.debug||false;
	this.default_weight = opts.default_weight||0;
	this.do_averaging = opts.do_averaging||false;
	this.do_normalization = opts.do_normalization||false;
	this.learning_rate = opts.learning_rate||0.1;
	this.retrain_count = 'retrain_count' in opts? opts.retrain_count: 1;
	
	this.weights = {};
	if (this.do_averaging) this.weights_sum = {};   // for averaging; see http://ciml.info/dl/v0_8/ciml-v0_8-ch03.pdf . But count only
 weight vectors with successful predictions (Carvalho and Cohen, 2006).
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.SvmJs"></a>[function <span class="apidocSignatureSpan">limdu.</span>classifiers.SvmJs (opts)](#apidoc.element.limdu.classifiers.SvmJs)
- description and source-code
```javascript
function SvmJs(opts) {
	this.base = new SvmJsBase();
	this.opts = opts;  // options for SvmJsBase.train
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.SvmLinear"></a>[function <span class="apidocSignatureSpan">limdu.</span>classifiers.SvmLinear (opts)](#apidoc.element.limdu.classifiers.SvmLinear)
- description and source-code
```javascript
function SvmLinear(opts) {
	this.learn_args = opts.learn_args || "";
	this.model_file_prefix = opts.model_file_prefix || null;
	this.bias = opts.bias || 1.0;
	this.multiclass = opts.multiclass || false;
	this.debug = opts.debug||false;
	this.train_command = opts.train_command || 'liblinear_train';
	this.test_command = opts.test_command || 'liblinear_test';
	this.timestamp = ""

	if (!SvmLinear.isInstalled()) {
                var msg = "Cannot find the executable 'liblinear_train'. Please download it from the LibLinear website, and put
a link to it in your path.";
                console.error(msg)
                throw new Error(msg);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.SvmPerf"></a>[function <span class="apidocSignatureSpan">limdu.</span>classifiers.SvmPerf (opts)](#apidoc.element.limdu.classifiers.SvmPerf)
- description and source-code
```javascript
function SvmPerf(opts) {
	if (!SvmPerf.isInstalled()) {
	 	var msg = "Cannot find the executable 'svm_perf_learn'. Please download it from the SvmPerf website, and put a link to it in
your path.";
	 	console.error(msg)
	 	throw new Error(msg);
	}
	this.learn_args = opts.learn_args || "";
	this.learn_args += " --b 0 ";  // we add the bias here, so we don't need SvmPerf to add it
	this.model_file_prefix = opts.model_file_prefix || null;
	this.bias = 'bias' in opts? opts.bias: 1.0;
	this.debug = opts.debug || false;
	this.ShowFeat = {}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.Winnow"></a>[function <span class="apidocSignatureSpan">limdu.</span>classifiers.Winnow (opts)](#apidoc.element.limdu.classifiers.Winnow)
- description and source-code
```javascript
function WinnowHash(opts) {
	if (!opts) opts = {}

	this.debug = opts.debug || false;
		
	// Default values are based on Carvalho and Cohen, 2006, section 4.2:	
	this.default_positive_weight = opts.default_positive_weight || 2.0;
	this.default_negative_weight = opts.default_negative_weight || 1.0;
	this.do_averaging = opts.do_averaging || false;
	this.threshold = ('threshold' in opts? opts.threshold: 1);
	this.promotion = opts.promotion || 1.5;
	this.demotion = opts.demotion || 0.5;
	this.margin = ('margin' in opts? opts.margin: 1.0);
	this.retrain_count = opts.retrain_count || 0;
	this.detailed_explanations = opts.detailed_explanations || false;
	
	this.bias = ('bias' in opts? opts.bias: 1.0);

	this.positive_weights = {};
	this.negative_weights = {};
	this.positive_weights_sum = {};   // for averaging; count only weight vectors with successful predictions (Carvalho and Cohen,
2006).
	this.negative_weights_sum = {};   // for averaging; count only weight vectors with successful predictions (Carvalho and Cohen,
2006).
}
```
- example usage
```shell
...
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
...
```

#### <a name="apidoc.element.limdu.classifiers.kNN"></a>[function <span class="apidocSignatureSpan">limdu.</span>classifiers.kNN (opts)](#apidoc.element.limdu.classifiers.kNN)
- description and source-code
```javascript
classifiers.kNN = function (opts) {
	this.k = opts.k
	this.mode = opts.mode
	this.distanceFunctionList = opts.distanceFunctionList
	this.distanceWeightening = opts.distanceWeightening
	this.labels = []
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.features.FeatureLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.</span>features.FeatureLookupTable ()](#apidoc.element.limdu.features.FeatureLookupTable)
- description and source-code
```javascript
features.FeatureLookupTable = function () {
	this.featureIndexToFeatureName = [undefined];
	this.featureNameToFeatureIndex = {undefined: 0};
}
```
- example usage
```shell
...
	binaryClassifierType: limdu.classifiers.SvmJs.bind(0, {C: 1.0})
});

// Initialize a classifier with a feature extractor and a lookup table:
var intentClassifier = new limdu.classifiers.EnhancedClassifier({
	classifierType: TextClassifier,
	featureExtractor: limdu.features.NGramsOfWords(1),  // each word ("1-gram") is a feature
	featureLookupTable: new limdu.features.FeatureLookupTable()
});

// Train and test:
intentClassifier.trainBatch([
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
...
```

#### <a name="apidoc.element.limdu.utils.PrecisionRecall"></a>[function <span class="apidocSignatureSpan">limdu.</span>utils.PrecisionRecall ()](#apidoc.element.limdu.utils.PrecisionRecall)
- description and source-code
```javascript
utils.PrecisionRecall = function () {
	this.labels = {}
	this.confusion = {} // only in single label case
	
	this.count = 0;
	this.TRUE = 0;
	this.startTime = new Date();
}
```
- example usage
```shell
...
var IntentClassifier = limdu.classifiers.EnhancedClassifier.bind(0, {
	classifierType: limdu.classifiers.multilabel.BinaryRelevance.bind(0, {
		binaryClassifierType: limdu.classifiers.Winnow.bind(0, {retrain_count: 10})
	}),
	featureExtractor: limdu.features.NGramsOfWords(1),
});

var microAverage = new limdu.utils.PrecisionRecall();
var macroAverage = new limdu.utils.PrecisionRecall();

limdu.utils.partitions.partitions(dataset, numOfFolds, function(trainSet, testSet) {
	console.log("Training on "+trainSet.length+" samples, testing on "+testSet.length+" samples");
	var classifier = new IntentClassifier();
	classifier.trainBatch(trainSet);
	limdu.utils.test(classifier, testSet, /* verbosity = */0,
...
```



# <a name="apidoc.module.limdu.EnhancedClassifier_2014"></a>[module limdu.EnhancedClassifier_2014](#apidoc.module.limdu.EnhancedClassifier_2014)

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.EnhancedClassifier_2014"></a>[function <span class="apidocSignatureSpan">limdu.</span>EnhancedClassifier_2014 (opts)](#apidoc.element.limdu.EnhancedClassifier_2014.EnhancedClassifier_2014)
- description and source-code
```javascript
EnhancedClassifier_2014 = function (opts) {
	if (!opts.classifierType) {
		console.dir(opts);
		throw new Error("opts must contain classifierType");
	}

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
    	this.tfidf = new opts.TfIdfImpl
		this.featureDocumentFrequency = {};
		}
	this.bias = opts.bias;

	this.spellChecker = opts.spellChecker;
	this.tokenizer = opts.tokenizer;
	this.instanceFilterRule = opts.instanceFilter

	// this.spellChecker =  [require('wordsworth').getInstance(), require('wordsworth').getInstance()],
	// this.pastTrainingSamples = opts.pastTrainingSamples;
	// TODO: it looks like the method with creating an array at the definition
	// create an array with the same pointer for every classifier of the given class
	
	this.pastTrainingSamples = []

	this.InputSplitLabel = opts.InputSplitLabel
	this.OutputSplitLabel = opts.OutputSplitLabel
	this.TestSplitLabel = opts.TestSplitLabel
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.EnhancedClassifier_2014.prototype"></a>[module limdu.EnhancedClassifier_2014.prototype](#apidoc.module.limdu.EnhancedClassifier_2014.prototype)

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.backClassify"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>backClassify (theClass)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.backClassify)
- description and source-code
```javascript
backClassify = function (theClass) {
		if (!this.pastTrainingSamples)
			throw new Error("No pastTrainingSamples array - can't backClassify");

		if (!(theClass instanceof Array))
			theClass = [theClass];
		var samples = [];
		this.pastTrainingSamples.forEach(function(datum) {
			if (_(datum.output).isEqual(theClass))
				samples.push(datum.input);
		});
		return samples;
	}
```
- example usage
```shell
...
intentClassifier.trainBatch([
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I really want an apple", output: "apl"},
	{input: "I want a banana very much", output: "bnn"},
	]);

console.dir(intentClassifier.backClassify("apl"));  // [ 'I want an apple', 'I really want an apple' ]
'''

## SVM wrappers

The native svm.js implementation takes a lot of time to train -  quadratic in the number of training samples.
There are two common packages that can be trained in time linear in the number of training samples. They are:
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>classify (sample, explain, continuous_output, original, classifier_compare)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.classify)
- description and source-code
```javascript
classify = function (sample, explain, continuous_output, original, classifier_compare) {
		var initial = sample
		sample = this.normalizedSample(sample)

		if (this.instanceFilter(sample))
			{	if (explain>0)
				return {
					classes: [],
					scores: {},
					explanation: {}
					// bonus: bonus
				};
			else
				return []
			}		
		
		if (!this.inputSplitter) {
			var classesWithExplanation = this.classifyPart(sample, explain, continuous_output);
			var classes = (explain>0? classesWithExplanation.classes: classesWithExplanation);
			var scores =  (continuous_output? classesWithExplanation.scores: null)
			var explanations = (explain>0? classesWithExplanation.explanation: null);
		} else {
			var parts = this.inputSplitter(sample);
			// var accumulatedClasses = {};
			var accumulatedClasses = [];
			var explanations = [];
			parts.forEach(function(part) {
				if (part.length==0) return;
				var classesWithExplanation = this.classifyPart(part, explain, continuous_output);
				var classes = (explain>0? classesWithExplanation.classes: classesWithExplanation);
				// for (var i in classes)
				// 	accumulatedClasses[classes[i]]=true;
				accumulatedClasses.push(classes)
				if (explain>0) {
					// explanations.push(part);
					explanations.push(classesWithExplanation.explanation);
				}
			}, this);
    		classes = []
    		if (accumulatedClasses[0])
    		{
			if (accumulatedClasses[0][0] instanceof Array)
				_(accumulatedClasses[0].length).times(function(n){
					classes.push(_.flatten(_.pluck(accumulatedClasses,n)))
				 });
			else
			{
				classes = _.flatten(accumulatedClasses)
			}
			}
		}

		if (this.labelLookupTable) {
			if (Array.isArray(classes)) {
				classes = classes.map(function(label) {
						if (_.isArray(label))
							label[0] = this.labelLookupTable.numberToFeature(label[0]);
						else
							label = this.labelLookupTable.numberToFeature(label);
						return label;
					}, this);
			} else {
				classes = this.labelLookupTable.numberToFeature(classes);
			}
		}

		if ((typeof this.OutputSplitLabel === 'function')) {

			// classes = this.OutputSplitLabel(classes, this.Observable, sample, explanations)
			// var classes = []
			// if (_.isArray(explanations))
			// var bonus = []
		
			if ((explain>0) && (this.inputSplitter))
				{ nclasses = []
				_(explanations.length).times(function(n){
					var clas = this.OutputSplitLabel(classes, this, parts[n], explanations[n], original, classifier_compare, initial)
					nclasses = nclasses.concat(clas)
				}, this)
				classes = nclasses
				}
			else
				{
				var classes = this.OutputSplitLabel(classes, this, sample, explanations, original, classifier_compare, initial)
				}
			}

		if (explain>0)
			return {
				classes: classes,
				scores: scores,
				explanation: explanations
				// bonus: bonus
			};
		else
			return classes;
	}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.classifyPart"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>classifyPart (sample, explain, continuous_output)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.classifyPart)
- description and source-code
```javascript
classifyPart = function (sample, explain, continuous_output) {
		
		var samplecorrected = this.correctFeatureSpelling(sample);
		var features = this.sampleToFeatures(samplecorrected, this.featureExtractors);
		this.editFeatureValues(features, /*remove_unknown_features=*/true);
		var array = this.featuresToArray(features);
		var classification = this.classifier.classify(array, explain, continuous_output);
		
		// if (this.spellChecker && classification.explanation) {
			// if (Array.isArray(classification.explanation))
				// classification.explanation.unshift({SpellCorrectedFeatures: JSON.stringify(features)});
			// else
				// classification.explanation['SpellCorrectedFeatures']=JSON.stringify(features);
		// }
		return classification;
	}
```
- example usage
```shell
...
					// bonus: bonus
				};
			else
				return []
			}		
		
		if (!this.inputSplitter) {
			var classesWithExplanation = this.classifyPart(sample, explain, continuous_output);
			var classes = (explain>0? classesWithExplanation.classes: classesWithExplanation);
			var scores =  (continuous_output? classesWithExplanation.scores: null)
			var explanations = (explain>0? classesWithExplanation.explanation: null);
		} else {
			var parts = this.inputSplitter(sample);
			// var accumulatedClasses = {};
			var accumulatedClasses = [];
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.correctFeatureSpelling"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>correctFeatureSpelling (sample)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.correctFeatureSpelling)
- description and source-code
```javascript
correctFeatureSpelling = function (sample) {
		if (this.spellChecker) {
			var features = this.tokenizer.tokenize(sample);
			for (var index in features) {
				var feature = features[index]
				if (!isNaN(parseInt(feature)))  // don't spell-correct numeric features
					{
					continue
					}
				
				if (!(this.spellChecker[1].exists(feature)))
					{
						if (this.spellChecker[1].suggest(feature).length != 0)
							{
							features[index] = this.spellChecker[1].suggest(feature)[0]
							}
						else
							{
								if (!(this.spellChecker[0].exists(feature)))
									{
										if (this.spellChecker[0].suggest(feature).length != 0)
											{
											features[index] = this.spellChecker[0].suggest(feature)[0]
											
											}
									}
							}
					}
			}
		sample = features.join(" ")
		}
		return sample
	}
```
- example usage
```shell
...
	/**
	 * internal function - classify a single segment of the input (used mainly when there is an inputSplitter)
	 * @param sample a document.
	 * @return an array whose VALUES are classes.
	 */
	classifyPart: function(sample, explain, continuous_output) {
		
		var samplecorrected = this.correctFeatureSpelling(sample);
		var features = this.sampleToFeatures(samplecorrected, this.featureExtractors);
		this.editFeatureValues(features, /*remove_unknown_features=*/true);
		var array = this.featuresToArray(features);
		var classification = this.classifier.classify(array, explain, continuous_output);
		
		// if (this.spellChecker && classification.explanation) {
			// if (Array.isArray(classification.explanation))
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.countFeatures"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>countFeatures (features)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.countFeatures)
- description and source-code
```javascript
countFeatures = function (features) {
		if (this.featureDocumentFrequency) {
			// this.tfidf.addDocument(datum.input);
			for (var feature in features)
				this.featureDocumentFrequency[feature] = (this.featureDocumentFrequency[feature] || 0)+1;
			this.documentCount = (this.documentCount||0)+1;
		}
	}
```
- example usage
```shell
...
	 * @param sample a document.
	 * @param classes an array whose VALUES are classes.
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
	},
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.editFeatureValues"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>editFeatureValues (features, remove_unknown_features)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.editFeatureValues)
- description and source-code
```javascript
editFeatureValues = function (features, remove_unknown_features) {

		if (this.multiplyFeaturesByIDF) {
			for (var feature in features) {
				var IDF = this.tfidf.idf(feature)
				if (IDF != Infinity)
					features[feature] *= IDF
				else
					delete features[feature]
			}

			if (this.bias && !features.bias)
			features.bias = this.bias;

		}
		// if (remove_unknown_features && this.minFeatureDocumentFrequency>0)
			// for (var feature in features)
				// if ((this.featureDocumentFrequency[feature]||0)<this.minFeatureDocumentFrequency)
					// delete features[feature];
		
	}
```
- example usage
```shell
...
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
	},

	/**
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.featuresToArray"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>featuresToArray (features)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.featuresToArray)
- description and source-code
```javascript
featuresToArray = function (features) {
		var array = features;
		if (this.featureLookupTable) {
			array = this.featureLookupTable.hashToArray(features);
		}
		return array;
	}
```
- example usage
```shell
...
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
	},

	/**
	 * Batch training:
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>fromJSON (json)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
		}
		if (this.spellChecker) this.spellChecker = json.spellChecker;
		if (this.pastTrainingSamples) this.pastTrainingSamples = json.pastTrainingSamples;
		this.featureDocumentFrequency = json.featureDocumentFrequency;
		this.documentCount = json.documentCount;
		/* Note: the feature extractors are functions - they should be created at initialization - they are not deserializable! */
	}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.getAllClasses"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>getAllClasses ()](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.getAllClasses)
- description and source-code
```javascript
getAllClasses = function () {  // relevant for multilabel classifiers
		return this.classifier.getAllClasses();
	}
```
- example usage
```shell
...
		if (this.pastTrainingSamples) this.pastTrainingSamples = json.pastTrainingSamples;
		this.featureDocumentFrequency = json.featureDocumentFrequency;
		this.documentCount = json.documentCount;
		/* Note: the feature extractors are functions - they should be created at initialization - they are not deserializable! */
	},

	getAllClasses: function() {  // relevant for multilabel classifiers
		return this.classifier.getAllClasses();
	},
}  // end of EnhancedClassifier prototype


var stringifyClass = function (aClass) {
	return (_(aClass).isString()? aClass: JSON.stringify(aClass));
}
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.instanceFilter"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>instanceFilter (data)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.instanceFilter)
- description and source-code
```javascript
instanceFilter = function (data) {
		if (this.instanceFilterRule)
			return this.instanceFilterRule(data)
	}
```
- example usage
```shell
...
				if (pastTrainingSamples && dataset!=pastTrainingSamples)
					pastTrainingSamples.push(datum);
				datum = _(datum).clone();

				datum.input = this.normalizedSample(datum.input);

				/*true - this instance is filtered as not useful*/
				if (this.instanceFilter(datum) == true)
					return null

				this.trainSpellChecker(datum.input);

				var features = this.sampleToFeatures(datum.input, this.featureExtractors);
				
				if (this.tfidf)
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.normalizedSample"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>normalizedSample (sample)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.normalizedSample)
- description and source-code
```javascript
normalizedSample = function (sample) {
		if (!(_.isArray(sample)))
		{
			if (this.normalizers) {
				try {
					for (var i in this.normalizers) {					
						sample = this.normalizers[i](sample);
					}
				} catch (err) {
					console.log(err)
					throw new Error("Cannot normalize '"+sample+"': "+JSON.stringify(err));
				}
			}
		}

		return sample;
	}
```
- example usage
```shell
...
	 * Online training:
	 * Tell the classifier that the given sample belongs to the given classes.
	 * @param sample a document.
	 * @param classes an array whose VALUES are classes.
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.outputToFormat"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>outputToFormat (data)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.outputToFormat)
- description and source-code
```javascript
outputToFormat = function (data) {
		dataset = util.clonedataset(data)
		dataset = dataset.map(function(datum) {
		var normalizedLabels = multilabelutils.normalizeOutputLabels(datum.output);
		return {
			input: datum.input,
			output: this.TestSplitLabel(normalizedLabels)
		}
		}, this);
		return dataset
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.retrain"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>retrain ()](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.retrain)
- description and source-code
```javascript
retrain = function () {
		if (!this.pastTrainingSamples)
			throw new Error("No pastTrainingSamples array - can't retrain");
		
		this.trainBatch(this.pastTrainingSamples);
	}
```
- example usage
```shell
...
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
var intentClassifierString = serialize.toString(intentClassifier, newClassifierFunction);

// Save the string to a file, and send it to a remote server.
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.sampleToFeatures"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>sampleToFeatures (sample, featureExtractor)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.sampleToFeatures)
- description and source-code
```javascript
sampleToFeatures = function (sample, featureExtractor) {
		var features = sample;
		if (featureExtractor) {
			try {
				features = {};
				featureExtractor(sample, features);
			} catch (err) {
				throw new Error("Cannot extract features from '"+sample+"': "+JSON.stringify(err));
			}
		}

		return features;
	}
```
- example usage
```shell
...
	 * Tell the classifier that the given sample belongs to the given classes.
	 * @param sample a document.
	 * @param classes an array whose VALUES are classes.
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.setFeatureExtractor"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>setFeatureExtractor (featureExtractor)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.setFeatureExtractor)
- description and source-code
```javascript
setFeatureExtractor = function (featureExtractor) {
		this.featureExtractors = ftrs.normalize(featureExtractor);
	}
```
- example usage
```shell
...
		throw new Error("opts must contain classifierType");
	}

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.setFeatureExtractorForClassification"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>setFeatureExtractorForClassification (featureExtractorForClassification)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.setFeatureExtractorForClassification)
- description and source-code
```javascript
setFeatureExtractorForClassification = function (featureExtractorForClassification) {
		if (featureExtractorForClassification) {
			if (Array.isArray(featureExtractorForClassification)) {
				featureExtractorForClassification.unshift(this.featureExtractors);
			} else {
				featureExtractorForClassification = [this.featureExtractors, featureExtractorForClassification];
			}
			this.featureExtractorsForClassification = new ftrs.CollectionOfExtractors(featureExtractorForClassification);
		}
	}
```
- example usage
```shell
...
	}

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.setFeatureLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.setFeatureLookupTable)
- description and source-code
```javascript
setFeatureLookupTable = function (featureLookupTable) {
		if (featureLookupTable) {
			this.featureLookupTable = featureLookupTable;
			if (this.classifier.setFeatureLookupTable)
				this.classifier.setFeatureLookupTable(featureLookupTable);  // for generating clearer explanations only
		}
	}
```
- example usage
```shell
...

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
	this.tfidf = new opts.TfIdfImpl
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.setLabelLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>setLabelLookupTable (labelLookupTable)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.setLabelLookupTable)
- description and source-code
```javascript
setLabelLookupTable = function (labelLookupTable) {
		if (labelLookupTable) {
			this.labelLookupTable = labelLookupTable;
			if (this.classifier.setLabelLookupTable)
				this.classifier.setLabelLookupTable(labelLookupTable);  // for generating clearer explanations only
		}
	}
```
- example usage
```shell
...
	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
    	this.tfidf = new opts.TfIdfImpl
		this.featureDocumentFrequency = {};
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.setNormalizer"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>setNormalizer (normalizer)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.setNormalizer)
- description and source-code
```javascript
setNormalizer = function (normalizer) {
		if (normalizer)
			this.normalizers = (Array.isArray(normalizer)? normalizer: [normalizer]);
	}
```
- example usage
```shell
...
		console.dir(opts);
		throw new Error("opts must contain classifierType");
	}

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>toJSON (callback)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.toJSON)
- description and source-code
```javascript
toJSON = function (callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
		var featureLookupTable = this.featureLookupTable;
		var pastTrainingSamples = this.pastTrainingSamples;

			if (this.spellChecker) {
				// var seeds = fs.readFileSync('./node_modules/wordsworth/data/seed.txt')
				// var trainings = fs.readFileSync('./node_modules/wordsworth/data/training.txt')
				var seeds = []
				var trainings = []
				this.spellChecker[0].initializeSync(seeds.toString().split("\r\n"), trainings.toString().split("\r\n"))
				}

			dataset = dataset.map(function(datum) {

				if (typeof this.InputSplitLabel === 'function') {
					datum.output = (this.InputSplitLabel(multilabelutils.normalizeOutputLabels(datum.output)))	
				}
				else
				{
					datum.output = normalizeClasses(datum.output, this.labelLookupTable);
				}

				if (pastTrainingSamples && dataset!=pastTrainingSamples)
					pastTrainingSamples.push(datum);
				datum = _(datum).clone();

				datum.input = this.normalizedSample(datum.input);

				<span class="apidocCodeCommentSpan">/*true - this instance is filtered as not useful*/
</span>				if (this.instanceFilter(datum) == true)
					return null

				this.trainSpellChecker(datum.input);

				var features = this.sampleToFeatures(datum.input, this.featureExtractors);
				
				if (this.tfidf)
					this.tfidf.addDocument(features);
				// this.trainSpellChecker(features);
				if (featureLookupTable)
					featureLookupTable.addFeatures(features);

				datum.input = features;
				return datum;
			}, this);

			dataset = _.compact(dataset)

		dataset.forEach(function(datum) {
			// run on single sentence
			this.editFeatureValues(datum.input, /*remove_unknown_features=*/false);
			if (featureLookupTable)
				datum.input = featureLookupTable.hashToArray(datum.input);
		}, this);

		this.classifier.trainBatch(dataset);
	}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>trainOnline (sample, classes)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
	}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2014.prototype.trainSpellChecker"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2014.prototype.</span>trainSpellChecker (features)](#apidoc.element.limdu.EnhancedClassifier_2014.prototype.trainSpellChecker)
- description and source-code
```javascript
trainSpellChecker = function (features) {
		if (this.spellChecker) {
			var tokens = this.tokenizer.tokenize(features);
			_.each(tokens, function(word, key, list){
				this.spellChecker[1].understand(word); // Adds the given word to the index of the spell-checker.
				this.spellChecker[1].train(word);
			}, this)
		}
	}
```
- example usage
```shell
...
	 * @param classes an array whose VALUES are classes.
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
	},
...
```



# <a name="apidoc.module.limdu.EnhancedClassifier_2015"></a>[module limdu.EnhancedClassifier_2015](#apidoc.module.limdu.EnhancedClassifier_2015)

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.EnhancedClassifier_2015"></a>[function <span class="apidocSignatureSpan">limdu.</span>EnhancedClassifier_2015 (opts)](#apidoc.element.limdu.EnhancedClassifier_2015.EnhancedClassifier_2015)
- description and source-code
```javascript
EnhancedClassifier_2015 = function (opts) {
	if (!opts.classifierType) {
		console.dir(opts);
		throw new Error("opts must contain classifierType");
	}

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	// this.setFeatureLookupTable(opts.featureLookupTable);
	this.setFeatureLookupTable(new ftrs.FeatureLookupTable());

	this.setLabelLookupTable(opts.labelLookupTable);
	this.setInstanceFilter(opts.instanceFilter);

	this.setFeatureExpansion(opts.featureExpansion);
	this.featureExpansionScale = opts.featureExpansionScale;
	this.featureExpansionPhrase = opts.featureExpansionPhrase;
	this.featureFine = opts.featureFine;

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
    	this.tfidf = new opts.TfIdfImpl
		this.featureDocumentFrequency = {};
		}
	this.bias = opts.bias;

	this.spellChecker = opts.spellChecker;
	this.tokenizer = opts.tokenizer;

	// this.spellChecker =  [require('wordsworth').getInstance(), require('wordsworth').getInstance()],
	// this.pastTrainingSamples = opts.pastTrainingSamples;
	// TODO: it looks like the method with creating an array at the definition
	// create an array with the same pointer for every classifier of the given class
	
	this.pastTrainingSamples = []

	this.preProcessor = opts.preProcessor
	this.postProcessor = opts.postProcessor
	// this.TestSplitLabel = opts.TestSplitLabel
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.EnhancedClassifier_2015.prototype"></a>[module limdu.EnhancedClassifier_2015.prototype](#apidoc.module.limdu.EnhancedClassifier_2015.prototype)

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.applyFeatureExpansion"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>applyFeatureExpansion ()](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.applyFeatureExpansion)
- description and source-code
```javascript
applyFeatureExpansion = function (){
	 	this.featureExpansioned = this.featureExpansion(this.featureLookupTable['featureIndexToFeatureName'], this.featureExpansionScale
, this.featureExpansionPhrase)
	}
```
- example usage
```shell
...
	},
	
	setLabelLookupTable: function(labelLookupTable) {
		if (labelLookupTable) {
			this.labelLookupTable = labelLookupTable;
			if (this.classifier.setLabelLookupTable)
				this.classifier.setLabelLookupTable(labelLookupTable);  // for generating clearer explanations only
			this.applyFeatureExpansion();
		}
	},

	applyFeatureExpansion: function(){
	 	this.featureExpansioned = this.featureExpansion(this.featureLookupTable['featureIndexToFeatureName'], this.featureExpansionScale
, this.featureExpansionPhrase)
	},
	// private function: use this.normalizers to normalize the given sample:
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.backClassify"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>backClassify (theClass)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.backClassify)
- description and source-code
```javascript
backClassify = function (theClass) {
		if (!this.pastTrainingSamples)
			throw new Error("No pastTrainingSamples array - can't backClassify");

		if (!(theClass instanceof Array))
			theClass = [theClass];
		var samples = [];
		this.pastTrainingSamples.forEach(function(datum) {
			if (_(datum.output).isEqual(theClass))
				samples.push(datum.input);
		});
		return samples;
	}
```
- example usage
```shell
...
intentClassifier.trainBatch([
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I really want an apple", output: "apl"},
	{input: "I want a banana very much", output: "bnn"},
	]);

console.dir(intentClassifier.backClassify("apl"));  // [ 'I want an apple', 'I really want an apple' ]
'''

## SVM wrappers

The native svm.js implementation takes a lot of time to train -  quadratic in the number of training samples.
There are two common packages that can be trained in time linear in the number of training samples. They are:
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>classify (sample, explain)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.classify)
- description and source-code
```javascript
classify = function (sample, explain) {
		var initial = sample

		if (_.isObject(sample))
			sample.text = this.normalizedSample(sample.text)
		else
			sample = this.normalizedSample(sample)

		if (!this.inputSplitter) {

			if (typeof this.preProcessor === 'function')
				sample = this.preProcessor(sample)

			var classesWithExplanation = this.classifyPart(sample, explain);
            //console.log("classesWithExplanation="+JSON.stringify(classesWithExplanation));
			var classes = (explain>0? classesWithExplanation.classes: classesWithExplanation);
            //console.log("classes="+JSON.stringify(classes));
			var scores =  classesWithExplanation.scores
            //console.log("scores="+JSON.stringify(scores));
			var explanations = (explain>0? classesWithExplanation.explanation: null);
            //console.log("explanations="+JSON.stringify(explanations));
		} else {
			var parts = this.inputSplitter(sample);
			var accumulatedClasses = [];
			var explanations = [];
			parts.forEach(function(part) {
				if (part.length==0) return;
				var part_filtered = part
				if (typeof this.preProcessor === 'function')
					part_filtered = this.preProcessor(part)
				var classesWithExplanation = this.classifyPart(part_filtered, explain);
				var classes = (explain>0? classesWithExplanation.classes: classesWithExplanation);
				if (typeof this.postProcessor === 'function')
					classes = this.postProcessor(part, classes)
				accumulatedClasses.push(classes)
				if (explain>0) {
					explanations.push(classesWithExplanation.explanation);
				}
			}, this);
			classes = _.flatten(accumulatedClasses)
		}

		if (this.labelLookupTable) {
			if (Array.isArray(classes)) {
				classes = classes.map(function(label) {
						if (_.isArray(label))
							label[0] = this.labelLookupTable.numberToFeature(label[0]);
						else
							label = this.labelLookupTable.numberToFeature(label);
						return label;
					}, this);
			} else {
				classes = this.labelLookupTable.numberToFeature(classes);
			}
		}

		if (explain>0)
			return {
				classes: classes,
				scores: scores,
				// expansioned: classesWithExplanation.expansioned,
				// features: classesWithExplanation.features,
				// explanation: explanations
			};
		else
			return classes;
	}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.classifyAsync"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>classifyAsync (sample, explain, callback_global)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.classifyAsync)
- description and source-code
```javascript
classifyAsync = function (sample, explain, callback_global) {
		var classes = []

		async.series([
   			(function(callback){
       		
        		if(!this.inputSplitter) {
        			if (typeof this.preProcessor === 'function')
						sample = this.preProcessor(sample)

					this.classifyPartAsync(sample, explain, function(error, classesWithExplanation){
						classes = (explain>0? classesWithExplanation.classes: classesWithExplanation);
						var scores =  classesWithExplanation.scores
						// var scores =  (continuous_output? classesWithExplanation.scores: null)
						var explanations = (explain>0? classesWithExplanation.explanation: null);
						callback(null, null);
					});					

        		} else {
          			callback(null, null);
        		}
   			}).bind(this),
    		(function(callback){

    			if (typeof this.inputSplitter === 'function')
    			{

	          		var parts = this.inputSplitter(sample);
					var accumulatedClasses = [];
					var explanations = [];
			
					async.eachSeries(parts, (function(part, callback1){
						if (part.length==0) return;

						var part_filtered = part

						if (typeof this.preProcessor === 'function')
							part_filtered = this.preProcessor(part)
					
						this.classifyPartAsync(part_filtered, explain, (function(error, classesWithExplanation){

							classes = (explain>0? classesWithExplanation.classes: classesWithExplanation);
				
							if (typeof this.postProcessor === 'function')
								classes = this.postProcessor(part, classes)

							accumulatedClasses.push(classes)
							if (explain>0)
								explanations.push(classesWithExplanation.explanation);

							callback1()
						}).bind(this))

				    }).bind(this), function(err){
	   					classes = _.flatten(accumulatedClasses)
	             	   	callback(null, null)
	                })
        		} else {
          			callback(null, null);
        		}
    		}).bind(this)
		], function () {

			if (this.labelLookupTable) {
				if (Array.isArray(classes)) {
					classes = classes.map(function(label) {
						if (_.isArray(label))
							label[0] = this.labelLookupTable.numberToFeature(label[0]);
						else
							label = this.labelLookupTable.numberToFeature(label);
						return label;
					}, this);
				} else {
					classes = this.labelLookupTable.numberToFeature(classes);
				}
			}
			
    		callback_global(null, classes)
		})
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.classifyBatch"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>classifyBatch (testSet)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.classifyBatch)
- description and source-code
```javascript
classifyBatch = function (testSet)
{
    _.each(testSet, function(value, key, list){
        testSet[key]["input"] = this.normalizedSample(testSet[key]["input"])
        var features = this.sampleToFeatures(testSet[key]["input"], this.featureExtractors, this.stopwords);
        this.editFeatureValues(features, /*remove_unknown_features=*/false);
        var array = this.featuresToArray(features);
        testSet[key]["input"] = array
    }, this)
    return this.classifier.classifyBatch(testSet);
}
```
- example usage
```shell
...
            _.each(testSet, function(value, key, list){
                testSet[key]["input"] = this.normalizedSample(testSet[key]["input"])
                var features = this.sampleToFeatures(testSet[key]["input"], this.featureExtractors, this.stopwords);
                this.editFeatureValues(features, /*remove_unknown_features=*/false);
                var array = this.featuresToArray(features);
                testSet[key]["input"] = array
            }, this)
            return this.classifier.classifyBatch(testSet);
        },
	
	classifyPartAsync: function(sample, explain, callback) {
		this.sampleToFeaturesAsync(sample, this.featureExtractors, (function(err, results){
			this.editFeatureValues(features, /*remove_unknown_features=*/false);
			var array = this.featuresToArray(features);
			var classification = this.classifier.classify(array, explain);
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.classifyPart"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>classifyPart (sample, explain, continuous_output)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.classifyPart)
- description and source-code
```javascript
classifyPart = function (sample, explain, continuous_output) {
		var features = this.sampleToFeatures(sample, this.featureExtractors);
        //console.log("features="+JSON.stringify(features));
		this.editFeatureValues(features, /*remove_unknown_features=*/false);  // change the value of each feature according to the TF/
IDF method
        //console.log("features="+JSON.stringify(features));
		var array = this.featuresToArray(features);  // convert textual features to numeric features using a lookup table
        //console.log("array="+JSON.stringify(array));
		var classification = this.classifier.classify(array, explain, continuous_output);
        //console.log("classification="+JSON.stringify(classification));
		classification['features'] = features
		return classification;
	}
```
- example usage
```shell
...
					// bonus: bonus
				};
			else
				return []
			}		
		
		if (!this.inputSplitter) {
			var classesWithExplanation = this.classifyPart(sample, explain, continuous_output);
			var classes = (explain>0? classesWithExplanation.classes: classesWithExplanation);
			var scores =  (continuous_output? classesWithExplanation.scores: null)
			var explanations = (explain>0? classesWithExplanation.explanation: null);
		} else {
			var parts = this.inputSplitter(sample);
			// var accumulatedClasses = {};
			var accumulatedClasses = [];
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.classifyPartAsync"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>classifyPartAsync (sample, explain, callback)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.classifyPartAsync)
- description and source-code
```javascript
classifyPartAsync = function (sample, explain, callback) {
		this.sampleToFeaturesAsync(sample, this.featureExtractors, (function(err, results){
			this.editFeatureValues(features, /*remove_unknown_features=*/false);
			var array = this.featuresToArray(features);
			var classification = this.classifier.classify(array, explain);
			classification['features'] = features
			callback(null, classification)
		}).bind(this))
	}
```
- example usage
```shell
...
		async.series([
   			(function(callback){
       		
        		if(!this.inputSplitter) {
        			if (typeof this.preProcessor === 'function')
						sample = this.preProcessor(sample)

					this.classifyPartAsync(sample, explain, function(error, classesWithExplanation){
						classes = (explain>0? classesWithExplanation.classes: classesWithExplanation);
						var scores =  classesWithExplanation.scores
						// var scores =  (continuous_output? classesWithExplanation.scores: null)
						var explanations = (explain>0? classesWithExplanation.explanation: null);
						callback(null, null);
					});
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.correctFeatureSpelling"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>correctFeatureSpelling (sample)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.correctFeatureSpelling)
- description and source-code
```javascript
correctFeatureSpelling = function (sample) {
		if (this.spellChecker) {
			var features = this.tokenizer.tokenize(sample);
			for (var index in features) {
				var feature = features[index]
				if (!isNaN(parseInt(feature)))  // don't spell-correct numeric features
					{
					continue
					}
				
				if (!(this.spellChecker[1].exists(feature)))
					{
						if (this.spellChecker[1].suggest(feature).length != 0)
							{
							features[index] = this.spellChecker[1].suggest(feature)[0]
							}
						else
							{
								if (!(this.spellChecker[0].exists(feature)))
									{
										if (this.spellChecker[0].suggest(feature).length != 0)
											{
											features[index] = this.spellChecker[0].suggest(feature)[0]
											
											}
									}
							}
					}
			}
		sample = features.join(" ")
		}
		return sample
	}
```
- example usage
```shell
...
	/**
	 * internal function - classify a single segment of the input (used mainly when there is an inputSplitter)
	 * @param sample a document.
	 * @return an array whose VALUES are classes.
	 */
	classifyPart: function(sample, explain, continuous_output) {
		
		var samplecorrected = this.correctFeatureSpelling(sample);
		var features = this.sampleToFeatures(samplecorrected, this.featureExtractors);
		this.editFeatureValues(features, /*remove_unknown_features=*/true);
		var array = this.featuresToArray(features);
		var classification = this.classifier.classify(array, explain, continuous_output);
		
		// if (this.spellChecker && classification.explanation) {
			// if (Array.isArray(classification.explanation))
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.countFeatures"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>countFeatures (features)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.countFeatures)
- description and source-code
```javascript
countFeatures = function (features) {
		if (this.featureDocumentFrequency) {
			// this.tfidf.addDocument(datum.input);
			for (var feature in features)
				this.featureDocumentFrequency[feature] = (this.featureDocumentFrequency[feature] || 0)+1;
			this.documentCount = (this.documentCount||0)+1;
		}
	}
```
- example usage
```shell
...
	 * @param sample a document.
	 * @param classes an array whose VALUES are classes.
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
	},
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.editFeatureValues"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>editFeatureValues (features, remove_unknown_features)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.editFeatureValues)
- description and source-code
```javascript
editFeatureValues = function (features, remove_unknown_features) {

		if (this.multiplyFeaturesByIDF) {
			for (var feature in features) {

				// Skip word2vec features
				if (typeof feature.match(/w2v/g) == "undefined" || feature.match(/w2v/g) == null)
					continue

				var IDF = this.tfidf.idf(feature)

				if (IDF != Infinity)
					features[feature] *= IDF
				else
					{
					console.error("Infinity "+feature)
					delete features[feature]
					}
			}

			if (this.bias && !features.bias)
			features.bias = this.bias;

		}
		// if (remove_unknown_features && this.minFeatureDocumentFrequency>0)
			// for (var feature in features)
				// if ((this.featureDocumentFrequency[feature]||0)<this.minFeatureDocumentFrequency)
					// delete features[feature];
		
	}
```
- example usage
```shell
...
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
	},

	/**
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.featuresToArray"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>featuresToArray (features)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.featuresToArray)
- description and source-code
```javascript
featuresToArray = function (features) {
		var array = features;
		if (this.featureLookupTable) {
			array = this.featureLookupTable.hashToArray(features);
		}
		return array;
	}
```
- example usage
```shell
...
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
	},

	/**
	 * Batch training:
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>fromJSON (json)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
		}
		if (this.spellChecker) this.spellChecker = json.spellChecker;
		if (this.pastTrainingSamples) this.pastTrainingSamples = json.pastTrainingSamples;
		this.featureDocumentFrequency = json.featureDocumentFrequency;
		this.documentCount = json.documentCount;
		/* Note: the feature extractors are functions - they should be created at initialization - they are not deserializable! */
	}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.getAllClasses"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>getAllClasses ()](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.getAllClasses)
- description and source-code
```javascript
getAllClasses = function () {  // relevant for multilabel classifiers
		return this.classifier.getAllClasses();
	}
```
- example usage
```shell
...
		if (this.pastTrainingSamples) this.pastTrainingSamples = json.pastTrainingSamples;
		this.featureDocumentFrequency = json.featureDocumentFrequency;
		this.documentCount = json.documentCount;
		/* Note: the feature extractors are functions - they should be created at initialization - they are not deserializable! */
	},

	getAllClasses: function() {  // relevant for multilabel classifiers
		return this.classifier.getAllClasses();
	},
}  // end of EnhancedClassifier prototype


var stringifyClass = function (aClass) {
	return (_(aClass).isString()? aClass: JSON.stringify(aClass));
}
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.instanceFilterRun"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>instanceFilterRun (data)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.instanceFilterRun)
- description and source-code
```javascript
instanceFilterRun = function (data) {
		if (this.instanceFilter)
			return this.instanceFilter(data)
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.normalizedSample"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>normalizedSample (sample)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.normalizedSample)
- description and source-code
```javascript
normalizedSample = function (sample) {
		if (!(_.isArray(sample)))
		{
			if (this.normalizers) {
				try {
					for (var i in this.normalizers) {					
						sample = this.normalizers[i](sample);
					}
				} catch (err) {
					console.log(err)
					throw new Error("Cannot normalize '"+sample+"': "+JSON.stringify(err));
				}
			}
		}

		return sample;
	}
```
- example usage
```shell
...
	 * Online training:
	 * Tell the classifier that the given sample belongs to the given classes.
	 * @param sample a document.
	 * @param classes an array whose VALUES are classes.
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.retrain"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>retrain ()](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.retrain)
- description and source-code
```javascript
retrain = function () {
		if (!this.pastTrainingSamples)
			throw new Error("No pastTrainingSamples array - can't retrain");
		
		this.trainBatch(this.pastTrainingSamples);
	}
```
- example usage
```shell
...
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
var intentClassifierString = serialize.toString(intentClassifier, newClassifierFunction);

// Save the string to a file, and send it to a remote server.
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.sampleToFeatures"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>sampleToFeatures (sample, featureExtractor)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.sampleToFeatures)
- description and source-code
```javascript
sampleToFeatures = function (sample, featureExtractor) {
		var features = sample;
		if (featureExtractor) {
			try {
				features = {};
				featureExtractor(sample, features);
			} catch (err) {
				console.log(err)
				throw new Error("Cannot extract features from '"+sample+"': "+JSON.stringify(err));
			}
		}

		return features;
	}
```
- example usage
```shell
...
	 * Tell the classifier that the given sample belongs to the given classes.
	 * @param sample a document.
	 * @param classes an array whose VALUES are classes.
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.sampleToFeaturesAsync"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>sampleToFeaturesAsync (sample, featureExtractor, callback)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.sampleToFeaturesAsync)
- description and source-code
```javascript
sampleToFeaturesAsync = function (sample, featureExtractor, callback) {
		// features = {}
		// 	async.eachSeries(featureExtractor, function(FE, callback1){
//               FE(sample, features, function(err, results){
//                   callback1()
//               })
//           }, function(err){
//               callback(null, features)
//               })
	
		features = {}
		featureExtractor(sample, features, function(err, results){
			callback(null, features)
		})
  }
```
- example usage
```shell
...
				datum.input = this.normalizedSample(datum.input);

			if (typeof this.preProcessor === 'function')
				datum = this.preProcessor(datum)

			if (!_.isUndefined(datum))
			{
				this.sampleToFeaturesAsync(datum.input, this.featureExtractors, (function(err, features){
			
					// this.omitStopWords(features, this.stopwords)

					if (this.tfidf)
						this.tfidf.addDocument(features)
					
					if (featureLookupTable)
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.setFeatureExpansion"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>setFeatureExpansion (featureExpansion)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.setFeatureExpansion)
- description and source-code
```javascript
setFeatureExpansion = function (featureExpansion) {
		this.featureExpansion = featureExpansion
	}
```
- example usage
```shell
...
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	// this.setFeatureLookupTable(opts.featureLookupTable);
	this.setFeatureLookupTable(new ftrs.FeatureLookupTable());

	this.setLabelLookupTable(opts.labelLookupTable);
	this.setInstanceFilter(opts.instanceFilter);

	this.setFeatureExpansion(opts.featureExpansion);
	this.featureExpansionScale = opts.featureExpansionScale;
	this.featureExpansionPhrase = opts.featureExpansionPhrase;
	this.featureFine = opts.featureFine;

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.setFeatureExtractor"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>setFeatureExtractor (featureExtractor)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.setFeatureExtractor)
- description and source-code
```javascript
setFeatureExtractor = function (featureExtractor) {
		this.featureExtractors = ftrs.normalize(featureExtractor);
	}
```
- example usage
```shell
...
		throw new Error("opts must contain classifierType");
	}

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.setFeatureExtractorForClassification"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>setFeatureExtractorForClassification (featureExtractorForClassification)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.setFeatureExtractorForClassification)
- description and source-code
```javascript
setFeatureExtractorForClassification = function (featureExtractorForClassification) {
		if (featureExtractorForClassification) {
			if (Array.isArray(featureExtractorForClassification)) {
				featureExtractorForClassification.unshift(this.featureExtractors);
			} else {
				featureExtractorForClassification = [this.featureExtractors, featureExtractorForClassification];
			}
			this.featureExtractorsForClassification = new ftrs.CollectionOfExtractors(featureExtractorForClassification);
		}
	}
```
- example usage
```shell
...
	}

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.setFeatureLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.setFeatureLookupTable)
- description and source-code
```javascript
setFeatureLookupTable = function (featureLookupTable) {
		if (featureLookupTable) {
			this.featureLookupTable = featureLookupTable;
			if (this.classifier.setFeatureLookupTable)
				this.classifier.setFeatureLookupTable(featureLookupTable);  // for generating clearer explanations only
		}
	}
```
- example usage
```shell
...

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
	this.tfidf = new opts.TfIdfImpl
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.setInstanceFilter"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>setInstanceFilter (instanceFilter)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.setInstanceFilter)
- description and source-code
```javascript
setInstanceFilter = function (instanceFilter) {
		this.instanceFilter = instanceFilter;
	}
```
- example usage
```shell
...
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	// this.setFeatureLookupTable(opts.featureLookupTable);
	this.setFeatureLookupTable(new ftrs.FeatureLookupTable());

	this.setLabelLookupTable(opts.labelLookupTable);
	this.setInstanceFilter(opts.instanceFilter);

	this.setFeatureExpansion(opts.featureExpansion);
	this.featureExpansionScale = opts.featureExpansionScale;
	this.featureExpansionPhrase = opts.featureExpansionPhrase;
	this.featureFine = opts.featureFine;

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.setLabelLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>setLabelLookupTable (labelLookupTable)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.setLabelLookupTable)
- description and source-code
```javascript
setLabelLookupTable = function (labelLookupTable) {
		if (labelLookupTable) {
			this.labelLookupTable = labelLookupTable;
			if (this.classifier.setLabelLookupTable)
				this.classifier.setLabelLookupTable(labelLookupTable);  // for generating clearer explanations only
			this.applyFeatureExpansion();
		}
	}
```
- example usage
```shell
...
	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
    	this.tfidf = new opts.TfIdfImpl
		this.featureDocumentFrequency = {};
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.setNormalizer"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>setNormalizer (normalizer)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.setNormalizer)
- description and source-code
```javascript
setNormalizer = function (normalizer) {
		if (normalizer)
			this.normalizers = (Array.isArray(normalizer)? normalizer: [normalizer]);
	}
```
- example usage
```shell
...
		console.dir(opts);
		throw new Error("opts must contain classifierType");
	}

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>toJSON (callback)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.toJSON)
- description and source-code
```javascript
toJSON = function (callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
		var featureLookupTable = this.featureLookupTable;
		var pastTrainingSamples = this.pastTrainingSamples;

			// if (this.spellChecker) {
				// var seeds = []
				// var trainings = []
				// this.spellChecker[0].initializeSync(seeds.toString().split("\r\n"), trainings.toString().split("\r\n"))
			// }

			dataset = _.map(dataset, function(datum){
						if (_.isObject(datum.input))
							datum.input.text = this.normalizedSample(datum.input.text);
						else	
							datum.input = this.normalizedSample(datum.input);
						return datum
					}, this);
			
			if ((typeof this.preProcessor === 'function')) {
				dataset = _.map(dataset, function(value){ return this.preProcessor(value) }, this);
			}

			dataset = _.compact(dataset)

			dataset = dataset.map(function(datum) {
				datum = _(datum).clone();

				var features = this.sampleToFeatures(datum.input, this.featureExtractors);
				if (this.tfidf)
					this.tfidf.addDocument(features);
				if (featureLookupTable)
					featureLookupTable.addFeatures(features);

				datum.input = features;
				return datum;
			}, this);

			dataset = _.compact(dataset)

		dataset.forEach(function(datum) {
			// run on single sentence
			this.editFeatureValues(datum.input, /*remove_unknown_features=*/false);
			if (featureLookupTable)
				datum.input = featureLookupTable.hashToArray(datum.input);
		}, this);

		this.classifier.trainBatch(dataset);

	}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.trainBatchAsync"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>trainBatchAsync (dataset, callbackg)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.trainBatchAsync)
- description and source-code
```javascript
trainBatchAsync = function (dataset, callbackg) {
		var featureLookupTable = this.featureLookupTable;
		var pastTrainingSamples = this.pastTrainingSamples;

		processed_dataset = []

		async.forEachOfSeries(dataset, (function(datum, dind, callback2){
			
			if (_.isObject(datum.input))
				datum.input.text = this.normalizedSample(datum.input.text);
			else	
				datum.input = this.normalizedSample(datum.input);

			if (typeof this.preProcessor === 'function')
				datum = this.preProcessor(datum)

			if (!_.isUndefined(datum))
			{
				this.sampleToFeaturesAsync(datum.input, this.featureExtractors, (function(err, features){
			
					// this.omitStopWords(features, this.stopwords)

					if (this.tfidf)
						this.tfidf.addDocument(features)
					
					if (featureLookupTable)
						featureLookupTable.addFeatures(features)

					datum.input = features
					processed_dataset.push(datum)

					callback2()
				}).bind(this))
			}
			else
			callback2()

		}).bind(this), (function(err){

			processed_dataset = _.compact(processed_dataset)

			processed_dataset.forEach(function(datum) {
			
				this.editFeatureValues(datum.input, /*remove_unknown_features=*/false);
				if (featureLookupTable)
					datum.input = featureLookupTable.hashToArray(datum.input);
			}, this)

			this.classifier.trainBatch(processed_dataset)
			callbackg(null,[])
		
		}).bind(this))
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>trainOnline (sample, classes)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
	}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```

#### <a name="apidoc.element.limdu.EnhancedClassifier_2015.prototype.trainSpellChecker"></a>[function <span class="apidocSignatureSpan">limdu.EnhancedClassifier_2015.prototype.</span>trainSpellChecker (features)](#apidoc.element.limdu.EnhancedClassifier_2015.prototype.trainSpellChecker)
- description and source-code
```javascript
trainSpellChecker = function (features) {
		if (this.spellChecker) {
			var tokens = this.tokenizer.tokenize(features);
			_.each(tokens, function(word, key, list){
				this.spellChecker[1].understand(word); // Adds the given word to the index of the spell-checker.
				this.spellChecker[1].train(word);
			}, this)
		}
	}
```
- example usage
```shell
...
	 * @param classes an array whose VALUES are classes.
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
	},
...
```



# <a name="apidoc.module.limdu.arff"></a>[module limdu.arff](#apidoc.module.limdu.arff)

#### <a name="apidoc.element.limdu.arff.toARFF"></a>[function <span class="apidocSignatureSpan">limdu.arff.</span>toARFF (dataset, relationName, featureExtractor)](#apidoc.element.limdu.arff.toARFF)
- description and source-code
```javascript
toARFF = function (dataset, relationName, featureExtractor) {
	if (!featureExtractor) featureExtractor=_.identity;
	
	var featureLookupTable = new FeaturesUnit.FeatureLookupTable();
	
	// Extract the input attributes (- features):
	dataset.forEach(function(datum) {
		datum.input = featureExtractor(datum.input, {});
		if (!_.isObject(datum.input))
			throw new Error("Expected feature vector to be a hash, but found "+JSON.stringify(datum.input));
		featureLookupTable.addFeatures(datum.input);
	});
	
	// Extract the target attributes (- classes):
	dataset.forEach(function(datum) {
		if (!_.isArray(datum.output))
			datum.output = [datum.output];
		datum.output = datum.output.map(function(anOutput) {
			return _.isString(anOutput)? anOutput: JSON.stringify(anOutput);
		});
		featureLookupTable.addFeatures(datum.output);
	});

	//console.dir(featureLookupTable);
	return toARFFLocal(dataset, relationName, featureLookupTable);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.arff.toARFFs"></a>[function <span class="apidocSignatureSpan">limdu.arff.</span>toARFFs (outputFolder, mapFileNameToDataset, featureExtractor)](#apidoc.element.limdu.arff.toARFFs)
- description and source-code
```javascript
toARFFs = function (outputFolder, mapFileNameToDataset, featureExtractor) {
	if (!featureExtractor) featureExtractor=_.identity;
	var featureLookupTable = new FeaturesUnit.FeatureLookupTable();
	
	// Extract the input attributes (- features):
	for (var relationName in mapFileNameToDataset) {
		mapFileNameToDataset[relationName].forEach(function(datum) {
			datum.input = featureExtractor(datum.input, {});
			if (!_.isObject(datum.input))
				throw new Error("Expected feature vector to be a hash, but found "+JSON.stringify(datum.input));
			featureLookupTable.addFeatures(datum.input);
		});
	}
	
	
	// Extract the target attributes (- classes):
	for (var relationName in mapFileNameToDataset) {
		mapFileNameToDataset[relationName].forEach(function(datum) {
			if (!_.isArray(datum.output))
				datum.output = [datum.output];
			datum.output = datum.output.map(function(anOutput) {
				return _.isString(anOutput)? anOutput: JSON.stringify(anOutput);
			});
			featureLookupTable.addFeatures(datum.output);
		});
	}
	

	//console.dir(featureLookupTable);

	var fs = require('fs');
	for (var relationName in mapFileNameToDataset) {
		fs.writeFileSync(outputFolder+"/"+relationName+".arff",
			toARFFLocal(mapFileNameToDataset[relationName], relationName, featureLookupTable));
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.classifiers"></a>[module limdu.classifiers](#apidoc.module.limdu.classifiers)

#### <a name="apidoc.element.limdu.classifiers.Bayesian"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>Bayesian (options)](#apidoc.element.limdu.classifiers.Bayesian)
- description and source-code
```javascript
Bayesian = function (options) {
	options = options || {}
	this.thresholds = options.thresholds || {};
	this.globalThreshold = options.globalThreshold || 1;
	this.default = options.default || 'unclassified';
	this.weight = options.weight || 1;
	this.assumed = options.assumed || 0.5;
	this.normalizeOutputProbabilities = options.normalizeOutputProbabilities||false;
	this.calculateRelativeProbabilities = options.calculateRelativeProbabilities||false;

	var backend = options.backend || { type: 'memory' };
	switch(backend.type.toLowerCase()) {
		case 'redis':
			//this.backend = new (require("./backends/redis").RedisBackend)(backend.options);
			throw new Error("Redis backend support was dropped, in order to remove dependencies");
			break;
		case 'localstorage':
			this.backend = new (require("./backends/localStorage")
										 .LocalStorageBackend)(backend.options);
			break;
		default:
			this.backend = new (require("./backends/memory").MemoryBackend)();
	}
}
```
- example usage
```shell
...
'''

### Explanations

Some classifiers can return "explanations" - additional information that explains how the classification result has been derived
:

'''js
var colorClassifier = new limdu.classifiers.Bayesian();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 'black'},
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 'white'},
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 'white'},
	]);
...
```

#### <a name="apidoc.element.limdu.classifiers.DecisionTree"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>DecisionTree (opts)](#apidoc.element.limdu.classifiers.DecisionTree)
- description and source-code
```javascript
function DecisionTree(opts) {
	if (!opts) opts = {}
	// this.debug = opts.debug || false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>EnhancedClassifier (opts)](#apidoc.element.limdu.classifiers.EnhancedClassifier)
- description and source-code
```javascript
EnhancedClassifier = function (opts) {
	if (!opts.classifierType) {
		console.dir(opts);
		throw new Error("opts must contain classifierType");
	}

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
    	this.tfidf = new opts.TfIdfImpl
		this.featureDocumentFrequency = {};
		}
	this.bias = opts.bias;

	this.spellChecker = opts.spellChecker;
	this.tokenizer = opts.tokenizer;
	this.instanceFilterRule = opts.instanceFilter

	// this.spellChecker =  [require('wordsworth').getInstance(), require('wordsworth').getInstance()],
	// this.pastTrainingSamples = opts.pastTrainingSamples;
	// TODO: it looks like the method with creating an array at the definition
	// create an array with the same pointer for every classifier of the given class
	
	this.pastTrainingSamples = []

	this.InputSplitLabel = opts.InputSplitLabel
	this.OutputSplitLabel = opts.OutputSplitLabel
	this.TestSplitLabel = opts.TestSplitLabel
}
```
- example usage
```shell
...
var WordExtractor = function(input, features) {
	input.split(" ").forEach(function(word) {
		features[word]=1;
	});
};

// Initialize a classifier with the base classifier type and the feature extractor:
var intentClassifier = new limdu.classifiers.EnhancedClassifier({
	classifierType: TextClassifier,
	featureExtractor: WordExtractor
});

// Train and test:
intentClassifier.trainBatch([
	{input: "I want an apple", output: "apl"},
...
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>NeuralNetwork (options)](#apidoc.element.limdu.classifiers.NeuralNetwork)
- description and source-code
```javascript
NeuralNetwork = function (options) {
  options = options || {};
  this.learningRate = options.learningRate || 0.3;
  this.momentum = options.momentum || 0.1;
  this.hiddenSizes = options.hiddenLayers;

  this.binaryThresh = options.binaryThresh || 0.5;
}
```
- example usage
```shell
...
## Binary Classification

### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);
...
```

#### <a name="apidoc.element.limdu.classifiers.Perceptron"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>Perceptron (opts)](#apidoc.element.limdu.classifiers.Perceptron)
- description and source-code
```javascript
Perceptron = function (opts) {
	if (!opts) opts = {};
	
	this.debug = opts.debug||false;
	this.default_weight = opts.default_weight||0;
	this.do_averaging = opts.do_averaging||false;
	this.do_normalization = opts.do_normalization||false;
	this.learning_rate = opts.learning_rate||0.1;
	this.retrain_count = 'retrain_count' in opts? opts.retrain_count: 1;
	
	this.weights = {};
	if (this.do_averaging) this.weights_sum = {};   // for averaging; see http://ciml.info/dl/v0_8/ciml-v0_8-ch03.pdf . But count only
 weight vectors with successful predictions (Carvalho and Cohen, 2006).
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.SvmJs"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>SvmJs (opts)](#apidoc.element.limdu.classifiers.SvmJs)
- description and source-code
```javascript
function SvmJs(opts) {
	this.base = new SvmJsBase();
	this.opts = opts;  // options for SvmJsBase.train
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.SvmLinear"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>SvmLinear (opts)](#apidoc.element.limdu.classifiers.SvmLinear)
- description and source-code
```javascript
function SvmLinear(opts) {
	this.learn_args = opts.learn_args || "";
	this.model_file_prefix = opts.model_file_prefix || null;
	this.bias = opts.bias || 1.0;
	this.multiclass = opts.multiclass || false;
	this.debug = opts.debug||false;
	this.train_command = opts.train_command || 'liblinear_train';
	this.test_command = opts.test_command || 'liblinear_test';
	this.timestamp = ""

	if (!SvmLinear.isInstalled()) {
                var msg = "Cannot find the executable 'liblinear_train'. Please download it from the LibLinear website, and put
a link to it in your path.";
                console.error(msg)
                throw new Error(msg);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.SvmPerf"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>SvmPerf (opts)](#apidoc.element.limdu.classifiers.SvmPerf)
- description and source-code
```javascript
function SvmPerf(opts) {
	if (!SvmPerf.isInstalled()) {
	 	var msg = "Cannot find the executable 'svm_perf_learn'. Please download it from the SvmPerf website, and put a link to it in
your path.";
	 	console.error(msg)
	 	throw new Error(msg);
	}
	this.learn_args = opts.learn_args || "";
	this.learn_args += " --b 0 ";  // we add the bias here, so we don't need SvmPerf to add it
	this.model_file_prefix = opts.model_file_prefix || null;
	this.bias = 'bias' in opts? opts.bias: 1.0;
	this.debug = opts.debug || false;
	this.ShowFeat = {}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.Winnow"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>Winnow (opts)](#apidoc.element.limdu.classifiers.Winnow)
- description and source-code
```javascript
function WinnowHash(opts) {
	if (!opts) opts = {}

	this.debug = opts.debug || false;
		
	// Default values are based on Carvalho and Cohen, 2006, section 4.2:	
	this.default_positive_weight = opts.default_positive_weight || 2.0;
	this.default_negative_weight = opts.default_negative_weight || 1.0;
	this.do_averaging = opts.do_averaging || false;
	this.threshold = ('threshold' in opts? opts.threshold: 1);
	this.promotion = opts.promotion || 1.5;
	this.demotion = opts.demotion || 0.5;
	this.margin = ('margin' in opts? opts.margin: 1.0);
	this.retrain_count = opts.retrain_count || 0;
	this.detailed_explanations = opts.detailed_explanations || false;
	
	this.bias = ('bias' in opts? opts.bias: 1.0);

	this.positive_weights = {};
	this.negative_weights = {};
	this.positive_weights_sum = {};   // for averaging; count only weight vectors with successful predictions (Carvalho and Cohen,
2006).
	this.negative_weights_sum = {};   // for averaging; count only weight vectors with successful predictions (Carvalho and Cohen,
2006).
}
```
- example usage
```shell
...
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
...
```

#### <a name="apidoc.element.limdu.classifiers.kNN"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>kNN (opts)](#apidoc.element.limdu.classifiers.kNN)
- description and source-code
```javascript
kNN = function (opts) {
	this.k = opts.k
	this.mode = opts.mode
	this.distanceFunctionList = opts.distanceFunctionList
	this.distanceWeightening = opts.distanceWeightening
	this.labels = []
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.classifiers.Bayesian"></a>[module limdu.classifiers.Bayesian](#apidoc.module.limdu.classifiers.Bayesian)

#### <a name="apidoc.element.limdu.classifiers.Bayesian.Bayesian"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>Bayesian (options)](#apidoc.element.limdu.classifiers.Bayesian.Bayesian)
- description and source-code
```javascript
Bayesian = function (options) {
	options = options || {}
	this.thresholds = options.thresholds || {};
	this.globalThreshold = options.globalThreshold || 1;
	this.default = options.default || 'unclassified';
	this.weight = options.weight || 1;
	this.assumed = options.assumed || 0.5;
	this.normalizeOutputProbabilities = options.normalizeOutputProbabilities||false;
	this.calculateRelativeProbabilities = options.calculateRelativeProbabilities||false;

	var backend = options.backend || { type: 'memory' };
	switch(backend.type.toLowerCase()) {
		case 'redis':
			//this.backend = new (require("./backends/redis").RedisBackend)(backend.options);
			throw new Error("Redis backend support was dropped, in order to remove dependencies");
			break;
		case 'localstorage':
			this.backend = new (require("./backends/localStorage")
										 .LocalStorageBackend)(backend.options);
			break;
		default:
			this.backend = new (require("./backends/memory").MemoryBackend)();
	}
}
```
- example usage
```shell
...
'''

### Explanations

Some classifiers can return "explanations" - additional information that explains how the classification result has been derived
:

'''js
var colorClassifier = new limdu.classifiers.Bayesian();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 'black'},
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 'white'},
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 'white'},
	]);
...
```



# <a name="apidoc.module.limdu.classifiers.Bayesian.prototype"></a>[module limdu.classifiers.Bayesian.prototype](#apidoc.module.limdu.classifiers.Bayesian.prototype)

#### <a name="apidoc.element.limdu.classifiers.Bayesian.prototype.bestMatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>bestMatch (pairs)](#apidoc.element.limdu.classifiers.Bayesian.prototype.bestMatch)
- description and source-code
```javascript
bestMatch = function (pairs) {
		var maxCategory = pairs[0][0];
		var maxProbability = pairs[0][1];

		if (pairs.length>1) {
			var nextProbability = pairs[1][1];
			var threshold = this.thresholds[maxCategory] || this.globalThreshold;
			if (nextProbability * threshold > maxProbability)
				maxCategory = this.default; // not greater than other category by enough
			if (this.calculateRelativeProbabilities)
				maxProbability /= nextProbability;
		}

		return {
			category: maxCategory,
			probability: maxProbability
		};
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.Bayesian.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>classify (document, explain)](#apidoc.element.limdu.classifiers.Bayesian.prototype.classify)
- description and source-code
```javascript
classify = function (document, explain) {
		if (!_.isObject(document)) {
			throw new Error("document should be a feature-value hash, but it is "+JSON.stringify(document));
		}
		var probs = this.getProbsSync(document);

		var max = this.bestMatch(probs);
		if (explain>0) {
			return {
				classes: max.category,
				explanation: probs.map(function(pair) {
					return pair[0]+": "+pair[1]
				})
			};
		} else {
			return max.category;
		}
	}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.Bayesian.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.Bayesian.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.Bayesian.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>fromJSON (json, callback)](#apidoc.element.limdu.classifiers.Bayesian.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json, callback) {
		this.backend.fromJSON(json, callback);
	}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.Bayesian.prototype.getCatProbs"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>getCatProbs (cats, document, counts)](#apidoc.element.limdu.classifiers.Bayesian.prototype.getCatProbs)
- description and source-code
```javascript
getCatProbs = function (cats, document, counts) {
		var numDocs = _(cats).reduce(function(sum, count) {
			return sum + count;
		}, 0);  // total number of training samples in all categories

		var probs = {};
		_(cats).each(function(catCount, cat) {
			var catPriorProb = (catCount || 0) / numDocs;

			// The probability to see a document is the product
			//     of the probability to see each word in the document.
			var docProb = _(Object.keys(document)).reduce(function(prob, word) {
				var wordCounts = counts[word] || {};
				var probWordGivenCat = this.wordProb(word, cat, cats, wordCounts);
				var probWordsGivenCat = Math.pow(probWordGivenCat, document[word]);
				//console.log("probWordGivenCat="+probWordGivenCat+" probWordsGivenCat="+probWordsGivenCat+" document[word]="+document[word])
				return prob * probWordsGivenCat;
			}, 1, this);
			//console.log("docProb="+docProb)

			// the probability this doc is in this category
			probs[cat] = catPriorProb * docProb;
		}, this);
		return probs;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.Bayesian.prototype.getCats"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>getCats (callback)](#apidoc.element.limdu.classifiers.Bayesian.prototype.getCats)
- description and source-code
```javascript
getCats = function (callback) {
			return this.backend.getCats(callback);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.Bayesian.prototype.getProbsSync"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>getProbsSync (document)](#apidoc.element.limdu.classifiers.Bayesian.prototype.getProbsSync)
- description and source-code
```javascript
getProbsSync = function (document) {
		var cats = this.getCats(); // a hash with the possible categories: { 'cat1': 1, 'cat2': 1 }
		var counts = this.getWordCounts(Object.keys(document), cats); // For each word encountered during training, the counts of times
 it occurred in each category.

		var probs = this.getCatProbs(cats, document, counts); // The probabilities that the given document belongs to each of the categories
, i.e.: { 'cat1': 0.1875, 'cat2': 0.0625 }

		if (this.normalizeOutputProbabilities) {
			var sum = _(probs).reduce(function(memo, num) { return memo + num; }, 0);
			for (var cat in probs)
				probs[cat] = probs[cat]/sum;
		}

		var pairs = _.pairs(probs);   // pairs of [category,probability], for all categories that appeared in the training set.
		//console.dir(pairs);
		if (pairs.length==0) {
			return {category: this.default, probability: 0};
		}
		pairs.sort(function(a,b) {   // sort by decreasing prob
			return b[1]-a[1];
		});

		return pairs;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.Bayesian.prototype.getWordCounts"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>getWordCounts (words, cats, callback)](#apidoc.element.limdu.classifiers.Bayesian.prototype.getWordCounts)
- description and source-code
```javascript
getWordCounts = function (words, cats, callback) {
			return this.backend.getWordCounts(words, cats, callback);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.Bayesian.prototype.incDocCounts"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>incDocCounts (samples, callback)](#apidoc.element.limdu.classifiers.Bayesian.prototype.incDocCounts)
- description and source-code
```javascript
incDocCounts = function (samples, callback) {
			// accumulate all the pending increments
			var wordIncs = {};
			var catIncs = {};
			samples.forEach(function(sample) {
				var cat = sample.output;
				//if (_.isObject(cat))
				//	cat = JSON.stringify(cat);
				catIncs[cat] = catIncs[cat] ? catIncs[cat] + 1: 1;

				var features = sample.input;
				for (var feature in features) {
					wordIncs[feature] = wordIncs[feature] || {};
					wordIncs[feature][cat] = wordIncs[feature][cat] || 0;
					wordIncs[feature][cat] += features[feature];
				}
			}, this);

			return this.backend.incCounts(catIncs, wordIncs, callback);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.Bayesian.prototype.setThresholds"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>setThresholds (thresholds)](#apidoc.element.limdu.classifiers.Bayesian.prototype.setThresholds)
- description and source-code
```javascript
setThresholds = function (thresholds) {
			this.thresholds = thresholds;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.Bayesian.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>toJSON (callback)](#apidoc.element.limdu.classifiers.Bayesian.prototype.toJSON)
- description and source-code
```javascript
toJSON = function (callback) {
		return this.backend.toJSON(callback);
	}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.Bayesian.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>trainBatch (data)](#apidoc.element.limdu.classifiers.Bayesian.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (data) {
		this.incDocCounts(data);
	}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.Bayesian.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>trainOnline (document, category)](#apidoc.element.limdu.classifiers.Bayesian.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (document, category) {
		this.incDocCounts([{input: document, output: category}]);
	}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```

#### <a name="apidoc.element.limdu.classifiers.Bayesian.prototype.wordProb"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Bayesian.prototype.</span>wordProb (word, cat, cats, wordCounts)](#apidoc.element.limdu.classifiers.Bayesian.prototype.wordProb)
- description and source-code
```javascript
wordProb = function (word, cat, cats, wordCounts) {
		// times word appears in a doc in this cat / docs in this cat
		var probWordGivenCat = (wordCounts[cat] || 0) / cats[cat];

		var totalWordCount = _(cats).reduce(function(sum, p, cat) {
			return sum + (wordCounts[cat] || 0);
		}, 0, this);
		// get weighted average with assumed so prob won't be extreme on rare words
		var modifiedProbGivenCat = (this.weight * this.assumed + totalWordCount * probWordGivenCat) / (this.weight + totalWordCount);

		//console.log("word="+word+" cat="+cat+" probWordGivenCat="+probWordGivenCat+" totalWordCount="+totalWordCount+" modifiedProbGivenCat
="+modifiedProbGivenCat)
		return modifiedProbGivenCat
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.classifiers.DecisionTree"></a>[module limdu.classifiers.DecisionTree](#apidoc.module.limdu.classifiers.DecisionTree)

#### <a name="apidoc.element.limdu.classifiers.DecisionTree.DecisionTree"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>DecisionTree (opts)](#apidoc.element.limdu.classifiers.DecisionTree.DecisionTree)
- description and source-code
```javascript
function DecisionTree(opts) {
	if (!opts) opts = {}
	// this.debug = opts.debug || false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.classifiers.DecisionTree.prototype"></a>[module limdu.classifiers.DecisionTree.prototype](#apidoc.module.limdu.classifiers.DecisionTree.prototype)

#### <a name="apidoc.element.limdu.classifiers.DecisionTree.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>classify (features, explain, continuous_output)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.classify)
- description and source-code
```javascript
classify = function (features, explain, continuous_output) {
		    root = this.root;
            while (root.type !== "result") {
                var attr = root.name;
                var sampleVal = features[attr];
                        var childNode = _.detect(root.vals,function(x) { return x.name == sampleVal });
                        root = childNode.child;
                }
            return root.val;
		}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.DecisionTree.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.DecisionTree.prototype.count"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>count (a, l)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.count)
- description and source-code
```javascript
count = function (a, l) {
        	return _.filter(l,function(b) { return b === a}).length
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.DecisionTree.prototype.createTree"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>createTree (dataset, features)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.createTree)
- description and source-code
```javascript
createTree = function (dataset, features) {
			var targets = _.unique(_.pluck(dataset, 'output'));
			if (targets.length == 1){
                // console.log("end node! "+targets[0]);
                return {type:"result", val: targets[0], name: targets[0], alias:targets[0]+this.randomTag() };
        	}
        	 if(features.length == 0){
                // console.log("returning the most dominate feature!!!");
                var topTarget = this.mostCommon(targets);
                return {type:"result", val: topTarget, name: topTarget, alias: topTarget+this.randomTag()};
        	}
        	var bestFeature = this.maxGain(dataset, features);
			var remainingFeatures = _.without(features,bestFeature);
        	var possibleValues = _.unique(_.pluck(_.pluck(dataset, 'input'), bestFeature));
        	var node = {name: bestFeature,alias: bestFeature+this.randomTag()};
        	node.type = "feature";
        	node.vals = _.map(possibleValues,function(v){
                var _newS = dataset.filter(function(x) {return x['input'][bestFeature] == v});
                var child_node = {name:v,alias:v+this.randomTag(),type: "feature_value"};
                child_node.child =  this.createTree(_newS,remainingFeatures);
                return child_node;
        }, this);

        return node;
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.DecisionTree.prototype.entropy"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>entropy (vals)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.entropy)
- description and source-code
```javascript
entropy = function (vals){
	        var uniqueVals = _.unique(vals);
	        var probs = uniqueVals.map(function(x){return this.prob(x,vals)}, this);
	        var logVals = probs.map(function(p){return -p*this.log2(p) }, this);
	        return logVals.reduce(function(a,b){return a+b},0);
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.DecisionTree.prototype.extractFeatures"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>extractFeatures (dataset)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.extractFeatures)
- description and source-code
```javascript
extractFeatures = function (dataset) {
			var features = []
			for (record in dataset)
			{
				for (key in dataset[record]['input'])
				{
					features.push(key)
				}
			}
			return features
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.DecisionTree.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
			this.root = json
		}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.DecisionTree.prototype.gain"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>gain (dataset, feature)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.gain)
- description and source-code
```javascript
gain = function (dataset, feature){
        	var attrVals = _.unique(_.pluck(_.pluck(dataset, 'input'), feature));
            var setEntropy = this.entropy(_.pluck(dataset, 'output'));
        	var setSize = _.size(dataset);
        	var entropies = attrVals.map(function(n){
            	var subset = dataset.filter(function(x){return x['input'][feature] === n});
                return (subset.length/setSize)*this.entropy(_.pluck(subset,'output'));
        	 }, this);
        	var sumOfEntropies =  entropies.reduce(function(a,b){return a+b},0);
        	return setEntropy - sumOfEntropies;
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.DecisionTree.prototype.log2"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>log2 (n)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.log2)
- description and source-code
```javascript
log2 = function (n){
	        return Math.log(n)/Math.log(2);
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.DecisionTree.prototype.maxGain"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>maxGain (dataset, features)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.maxGain)
- description and source-code
```javascript
maxGain = function (dataset, features) {
	        return _.max(features,function(e){return this.gain(dataset,e)}, this)
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.DecisionTree.prototype.mostCommon"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>mostCommon (l)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.mostCommon)
- description and source-code
```javascript
mostCommon = function (l) {
        	return  _.sortBy(l,function(a){ return this.count(a,l); },this).reverse()[0];
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.DecisionTree.prototype.prob"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>prob (val, vals)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.prob)
- description and source-code
```javascript
prob = function (val, vals){
	        var instances = _.filter(vals,function(x) {return x === val}).length;
	        var total = vals.length;
	        return instances/total;
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.DecisionTree.prototype.randomTag"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>randomTag ()](#apidoc.element.limdu.classifiers.DecisionTree.prototype.randomTag)
- description and source-code
```javascript
randomTag = function () {
        	return "_r"+Math.round(Math.random()*1000000).toString();
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.DecisionTree.prototype.setFeatureLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.setFeatureLookupTable)
- description and source-code
```javascript
setFeatureLookupTable = function (featureLookupTable) {
			this.featureLookupTable = featureLookupTable;
		}
```
- example usage
```shell
...

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
	this.tfidf = new opts.TfIdfImpl
...
```

#### <a name="apidoc.element.limdu.classifiers.DecisionTree.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>toJSON (folder)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.toJSON)
- description and source-code
```javascript
toJSON = function (folder) {
			return this.root
		}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.DecisionTree.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.DecisionTree.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.DecisionTree.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
			features = this.extractFeatures(dataset)
			this.root = this.createTree(dataset, features)
		}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```



# <a name="apidoc.module.limdu.classifiers.EnhancedClassifier"></a>[module limdu.classifiers.EnhancedClassifier](#apidoc.module.limdu.classifiers.EnhancedClassifier)

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.EnhancedClassifier"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>EnhancedClassifier (opts)](#apidoc.element.limdu.classifiers.EnhancedClassifier.EnhancedClassifier)
- description and source-code
```javascript
EnhancedClassifier = function (opts) {
	if (!opts.classifierType) {
		console.dir(opts);
		throw new Error("opts must contain classifierType");
	}

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
    	this.tfidf = new opts.TfIdfImpl
		this.featureDocumentFrequency = {};
		}
	this.bias = opts.bias;

	this.spellChecker = opts.spellChecker;
	this.tokenizer = opts.tokenizer;
	this.instanceFilterRule = opts.instanceFilter

	// this.spellChecker =  [require('wordsworth').getInstance(), require('wordsworth').getInstance()],
	// this.pastTrainingSamples = opts.pastTrainingSamples;
	// TODO: it looks like the method with creating an array at the definition
	// create an array with the same pointer for every classifier of the given class
	
	this.pastTrainingSamples = []

	this.InputSplitLabel = opts.InputSplitLabel
	this.OutputSplitLabel = opts.OutputSplitLabel
	this.TestSplitLabel = opts.TestSplitLabel
}
```
- example usage
```shell
...
var WordExtractor = function(input, features) {
	input.split(" ").forEach(function(word) {
		features[word]=1;
	});
};

// Initialize a classifier with the base classifier type and the feature extractor:
var intentClassifier = new limdu.classifiers.EnhancedClassifier({
	classifierType: TextClassifier,
	featureExtractor: WordExtractor
});

// Train and test:
intentClassifier.trainBatch([
	{input: "I want an apple", output: "apl"},
...
```



# <a name="apidoc.module.limdu.classifiers.EnhancedClassifier.prototype"></a>[module limdu.classifiers.EnhancedClassifier.prototype](#apidoc.module.limdu.classifiers.EnhancedClassifier.prototype)

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.backClassify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>backClassify (theClass)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.backClassify)
- description and source-code
```javascript
backClassify = function (theClass) {
		if (!this.pastTrainingSamples)
			throw new Error("No pastTrainingSamples array - can't backClassify");

		if (!(theClass instanceof Array))
			theClass = [theClass];
		var samples = [];
		this.pastTrainingSamples.forEach(function(datum) {
			if (_(datum.output).isEqual(theClass))
				samples.push(datum.input);
		});
		return samples;
	}
```
- example usage
```shell
...
intentClassifier.trainBatch([
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I really want an apple", output: "apl"},
	{input: "I want a banana very much", output: "bnn"},
	]);

console.dir(intentClassifier.backClassify("apl"));  // [ 'I want an apple', 'I really want an apple' ]
'''

## SVM wrappers

The native svm.js implementation takes a lot of time to train -  quadratic in the number of training samples.
There are two common packages that can be trained in time linear in the number of training samples. They are:
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>classify (sample, explain, continuous_output, original, classifier_compare)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.classify)
- description and source-code
```javascript
classify = function (sample, explain, continuous_output, original, classifier_compare) {
		var initial = sample
		sample = this.normalizedSample(sample)

		if (this.instanceFilter(sample))
			{	if (explain>0)
				return {
					classes: [],
					scores: {},
					explanation: {}
					// bonus: bonus
				};
			else
				return []
			}		
		
		if (!this.inputSplitter) {
			var classesWithExplanation = this.classifyPart(sample, explain, continuous_output);
			var classes = (explain>0? classesWithExplanation.classes: classesWithExplanation);
			var scores =  (continuous_output? classesWithExplanation.scores: null)
			var explanations = (explain>0? classesWithExplanation.explanation: null);
		} else {
			var parts = this.inputSplitter(sample);
			// var accumulatedClasses = {};
			var accumulatedClasses = [];
			var explanations = [];
			parts.forEach(function(part) {
				if (part.length==0) return;
				var classesWithExplanation = this.classifyPart(part, explain, continuous_output);
				var classes = (explain>0? classesWithExplanation.classes: classesWithExplanation);
				// for (var i in classes)
				// 	accumulatedClasses[classes[i]]=true;
				accumulatedClasses.push(classes)
				if (explain>0) {
					// explanations.push(part);
					explanations.push(classesWithExplanation.explanation);
				}
			}, this);
    		classes = []
    		if (accumulatedClasses[0])
    		{
			if (accumulatedClasses[0][0] instanceof Array)
				_(accumulatedClasses[0].length).times(function(n){
					classes.push(_.flatten(_.pluck(accumulatedClasses,n)))
				 });
			else
			{
				classes = _.flatten(accumulatedClasses)
			}
			}
		}

		if (this.labelLookupTable) {
			if (Array.isArray(classes)) {
				classes = classes.map(function(label) {
						if (_.isArray(label))
							label[0] = this.labelLookupTable.numberToFeature(label[0]);
						else
							label = this.labelLookupTable.numberToFeature(label);
						return label;
					}, this);
			} else {
				classes = this.labelLookupTable.numberToFeature(classes);
			}
		}

		if ((typeof this.OutputSplitLabel === 'function')) {

			// classes = this.OutputSplitLabel(classes, this.Observable, sample, explanations)
			// var classes = []
			// if (_.isArray(explanations))
			// var bonus = []
		
			if ((explain>0) && (this.inputSplitter))
				{ nclasses = []
				_(explanations.length).times(function(n){
					var clas = this.OutputSplitLabel(classes, this, parts[n], explanations[n], original, classifier_compare, initial)
					nclasses = nclasses.concat(clas)
				}, this)
				classes = nclasses
				}
			else
				{
				var classes = this.OutputSplitLabel(classes, this, sample, explanations, original, classifier_compare, initial)
				}
			}

		if (explain>0)
			return {
				classes: classes,
				scores: scores,
				explanation: explanations
				// bonus: bonus
			};
		else
			return classes;
	}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.classifyPart"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>classifyPart (sample, explain, continuous_output)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.classifyPart)
- description and source-code
```javascript
classifyPart = function (sample, explain, continuous_output) {
		
		var samplecorrected = this.correctFeatureSpelling(sample);
		var features = this.sampleToFeatures(samplecorrected, this.featureExtractors);
		this.editFeatureValues(features, /*remove_unknown_features=*/true);
		var array = this.featuresToArray(features);
		var classification = this.classifier.classify(array, explain, continuous_output);
		
		// if (this.spellChecker && classification.explanation) {
			// if (Array.isArray(classification.explanation))
				// classification.explanation.unshift({SpellCorrectedFeatures: JSON.stringify(features)});
			// else
				// classification.explanation['SpellCorrectedFeatures']=JSON.stringify(features);
		// }
		return classification;
	}
```
- example usage
```shell
...
					// bonus: bonus
				};
			else
				return []
			}		
		
		if (!this.inputSplitter) {
			var classesWithExplanation = this.classifyPart(sample, explain, continuous_output);
			var classes = (explain>0? classesWithExplanation.classes: classesWithExplanation);
			var scores =  (continuous_output? classesWithExplanation.scores: null)
			var explanations = (explain>0? classesWithExplanation.explanation: null);
		} else {
			var parts = this.inputSplitter(sample);
			// var accumulatedClasses = {};
			var accumulatedClasses = [];
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.correctFeatureSpelling"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>correctFeatureSpelling (sample)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.correctFeatureSpelling)
- description and source-code
```javascript
correctFeatureSpelling = function (sample) {
		if (this.spellChecker) {
			var features = this.tokenizer.tokenize(sample);
			for (var index in features) {
				var feature = features[index]
				if (!isNaN(parseInt(feature)))  // don't spell-correct numeric features
					{
					continue
					}
				
				if (!(this.spellChecker[1].exists(feature)))
					{
						if (this.spellChecker[1].suggest(feature).length != 0)
							{
							features[index] = this.spellChecker[1].suggest(feature)[0]
							}
						else
							{
								if (!(this.spellChecker[0].exists(feature)))
									{
										if (this.spellChecker[0].suggest(feature).length != 0)
											{
											features[index] = this.spellChecker[0].suggest(feature)[0]
											
											}
									}
							}
					}
			}
		sample = features.join(" ")
		}
		return sample
	}
```
- example usage
```shell
...
	/**
	 * internal function - classify a single segment of the input (used mainly when there is an inputSplitter)
	 * @param sample a document.
	 * @return an array whose VALUES are classes.
	 */
	classifyPart: function(sample, explain, continuous_output) {
		
		var samplecorrected = this.correctFeatureSpelling(sample);
		var features = this.sampleToFeatures(samplecorrected, this.featureExtractors);
		this.editFeatureValues(features, /*remove_unknown_features=*/true);
		var array = this.featuresToArray(features);
		var classification = this.classifier.classify(array, explain, continuous_output);
		
		// if (this.spellChecker && classification.explanation) {
			// if (Array.isArray(classification.explanation))
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.countFeatures"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>countFeatures (features)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.countFeatures)
- description and source-code
```javascript
countFeatures = function (features) {
		if (this.featureDocumentFrequency) {
			// this.tfidf.addDocument(datum.input);
			for (var feature in features)
				this.featureDocumentFrequency[feature] = (this.featureDocumentFrequency[feature] || 0)+1;
			this.documentCount = (this.documentCount||0)+1;
		}
	}
```
- example usage
```shell
...
	 * @param sample a document.
	 * @param classes an array whose VALUES are classes.
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
	},
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.editFeatureValues"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>editFeatureValues (features, remove_unknown_features)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.editFeatureValues)
- description and source-code
```javascript
editFeatureValues = function (features, remove_unknown_features) {

		if (this.multiplyFeaturesByIDF) {
			for (var feature in features) {
				var IDF = this.tfidf.idf(feature)
				if (IDF != Infinity)
					features[feature] *= IDF
				else
					delete features[feature]
			}

			if (this.bias && !features.bias)
			features.bias = this.bias;

		}
		// if (remove_unknown_features && this.minFeatureDocumentFrequency>0)
			// for (var feature in features)
				// if ((this.featureDocumentFrequency[feature]||0)<this.minFeatureDocumentFrequency)
					// delete features[feature];
		
	}
```
- example usage
```shell
...
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
	},

	/**
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.featuresToArray"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>featuresToArray (features)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.featuresToArray)
- description and source-code
```javascript
featuresToArray = function (features) {
		var array = features;
		if (this.featureLookupTable) {
			array = this.featureLookupTable.hashToArray(features);
		}
		return array;
	}
```
- example usage
```shell
...
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
	},

	/**
	 * Batch training:
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
		}
		if (this.spellChecker) this.spellChecker = json.spellChecker;
		if (this.pastTrainingSamples) this.pastTrainingSamples = json.pastTrainingSamples;
		this.featureDocumentFrequency = json.featureDocumentFrequency;
		this.documentCount = json.documentCount;
		/* Note: the feature extractors are functions - they should be created at initialization - they are not deserializable! */
	}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.getAllClasses"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.getAllClasses)
- description and source-code
```javascript
getAllClasses = function () {  // relevant for multilabel classifiers
		return this.classifier.getAllClasses();
	}
```
- example usage
```shell
...
		if (this.pastTrainingSamples) this.pastTrainingSamples = json.pastTrainingSamples;
		this.featureDocumentFrequency = json.featureDocumentFrequency;
		this.documentCount = json.documentCount;
		/* Note: the feature extractors are functions - they should be created at initialization - they are not deserializable! */
	},

	getAllClasses: function() {  // relevant for multilabel classifiers
		return this.classifier.getAllClasses();
	},
}  // end of EnhancedClassifier prototype


var stringifyClass = function (aClass) {
	return (_(aClass).isString()? aClass: JSON.stringify(aClass));
}
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.instanceFilter"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>instanceFilter (data)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.instanceFilter)
- description and source-code
```javascript
instanceFilter = function (data) {
		if (this.instanceFilterRule)
			return this.instanceFilterRule(data)
	}
```
- example usage
```shell
...
				if (pastTrainingSamples && dataset!=pastTrainingSamples)
					pastTrainingSamples.push(datum);
				datum = _(datum).clone();

				datum.input = this.normalizedSample(datum.input);

				/*true - this instance is filtered as not useful*/
				if (this.instanceFilter(datum) == true)
					return null

				this.trainSpellChecker(datum.input);

				var features = this.sampleToFeatures(datum.input, this.featureExtractors);
				
				if (this.tfidf)
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.normalizedSample"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>normalizedSample (sample)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.normalizedSample)
- description and source-code
```javascript
normalizedSample = function (sample) {
		if (!(_.isArray(sample)))
		{
			if (this.normalizers) {
				try {
					for (var i in this.normalizers) {					
						sample = this.normalizers[i](sample);
					}
				} catch (err) {
					console.log(err)
					throw new Error("Cannot normalize '"+sample+"': "+JSON.stringify(err));
				}
			}
		}

		return sample;
	}
```
- example usage
```shell
...
	 * Online training:
	 * Tell the classifier that the given sample belongs to the given classes.
	 * @param sample a document.
	 * @param classes an array whose VALUES are classes.
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.outputToFormat"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>outputToFormat (data)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.outputToFormat)
- description and source-code
```javascript
outputToFormat = function (data) {
		dataset = util.clonedataset(data)
		dataset = dataset.map(function(datum) {
		var normalizedLabels = multilabelutils.normalizeOutputLabels(datum.output);
		return {
			input: datum.input,
			output: this.TestSplitLabel(normalizedLabels)
		}
		}, this);
		return dataset
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.retrain"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>retrain ()](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.retrain)
- description and source-code
```javascript
retrain = function () {
		if (!this.pastTrainingSamples)
			throw new Error("No pastTrainingSamples array - can't retrain");
		
		this.trainBatch(this.pastTrainingSamples);
	}
```
- example usage
```shell
...
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
var intentClassifierString = serialize.toString(intentClassifier, newClassifierFunction);

// Save the string to a file, and send it to a remote server.
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.sampleToFeatures"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>sampleToFeatures (sample, featureExtractor)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.sampleToFeatures)
- description and source-code
```javascript
sampleToFeatures = function (sample, featureExtractor) {
		var features = sample;
		if (featureExtractor) {
			try {
				features = {};
				featureExtractor(sample, features);
			} catch (err) {
				throw new Error("Cannot extract features from '"+sample+"': "+JSON.stringify(err));
			}
		}

		return features;
	}
```
- example usage
```shell
...
	 * Tell the classifier that the given sample belongs to the given classes.
	 * @param sample a document.
	 * @param classes an array whose VALUES are classes.
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.setFeatureExtractor"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>setFeatureExtractor (featureExtractor)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.setFeatureExtractor)
- description and source-code
```javascript
setFeatureExtractor = function (featureExtractor) {
		this.featureExtractors = ftrs.normalize(featureExtractor);
	}
```
- example usage
```shell
...
		throw new Error("opts must contain classifierType");
	}

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.setFeatureExtractorForClassification"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>setFeatureExtractorForClassification (featureExtractorForClassification)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.setFeatureExtractorForClassification)
- description and source-code
```javascript
setFeatureExtractorForClassification = function (featureExtractorForClassification) {
		if (featureExtractorForClassification) {
			if (Array.isArray(featureExtractorForClassification)) {
				featureExtractorForClassification.unshift(this.featureExtractors);
			} else {
				featureExtractorForClassification = [this.featureExtractors, featureExtractorForClassification];
			}
			this.featureExtractorsForClassification = new ftrs.CollectionOfExtractors(featureExtractorForClassification);
		}
	}
```
- example usage
```shell
...
	}

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.setFeatureLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.setFeatureLookupTable)
- description and source-code
```javascript
setFeatureLookupTable = function (featureLookupTable) {
		if (featureLookupTable) {
			this.featureLookupTable = featureLookupTable;
			if (this.classifier.setFeatureLookupTable)
				this.classifier.setFeatureLookupTable(featureLookupTable);  // for generating clearer explanations only
		}
	}
```
- example usage
```shell
...

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
	this.tfidf = new opts.TfIdfImpl
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.setLabelLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>setLabelLookupTable (labelLookupTable)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.setLabelLookupTable)
- description and source-code
```javascript
setLabelLookupTable = function (labelLookupTable) {
		if (labelLookupTable) {
			this.labelLookupTable = labelLookupTable;
			if (this.classifier.setLabelLookupTable)
				this.classifier.setLabelLookupTable(labelLookupTable);  // for generating clearer explanations only
		}
	}
```
- example usage
```shell
...
	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
    	this.tfidf = new opts.TfIdfImpl
		this.featureDocumentFrequency = {};
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.setNormalizer"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>setNormalizer (normalizer)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.setNormalizer)
- description and source-code
```javascript
setNormalizer = function (normalizer) {
		if (normalizer)
			this.normalizers = (Array.isArray(normalizer)? normalizer: [normalizer]);
	}
```
- example usage
```shell
...
		console.dir(opts);
		throw new Error("opts must contain classifierType");
	}

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>toJSON (callback)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.toJSON)
- description and source-code
```javascript
toJSON = function (callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
		var featureLookupTable = this.featureLookupTable;
		var pastTrainingSamples = this.pastTrainingSamples;

			if (this.spellChecker) {
				// var seeds = fs.readFileSync('./node_modules/wordsworth/data/seed.txt')
				// var trainings = fs.readFileSync('./node_modules/wordsworth/data/training.txt')
				var seeds = []
				var trainings = []
				this.spellChecker[0].initializeSync(seeds.toString().split("\r\n"), trainings.toString().split("\r\n"))
				}

			dataset = dataset.map(function(datum) {

				if (typeof this.InputSplitLabel === 'function') {
					datum.output = (this.InputSplitLabel(multilabelutils.normalizeOutputLabels(datum.output)))	
				}
				else
				{
					datum.output = normalizeClasses(datum.output, this.labelLookupTable);
				}

				if (pastTrainingSamples && dataset!=pastTrainingSamples)
					pastTrainingSamples.push(datum);
				datum = _(datum).clone();

				datum.input = this.normalizedSample(datum.input);

				<span class="apidocCodeCommentSpan">/*true - this instance is filtered as not useful*/
</span>				if (this.instanceFilter(datum) == true)
					return null

				this.trainSpellChecker(datum.input);

				var features = this.sampleToFeatures(datum.input, this.featureExtractors);
				
				if (this.tfidf)
					this.tfidf.addDocument(features);
				// this.trainSpellChecker(features);
				if (featureLookupTable)
					featureLookupTable.addFeatures(features);

				datum.input = features;
				return datum;
			}, this);

			dataset = _.compact(dataset)

		dataset.forEach(function(datum) {
			// run on single sentence
			this.editFeatureValues(datum.input, /*remove_unknown_features=*/false);
			if (featureLookupTable)
				datum.input = featureLookupTable.hashToArray(datum.input);
		}, this);

		this.classifier.trainBatch(dataset);
	}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>trainOnline (sample, classes)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
	}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```

#### <a name="apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.trainSpellChecker"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.EnhancedClassifier.prototype.</span>trainSpellChecker (features)](#apidoc.element.limdu.classifiers.EnhancedClassifier.prototype.trainSpellChecker)
- description and source-code
```javascript
trainSpellChecker = function (features) {
		if (this.spellChecker) {
			var tokens = this.tokenizer.tokenize(features);
			_.each(tokens, function(word, key, list){
				this.spellChecker[1].understand(word); // Adds the given word to the index of the spell-checker.
				this.spellChecker[1].train(word);
			}, this)
		}
	}
```
- example usage
```shell
...
	 * @param classes an array whose VALUES are classes.
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
	},
...
```



# <a name="apidoc.module.limdu.classifiers.NeuralNetwork"></a>[module limdu.classifiers.NeuralNetwork](#apidoc.module.limdu.classifiers.NeuralNetwork)

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.NeuralNetwork"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>NeuralNetwork (options)](#apidoc.element.limdu.classifiers.NeuralNetwork.NeuralNetwork)
- description and source-code
```javascript
NeuralNetwork = function (options) {
  options = options || {};
  this.learningRate = options.learningRate || 0.3;
  this.momentum = options.momentum || 0.1;
  this.hiddenSizes = options.hiddenLayers;

  this.binaryThresh = options.binaryThresh || 0.5;
}
```
- example usage
```shell
...
## Binary Classification

### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);
...
```



# <a name="apidoc.module.limdu.classifiers.NeuralNetwork.prototype"></a>[module limdu.classifiers.NeuralNetwork.prototype](#apidoc.module.limdu.classifiers.NeuralNetwork.prototype)

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.prototype.adjustWeights"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>adjustWeights (learningRate)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.adjustWeights)
- description and source-code
```javascript
adjustWeights = function (learningRate) {
  for (var layer = 1; layer <= this.outputLayer; layer++) {
    var incoming = this.outputs[layer - 1];

    for (var node = 0; node < this.sizes[layer]; node++) {
      var delta = this.deltas[layer][node];

      for (var k = 0; k < incoming.length; k++) {
        var change = this.changes[layer][node][k];

        change = (learningRate * delta * incoming[k])
                 + (this.momentum * change);

        this.changes[layer][node][k] = change;
        this.weights[layer][node][k] += change;
      }
      this.biases[layer][node] += learningRate * delta;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.prototype.calculateDeltas"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>calculateDeltas (target)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.calculateDeltas)
- description and source-code
```javascript
calculateDeltas = function (target) {
  for (var layer = this.outputLayer; layer >= 0; layer--) {
    for (var node = 0; node < this.sizes[layer]; node++) {
      var output = this.outputs[layer][node];

      var error = 0;
      if (layer == this.outputLayer) {
        error = target[node] - output;
      }
      else {
        var deltas = this.deltas[layer + 1];
        for (var k = 0; k < deltas.length; k++) {
          error += deltas[k] * this.weights[layer + 1][k][node];
        }
      }
      this.errors[layer][node] = error;
      this.deltas[layer][node] = error * output * (1 - output);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>classify (input)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.classify)
- description and source-code
```javascript
classify = function (input) {
  if (this.inputLookup) {
    input = lookup.toArray(this.inputLookup, input);
  }

  var output = this.runInput(input);

  if (this.outputLookup) {
    output = lookup.toHash(this.outputLookup, output);
  }
  return output;
}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.prototype.createTrainStream"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>createTrainStream (opts)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.createTrainStream)
- description and source-code
```javascript
createTrainStream = function (opts) {
  opts = opts || {};
  opts.neuralNetwork = this;
  this.trainStream = new TrainStream(opts);
  return this.trainStream;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.prototype.formatData"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>formatData (data)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.formatData)
- description and source-code
```javascript
formatData = function (data) {
  if (!_.isArray(data)) { // turn stream datum into array
    var tmp = [];
    tmp.push(data);
    data = tmp;
  }
  // turn sparse hash input into arrays with 0s as filler
  var datum = data[0].input;
  if (!_(datum).isArray() && !(datum instanceof Float64Array)) {
    if (!this.inputLookup) {
      this.inputLookup = lookup.buildLookup(_(data).pluck("input"));
    }
    data = data.map(function(datum) {
      var array = lookup.toArray(this.inputLookup, datum.input)
      return _(_(datum).clone()).extend({ input: array });
    }, this);
  }

  if (!_(data[0].output).isArray()) {
    if (!this.outputLookup) {
      this.outputLookup = lookup.buildLookup(_(data).pluck("output"));
    }
    data = data.map(function(datum) {
      var array = lookup.toArray(this.outputLookup, datum.output);
      return _(_(datum).clone()).extend({ output: array });
    }, this);
  }
  return data;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
  var size = json.layers.length;
  this.outputLayer = size - 1;

  this.sizes = new Array(size);
  this.weights = new Array(size);
  this.biases = new Array(size);
  this.outputs = new Array(size);

  for (var i = 0; i <= this.outputLayer; i++) {
    var layer = json.layers[i];
    if (i == 0 && (!layer[0] || json.inputLookup)) {
      this.inputLookup = lookup.lookupFromHash(layer);
    }
    else if (i == this.outputLayer && (!layer[0] || json.outputLookup)) {
      this.outputLookup = lookup.lookupFromHash(layer);
    }

    var nodes = _(layer).keys();
    this.sizes[i] = nodes.length;
    this.weights[i] = [];
    this.biases[i] = [];
    this.outputs[i] = [];

    for (var j in nodes) {
      var node = nodes[j];
      this.biases[i][j] = layer[node].bias;
      this.weights[i][j] = _(layer[node].weights).toArray();
    }
  }
  return this;
}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.prototype.initialize"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>initialize (sizes)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.initialize)
- description and source-code
```javascript
initialize = function (sizes) {
  this.sizes = sizes;
  this.outputLayer = this.sizes.length - 1;

  this.biases = []; // weights for bias nodes
  this.weights = [];
  this.outputs = [];

  // state for training
  this.deltas = [];
  this.changes = []; // for momentum
  this.errors = [];

  for (var layer = 0; layer <= this.outputLayer; layer++) {
    var size = this.sizes[layer];
    this.deltas[layer] = zeros(size);
    this.errors[layer] = zeros(size);
    this.outputs[layer] = zeros(size);

    if (layer > 0) {
      this.biases[layer] = randos(size);
      this.weights[layer] = new Array(size);
      this.changes[layer] = new Array(size);

      for (var node = 0; node < size; node++) {
        var prevSize = this.sizes[layer - 1];
        this.weights[layer][node] = randos(prevSize);
        this.changes[layer][node] = zeros(prevSize);
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.prototype.run"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>run (input)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.run)
- description and source-code
```javascript
run = function (input) {
  if (this.inputLookup) {
    input = lookup.toArray(this.inputLookup, input);
  }

  var output = this.runInput(input);

  if (this.outputLookup) {
    output = lookup.toHash(this.outputLookup, output);
  }
  return output;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.prototype.runInput"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>runInput (input)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.runInput)
- description and source-code
```javascript
runInput = function (input) {
  this.outputs[0] = input;  // set output state of input layer

  for (var layer = 1; layer <= this.outputLayer; layer++) {
    for (var node = 0; node < this.sizes[layer]; node++) {
      var weights = this.weights[layer][node];

      var sum = this.biases[layer][node];
      for (var k = 0; k < weights.length; k++) {
        sum += weights[k] * input[k];
      }
      this.outputs[layer][node] = 1 / (1 + Math.exp(-sum));
    }
    var output = input = this.outputs[layer];
  }
  return output;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.prototype.test"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>test (data)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.test)
- description and source-code
```javascript
test = function (data) {
  data = this.formatData(data);

  // for binary classification problems with one output node
  var isBinary = data[0].output.length == 1;
  var falsePos = 0,
      falseNeg = 0,
      truePos = 0,
      trueNeg = 0;

  // for classification problems
  var misclasses = [];

  // run each pattern through the trained network and collect
  // error and misclassification statistics
  var sum = 0;
  for (var i = 0; i < data.length; i++) {
    var output = this.runInput(data[i].input);
    var target = data[i].output;

    var actual, expected;
    if (isBinary) {
      actual = output[0] > this.binaryThresh ? 1 : 0;
      expected = target[0];
    }
    else {
      actual = output.indexOf(_(output).max());
      expected = target.indexOf(_(target).max());
    }

    if (actual != expected) {
      var misclass = data[i];
      _(misclass).extend({
        actual: actual,
        expected: expected
      })
      misclasses.push(misclass);
    }

    if (isBinary) {
      if (actual == 0 && expected == 0) {
        trueNeg++;
      }
      else if (actual == 1 && expected == 1) {
        truePos++;
      }
      else if (actual == 0 && expected == 1) {
        falseNeg++;
      }
      else if (actual == 1 && expected == 0) {
        falsePos++;
      }
    }

    var errors = output.map(function(value, i) {
      return target[i] - value;
    });
    sum += mse(errors);
  }
  var error = sum / data.length;

  var stats = {
    error: error,
    misclasses: misclasses
  };

  if (isBinary) {
    _(stats).extend({
      trueNeg: trueNeg,
      truePos: truePos,
      falseNeg: falseNeg,
      falsePos: falsePos,
      total: data.length,
      precision: truePos / (truePos + falsePos),
      recall: truePos / (truePos + falseNeg),
      accuracy: (trueNeg + truePos) / data.length
    })
  }
  return stats;
}
```
- example usage
```shell
...
var microAverage = new limdu.utils.PrecisionRecall();
var macroAverage = new limdu.utils.PrecisionRecall();

limdu.utils.partitions.partitions(dataset, numOfFolds, function(trainSet, testSet) {
	console.log("Training on "+trainSet.length+" samples, testing on "+testSet.length+" samples");
	var classifier = new IntentClassifier();
	classifier.trainBatch(trainSet);
	limdu.utils.test(classifier, testSet, /* verbosity = */0,
		microAverage, macroAverage);
});

macroAverage.calculateMacroAverageStats(numOfFolds);
console.log("\n\nMACRO AVERAGE:"); console.dir(macroAverage.fullStats());

microAverage.calculateStats();
...
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.prototype.toFunction"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>toFunction ()](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.toFunction)
- description and source-code
```javascript
toFunction = function () {
  var json = this.toJSON();
  // return standalone function that mimics run()
  return new Function("input",
'  var net = ' + JSON.stringify(json) + ';\n\n\
for (var i = 1; i < net.layers.length; i++) {\n\
  var layer = net.layers[i];\n\
  var output = {};\n\
  \n\
  for (var id in layer) {\n\
    var node = layer[id];\n\
    var sum = node.bias;\n\
    \n\
    for (var iid in node.weights) {\n\
      sum += node.weights[iid] * input[iid];\n\
    }\n\
    output[id] = (1 / (1 + Math.exp(-sum)));\n\
  }\n\
  input = output;\n\
}\n\
return output;');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
<span class="apidocCodeCommentSpan">  /* make json look like:
    {
      layers: [
        { x: {},
          y: {}},
        {'0': {bias: -0.98771313, weights: {x: 0.8374838, y: 1.245858},
         '1': {bias: 3.48192004, weights: {x: 1.7825821, y: -2.67899}}},
        { f: {bias: 0.27205739, weights: {'0': 1.3161821, '1': 2.00436}}}
      ]
    }
  */
</span>  var layers = [];
  for (var layer = 0; layer <= this.outputLayer; layer++) {
    layers[layer] = {};

    var nodes;
    // turn any internal arrays back into hashes for readable json
    if (layer == 0 && this.inputLookup) {
      nodes = _(this.inputLookup).keys();
    }
    else if (layer == this.outputLayer && this.outputLookup) {
      nodes = _(this.outputLookup).keys();
    }
    else {
      nodes = _.range(0, this.sizes[layer]);
    }

    for (var j = 0; j < nodes.length; j++) {
      var node = nodes[j];
      layers[layer][node] = {};

      if (layer > 0) {
        layers[layer][node].bias = this.biases[layer][j];
        layers[layer][node].weights = {};
        for (var k in layers[layer - 1]) {
          var index = k;
          if (layer == 1 && this.inputLookup) {
            index = this.inputLookup[k];
          }
          layers[layer][node].weights[k] = this.weights[layer][j][index];
        }
      }
    }
  }
  return { layers: layers, outputLookup:!!this.outputLookup, inputLookup:!!this.inputLookup };
}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.prototype.train"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>train (data, options)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.train)
- description and source-code
```javascript
train = function (data, options) {
  data = this.formatData(data);

  options = options || {};
  var iterations = options.iterations || 20000;
  var errorThresh = options.errorThresh || 0.005;
  var log = options.log || false;
  var logPeriod = options.logPeriod || 10;
  var learningRate = options.learningRate || this.learningRate || 0.3;
  var callback = options.callback;
  var callbackPeriod = options.callbackPeriod || 10;

  var inputSize = data[0].input.length;
  var outputSize = data[0].output.length;

  var hiddenSizes = this.hiddenSizes;
  if (!hiddenSizes) {
    hiddenSizes = [Math.max(3, Math.floor(inputSize / 2))];
  }
  var sizes = _([inputSize, hiddenSizes, outputSize]).flatten();
  this.initialize(sizes);

  var error = 1;
  for (var i = 0; i < iterations && error > errorThresh; i++) {
    var sum = 0;
    for (var j = 0; j < data.length; j++) {
      var err = this.trainPattern(data[j].input, data[j].output, learningRate);
      sum += err;
    }
    error = sum / data.length;

    if (log && (i % logPeriod == 0)) {
      console.log("iterations:", i, "training error:", error);
    }
    if (callback && (i % callbackPeriod == 0)) {
      callback({ error: error, iterations: i });
    }
  }

  return {
    error: error,
    iterations: i
  };
}
```
- example usage
```shell
...
	},
	
	trainSpellChecker: function(features) {
		if (this.spellChecker) {
			var tokens = this.tokenizer.tokenize(features);
			_.each(tokens, function(word, key, list){
				this.spellChecker[1].understand(word); // Adds the given word to the index of the spell-checker.
				this.spellChecker[1].train(word);
			}, this)
		}
	},
	
	correctFeatureSpelling: function(sample) {
		if (this.spellChecker) {
			var features = this.tokenizer.tokenize(sample);
...
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
	dataset.forEach(function(datum) {
		if (!Array.isArray(datum.output) && !(datum.output instanceof Object))
			datum.output = [datum.output];
	});
	this.train(dataset);
}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>trainOnline ()](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function () {throw new Error("NeuralNetwork does not support online training");}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```

#### <a name="apidoc.element.limdu.classifiers.NeuralNetwork.prototype.trainPattern"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.NeuralNetwork.prototype.</span>trainPattern (input, target, learningRate)](#apidoc.element.limdu.classifiers.NeuralNetwork.prototype.trainPattern)
- description and source-code
```javascript
trainPattern = function (input, target, learningRate) {
  learningRate = learningRate || this.learningRate;

  // forward propogate
  this.runInput(input);

  // back propogate
  this.calculateDeltas(target);
  this.adjustWeights(learningRate);

  var error = mse(this.errors[this.outputLayer]);
  return error;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.classifiers.Perceptron"></a>[module limdu.classifiers.Perceptron](#apidoc.module.limdu.classifiers.Perceptron)

#### <a name="apidoc.element.limdu.classifiers.Perceptron.Perceptron"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>Perceptron (opts)](#apidoc.element.limdu.classifiers.Perceptron.Perceptron)
- description and source-code
```javascript
Perceptron = function (opts) {
	if (!opts) opts = {};
	
	this.debug = opts.debug||false;
	this.default_weight = opts.default_weight||0;
	this.do_averaging = opts.do_averaging||false;
	this.do_normalization = opts.do_normalization||false;
	this.learning_rate = opts.learning_rate||0.1;
	this.retrain_count = 'retrain_count' in opts? opts.retrain_count: 1;
	
	this.weights = {};
	if (this.do_averaging) this.weights_sum = {};   // for averaging; see http://ciml.info/dl/v0_8/ciml-v0_8-ch03.pdf . But count only
 weight vectors with successful predictions (Carvalho and Cohen, 2006).
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.classifiers.Perceptron.prototype"></a>[module limdu.classifiers.Perceptron.prototype](#apidoc.module.limdu.classifiers.Perceptron.prototype)

#### <a name="apidoc.element.limdu.classifiers.Perceptron.prototype.adjust"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>adjust (result, expected, input, feature)](#apidoc.element.limdu.classifiers.Perceptron.prototype.adjust)
- description and source-code
```javascript
adjust = function (result, expected, input, feature) {
		var delta = (expected - result) * this.learning_rate * input;
		if (isNaN(delta)) throw new Error('delta is NaN!! result='+result+" expected="+expected+" input="+input+" feature="+feature);
		this.weights[feature] += delta;
		if (isNaN(this.weights[feature])) throw new Error('weights['+feature+'] went to NaN!! delta='+d);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.Perceptron.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>classify (features, explain, continuous_output)](#apidoc.element.limdu.classifiers.Perceptron.prototype.classify)
- description and source-code
```javascript
classify = function (features, explain, continuous_output) {
		return this.perceive_features(
			this.normalized_features(features, /*remove_unknown_features=*/true),
			continuous_output,
			(this.do_averaging? this.weights_sum: this.weights),
			explain);
	}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.Perceptron.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.Perceptron.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.Perceptron.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.Perceptron.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
		this.weights = json.weights;
		this.weights_sum = json.weights_sum;
	}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.Perceptron.prototype.normalized_features"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>normalized_features (features, remove_unknown_features)](#apidoc.element.limdu.classifiers.Perceptron.prototype.normalized_features)
- description and source-code
```javascript
normalized_features = function (features, remove_unknown_features) {
		features['bias'] = 1;
		if (remove_unknown_features) {
			for (var feature in features)
				if (!(feature in this.weights))
					delete features[feature];
		}
		if (this.do_normalization)
			hash.normalize_sum_of_values_to_1(features);
		return features;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.Perceptron.prototype.perceive_features"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>perceive_features (features, continuous_output, weights_for_classification, explain)](#apidoc.element.limdu.classifiers.Perceptron.prototype.perceive_features)
- description and source-code
```javascript
perceive_features = function (features, continuous_output, weights_for_classification, explain) {
		var score = hash.inner_product(features, weights_for_classification);
		if (this.debug) console.log("> perceive_features ",features," = ",score);
		var result = (continuous_output? score: (score > 0 ? 1 : 0));
		if (explain) {
			result = {
				classification: result,
				explanation: ["Perceptron does not support explanations yet"],
				net_score: score,
			}
		}
		return result;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.Perceptron.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.Perceptron.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
		return {
			weights: this.weights,
			weights_sum: this.weights_sum
		}
	}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.Perceptron.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.Perceptron.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
		var normalized_features = [];
		for (var i=0; i<dataset.length; ++i)
			normalized_features[i] = this.normalized_features(dataset[i].input, /*remove_unknown_features=*/false);

		for (var r=0; r<=this.retrain_count; ++r)
			for (var i=0; i<normalized_features.length; ++i)
				this.train_features(normalized_features[i], dataset[i].output);
	}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.Perceptron.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>trainOnline (features, expected)](#apidoc.element.limdu.classifiers.Perceptron.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (features, expected) {
		return this.train_features(
			this.normalized_features(features, /*remove_unknown_features=*/false), expected);
	}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```

#### <a name="apidoc.element.limdu.classifiers.Perceptron.prototype.train_features"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Perceptron.prototype.</span>train_features (features, expected)](#apidoc.element.limdu.classifiers.Perceptron.prototype.train_features)
- description and source-code
```javascript
train_features = function (features, expected) {
		for (feature in features)
			if (!(feature in this.weights))
				this.weights[feature] = this.default_weight;

		var result = this.perceive_features(features, /*net=*/false, this.weights); // always use the running 'weights' vector for training
, and NOT the weights_sum!

		if (this.debug) console.log('> training ',features,', expecting: ',expected, ' got: ', result);

		if (result != expected) {
			// Current model is incorrect - adjustment needed!
			if (this.debug) console.log('> adjusting weights...', this.weights, features);
			for (var feature in features)
				this.adjust(result, expected, features[feature], feature);
			if (this.debug) console.log(' -> weights:', this.weights)
		} else {
			if (this.do_averaging) hash.add(this.weights_sum, this.weights);
		}
		
		return (result == expected);
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.classifiers.SvmJs"></a>[module limdu.classifiers.SvmJs](#apidoc.module.limdu.classifiers.SvmJs)

#### <a name="apidoc.element.limdu.classifiers.SvmJs.SvmJs"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>SvmJs (opts)](#apidoc.element.limdu.classifiers.SvmJs.SvmJs)
- description and source-code
```javascript
function SvmJs(opts) {
	this.base = new SvmJsBase();
	this.opts = opts;  // options for SvmJsBase.train
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.classifiers.SvmJs.prototype"></a>[module limdu.classifiers.SvmJs.prototype](#apidoc.module.limdu.classifiers.SvmJs.prototype)

#### <a name="apidoc.element.limdu.classifiers.SvmJs.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmJs.prototype.</span>classify (features, explain, continuous_output)](#apidoc.element.limdu.classifiers.SvmJs.prototype.classify)
- description and source-code
```javascript
classify = function (features, explain, continuous_output) {
	var score = this.base.marginOne(features);
	var classification = continuous_output? score: (score>0? 1: 0);
	
	if (explain>0) {
        var f = this.base.b;

        // if the linear kernel was used and w was computed and stored,
        // (i.e. the svm has fully finished training)
        // the internal class variable usew_ will be set to true.
        var explanations = [];
        if(this.base.usew_) {
          var w = this.base.w;
          for(var j=0;j<this.base.D;j++) {
        	explanations[j] = {
        		feature: j,
        		value: features[j],
        		weight: w[j],
        		relevance: features[j] * w[j],
        	};
          }
        } else {
        	// explanations not supported.
            //for(var i=0;i<this.N;i++) {
            // f += this.alpha[i] * this.labels[i] * this.kernel(inst, this.data[i]);
            //}
        }
        explanations.sort(function(a,b){return b.relevance-a.relevance});
        return {
        	classification: classification,
        	explanation: explanations.slice(0, explain),
        }
	} else {
		return classification;
	}
}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmJs.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmJs.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.SvmJs.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmJs.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmJs.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.SvmJs.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
	this.base.fromJSON(json);
}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmJs.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmJs.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.SvmJs.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
	return this.base.toJSON();
}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmJs.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmJs.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.SvmJs.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
		var data = [];
		var labels = [];
		dataset.forEach(function(datum) {
			data.push(datum.input);
			labels.push(datum.output>0? 1: -1);
		});
		return this.base.train(data, labels, this.opts);
	}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmJs.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmJs.prototype.</span>trainOnline (features, label)](#apidoc.element.limdu.classifiers.SvmJs.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (features, label) {
		throw new Error("svm.js does not support online training");
	}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```



# <a name="apidoc.module.limdu.classifiers.SvmLinear"></a>[module limdu.classifiers.SvmLinear](#apidoc.module.limdu.classifiers.SvmLinear)

#### <a name="apidoc.element.limdu.classifiers.SvmLinear.SvmLinear"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>SvmLinear (opts)](#apidoc.element.limdu.classifiers.SvmLinear.SvmLinear)
- description and source-code
```javascript
function SvmLinear(opts) {
	this.learn_args = opts.learn_args || "";
	this.model_file_prefix = opts.model_file_prefix || null;
	this.bias = opts.bias || 1.0;
	this.multiclass = opts.multiclass || false;
	this.debug = opts.debug||false;
	this.train_command = opts.train_command || 'liblinear_train';
	this.test_command = opts.test_command || 'liblinear_test';
	this.timestamp = ""

	if (!SvmLinear.isInstalled()) {
                var msg = "Cannot find the executable 'liblinear_train'. Please download it from the LibLinear website, and put
a link to it in your path.";
                console.error(msg)
                throw new Error(msg);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.SvmLinear.isInstalled"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.</span>isInstalled ()](#apidoc.element.limdu.classifiers.SvmLinear.isInstalled)
- description and source-code
```javascript
isInstalled = function () {
	try {
	    var result = child_process.execSync('liblinear_train');
	} catch (err) {
	    return false
	}
	return true
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.classifiers.SvmLinear.prototype"></a>[module limdu.classifiers.SvmLinear.prototype](#apidoc.module.limdu.classifiers.SvmLinear.prototype)

#### <a name="apidoc.element.limdu.classifiers.SvmLinear.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>classify (features, explain, continuous_output)](#apidoc.element.limdu.classifiers.SvmLinear.prototype.classify)
- description and source-code
```javascript
classify = function (features, explain, continuous_output) {

			if (!this.mapLabelToMapFeatureToWeight)
				this.setModel(this.modelFileString)

			if (this.allLabels.length==1) {  // a single label
				var result = (
						!continuous_output?   this.allLabels[0]:
							!this.multiclass? 1.0:
							                  [[this.allLabels[0], 1.0]]);
				return (explain>0?
						{
							classes: result,
							explanation: ["Single label ("+result+") - no classification needed"],
						}:
						result);
			}
			var labels = [];
			if (explain>0) var explanations = [];
			for (var label in this.mapLabelToMapFeatureToWeight) {
				var mapFeatureToWeight = this.mapLabelToMapFeatureToWeight[label];

				var scoreWithExplain = svmcommon.classifyWithModelMap(
					mapFeatureToWeight, this.bias, features, explain, /*continuous_output=*/true, this.featureLookupTable);

				var score = (explain>0? scoreWithExplain.classification: scoreWithExplain);

				var labelAndScore = [parseInt(label), score];
				if (scoreWithExplain.explanation && explain>0) {
					labelAndScore.push(this.multiclass?
						scoreWithExplain.explanation.join(" "):
						scoreWithExplain.explanation)
				}

				labels.push(labelAndScore);
			}

			labels.sort(function(a,b) {return b[1]-a[1]}); // sort by decreasing score

			if (explain>0) {
				if (this.multiclass) {
					var explanations = [];
					labels.forEach(function(datum) {
						explanations.push(datum[0]+": score="+JSON.stringify(datum[1])+" features="+datum[2]);
						datum.pop();
					});
				} else {
					var explanations = (labels[0][0]>0? labels[0][2]: labels[1][2])
				}
			}

			var result = (
				!continuous_output?   labels[0][0]:
					!this.multiclass? (labels[0][0]>0? labels[0][1]: labels[1][1]):
					                  labels);
			return (explain>0?
				{
					classes: result,
					classification: result,
					explanation: explanations,
				}:
				result);
		}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmLinear.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.SvmLinear.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmLinear.prototype.classifyBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>classifyBatch (trainset)](#apidoc.element.limdu.classifiers.SvmLinear.prototype.classifyBatch)
- description and source-code
```javascript
classifyBatch = function (trainset) {

			// console.log(JSON.stringify(this.modelFileString, null, 4))
			_.each(trainset, function(value, key, list){
				trainset[key].output = 0
			}, this)

			var testFile = svmcommon.writeDatasetToFile(
                                        trainset, this.bias, /*binarize=*/false, "/tmp/test_"+this.timestamp, "SvmLinear", FIRST_FEATURE_NUMBER
);

			var command = this.test_command+" "+testFile + " " + this.modelFileString + " /tmp/out_" + this.timestamp;

			var output = child_process.execSync(command)
			console.log(command)

			var result = fs.readFileSync("/tmp/out_" + this.timestamp, "utf-8").split("\n")

			return result
		}
```
- example usage
```shell
...
            _.each(testSet, function(value, key, list){
                testSet[key]["input"] = this.normalizedSample(testSet[key]["input"])
                var features = this.sampleToFeatures(testSet[key]["input"], this.featureExtractors, this.stopwords);
                this.editFeatureValues(features, /*remove_unknown_features=*/false);
                var array = this.featuresToArray(features);
                testSet[key]["input"] = array
            }, this)
            return this.classifier.classifyBatch(testSet);
        },
	
	classifyPartAsync: function(sample, explain, callback) {
		this.sampleToFeaturesAsync(sample, this.featureExtractors, (function(err, results){
			this.editFeatureValues(features, /*remove_unknown_features=*/false);
			var array = this.featuresToArray(features);
			var classification = this.classifier.classify(array, explain);
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmLinear.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.SvmLinear.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
			this.mapFeatureToWeight = json;
		}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmLinear.prototype.getModelWeights"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>getModelWeights ()](#apidoc.element.limdu.classifiers.SvmLinear.prototype.getModelWeights)
- description and source-code
```javascript
getModelWeights = function () {
			if (!this.mapLabelToMapFeatureToWeight)
                                this.setModel(this.modelFileString)
			return (this.multiclass? this.mapLabelToMapFeatureToWeight: this.mapLabelToMapFeatureToWeight[1]);
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.SvmLinear.prototype.setFeatureLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.SvmLinear.prototype.setFeatureLookupTable)
- description and source-code
```javascript
setFeatureLookupTable = function (featureLookupTable) {
			this.featureLookupTable = featureLookupTable;
		}
```
- example usage
```shell
...

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
	this.tfidf = new opts.TfIdfImpl
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmLinear.prototype.setModel"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>setModel (modelFileString)](#apidoc.element.limdu.classifiers.SvmLinear.prototype.setModel)
- description and source-code
```javascript
setModel = function (modelFileString) {
			// this.modelFileString = modelFileString;
			this.modelString = fs.readFileSync(modelFileString, "utf-8")
			this.mapLabelToMapFeatureToWeight = modelStringToModelMap(this.modelString);
			this.allLabels = Object.keys(this.mapLabelToMapFeatureToWeight);
			if (this.debug) console.dir(this.mapLabelToMapFeatureToWeight);
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.SvmLinear.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.SvmLinear.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
			return this.mapFeatureToWeight;
		}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmLinear.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.SvmLinear.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
			this.timestamp = new Date().getTime()+"_"+process.pid

			// check for multilabel
			_.each(dataset, function(datum, key, list){
				if (_.isArray(datum.output))
					if (datum.output.length > 1)
					{
						console.log("Multi-label is not allowed")
						console.log(JSON.stringify(darum.output, null, 4))
						process.exit(0)
					}
            }, this)

            //  convert all arraay-like outputs to just values
			dataset = _.map(dataset, function(datum){
				if (_.isArray(datum.output))
					datum.output = datum.output[0]
				return datum });

			this.allLabels = _(dataset).map(function(datum){return datum.output});
			this.allLabels = _.uniq(_.flatten(this.allLabels))

			// dataset = _.map(dataset, function(datum){
			// 	datum.output = this.allLabels.indexOf(datum.output)
			// 	return datum });

			if (this.allLabels.length==1) // a single label
				return;
			//console.log(util.inspect(dataset,{depth:1}));
			if (this.debug) console.log("trainBatch start");
			var learnFile = svmcommon.writeDatasetToFile(
					dataset, this.bias, /*binarize=*/false, this.model_file_prefix+"_"+this.timestamp, "SvmLinear", FIRST_FEATURE_NUMBER);
			var modelFile = learnFile.replace(/[.]learn/,".model");

			var command = this.train_command+" "+this.learn_args+" "+learnFile + " "+modelFile;
			console.log("running "+command);

			var result = child_process.execSync(command);
			if (result.code>0) {
				console.dir(result);
				console.log(fs.readFileSync(learnFile, 'utf-8'));
				throw new Error("Failed to execute: "+command);
			}

			this.modelFileString = modelFile;

			if (this.debug) console.log("trainBatch end");
		}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmLinear.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmLinear.prototype.</span>trainOnline (features, expected)](#apidoc.element.limdu.classifiers.SvmLinear.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (features, expected) {
			throw new Error("LibLinear does not support online training");
		}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```



# <a name="apidoc.module.limdu.classifiers.SvmPerf"></a>[module limdu.classifiers.SvmPerf](#apidoc.module.limdu.classifiers.SvmPerf)

#### <a name="apidoc.element.limdu.classifiers.SvmPerf.SvmPerf"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>SvmPerf (opts)](#apidoc.element.limdu.classifiers.SvmPerf.SvmPerf)
- description and source-code
```javascript
function SvmPerf(opts) {
	if (!SvmPerf.isInstalled()) {
	 	var msg = "Cannot find the executable 'svm_perf_learn'. Please download it from the SvmPerf website, and put a link to it in
your path.";
	 	console.error(msg)
	 	throw new Error(msg);
	}
	this.learn_args = opts.learn_args || "";
	this.learn_args += " --b 0 ";  // we add the bias here, so we don't need SvmPerf to add it
	this.model_file_prefix = opts.model_file_prefix || null;
	this.bias = 'bias' in opts? opts.bias: 1.0;
	this.debug = opts.debug || false;
	this.ShowFeat = {}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.SvmPerf.isInstalled"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.</span>isInstalled ()](#apidoc.element.limdu.classifiers.SvmPerf.isInstalled)
- description and source-code
```javascript
isInstalled = function () {
  try {
    var result = execSync("svm_perf_learn");
  } catch (err) {
    return false;
  }
  return true
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.classifiers.SvmPerf.prototype"></a>[module limdu.classifiers.SvmPerf.prototype](#apidoc.module.limdu.classifiers.SvmPerf.prototype)

#### <a name="apidoc.element.limdu.classifiers.SvmPerf.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>classify (features, explain, continuous_output)](#apidoc.element.limdu.classifiers.SvmPerf.prototype.classify)
- description and source-code
```javascript
classify = function (features, explain, continuous_output) {
			return svmcommon.classifyWithModelMap(
					this.mapFeatureToWeight, this.bias, features, explain, continuous_output, this.featureLookupTable);
		}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmPerf.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.SvmPerf.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmPerf.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.SvmPerf.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
			this.mapFeatureToWeight = json;
		}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmPerf.prototype.getFeatures"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>getFeatures ()](#apidoc.element.limdu.classifiers.SvmPerf.prototype.getFeatures)
- description and source-code
```javascript
getFeatures = function () {
			var featlist = []
			_.each(this.mapFeatureToWeight, function(weight, index, list){
				if (parseInt(index) == 0)
					featlist.push(['bias', weight])
				else
					featlist.push([this.featureLookupTable.numberToFeature(parseInt(index)-1), weight])
			}, this)
			featlist = _.sortBy(featlist, function(num){return num[1]})
			return featlist
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.SvmPerf.prototype.getModelWeights"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>getModelWeights ()](#apidoc.element.limdu.classifiers.SvmPerf.prototype.getModelWeights)
- description and source-code
```javascript
getModelWeights = function () {
			return this.mapFeatureToWeight;
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.SvmPerf.prototype.setFeatureLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.SvmPerf.prototype.setFeatureLookupTable)
- description and source-code
```javascript
setFeatureLookupTable = function (featureLookupTable) {
			//console.log("SVMPERF setFeatureLookupTable "+featureLookupTable);
			this.featureLookupTable = featureLookupTable;
		}
```
- example usage
```shell
...

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
	this.tfidf = new opts.TfIdfImpl
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmPerf.prototype.setModel"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>setModel (modelString)](#apidoc.element.limdu.classifiers.SvmPerf.prototype.setModel)
- description and source-code
```javascript
setModel = function (modelString) {
			this.modelString = modelString;
			this.mapFeatureToWeight = modelStringToModelMap(modelString);  // weights in modelMap start from 0 (- the bias).
			if (this.debug) console.dir(this.mapFeatureToWeight);
			// console.log("maps"+JSON.stringify(_.keys(this.mapFeatureToWeight).length, null, 4))
			// process.exit(0)
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.SvmPerf.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.SvmPerf.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
			return this.mapFeatureToWeight;
		}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmPerf.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.SvmPerf.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
			if (this.debug) console.log("trainBatch start");

			var timestamp = new Date().getTime()+"_"+process.pid
			var learnFile = svmcommon.writeDatasetToFile(dataset, this.bias, /*binarize=*/true, this.model_file_prefix+"_"+timestamp, "SvmPerf
", FIRST_FEATURE_NUMBER);
			var modelFile = learnFile.replace(/[.]learn/,".model");
			var command = "svm_perf_learn "+this.learn_args+" "+learnFile + " "+modelFile;
			if (this.debug) console.log("running "+command);
			console.log(command)

			var result = execSync(command);
			if (result.code>0) {
				console.dir(result);
				console.log(fs.readFileSync(learnFile, 'utf-8'));
				throw new Error("Failed to execute: "+command);
			}

			this.setModel(fs.readFileSync(modelFile, "utf-8"));
			if (this.debug) console.log("trainBatch end");
		}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.SvmPerf.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.SvmPerf.prototype.</span>trainOnline (features, expected)](#apidoc.element.limdu.classifiers.SvmPerf.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (features, expected) {
			//throw new Error("SVM-perf does not support online training");
			console.error("SVM-perf does not support online training");
		}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```



# <a name="apidoc.module.limdu.classifiers.Winnow"></a>[module limdu.classifiers.Winnow](#apidoc.module.limdu.classifiers.Winnow)

#### <a name="apidoc.element.limdu.classifiers.Winnow.Winnow"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>Winnow (opts)](#apidoc.element.limdu.classifiers.Winnow.Winnow)
- description and source-code
```javascript
function WinnowHash(opts) {
	if (!opts) opts = {}

	this.debug = opts.debug || false;
		
	// Default values are based on Carvalho and Cohen, 2006, section 4.2:	
	this.default_positive_weight = opts.default_positive_weight || 2.0;
	this.default_negative_weight = opts.default_negative_weight || 1.0;
	this.do_averaging = opts.do_averaging || false;
	this.threshold = ('threshold' in opts? opts.threshold: 1);
	this.promotion = opts.promotion || 1.5;
	this.demotion = opts.demotion || 0.5;
	this.margin = ('margin' in opts? opts.margin: 1.0);
	this.retrain_count = opts.retrain_count || 0;
	this.detailed_explanations = opts.detailed_explanations || false;
	
	this.bias = ('bias' in opts? opts.bias: 1.0);

	this.positive_weights = {};
	this.negative_weights = {};
	this.positive_weights_sum = {};   // for averaging; count only weight vectors with successful predictions (Carvalho and Cohen,
2006).
	this.negative_weights_sum = {};   // for averaging; count only weight vectors with successful predictions (Carvalho and Cohen,
2006).
}
```
- example usage
```shell
...
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
...
```



# <a name="apidoc.module.limdu.classifiers.Winnow.prototype"></a>[module limdu.classifiers.Winnow.prototype](#apidoc.module.limdu.classifiers.Winnow.prototype)

#### <a name="apidoc.element.limdu.classifiers.Winnow.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>classify (features, explain, continuous_output)](#apidoc.element.limdu.classifiers.Winnow.prototype.classify)
- description and source-code
```javascript
classify = function (features, explain, continuous_output) {
			this.editFeatureValues(features, /*remove_unknown_features=*/true);
			return this.perceive_features(
				//this.normalized_features(features, /*remove_unknown_features=*/true),
				features,
				continuous_output,
				(this.do_averaging? this.positive_weights_sum: this.positive_weights),
				(this.do_averaging? this.negative_weights_sum: this.negative_weights),
				explain );
		}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.Winnow.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.Winnow.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.Winnow.prototype.editFeatureValues"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>editFeatureValues (features, remove_unknown_features)](#apidoc.element.limdu.classifiers.Winnow.prototype.editFeatureValues)
- description and source-code
```javascript
editFeatureValues = function (features, remove_unknown_features) {
			if (this.bias && !('bias' in features))
				features['bias'] = 1;
			if (remove_unknown_features) {
				for (var feature in features)
					if (!(feature in this.positive_weights))
						delete features[feature];
			}
			hash.normalize_sum_of_values_to_1(features);
		}
```
- example usage
```shell
...
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
	},

	/**
...
```

#### <a name="apidoc.element.limdu.classifiers.Winnow.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.Winnow.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
			if (!json.positive_weights) throw new Error("No positive weights in json: "+JSON.stringify(json));
			this.positive_weights = json.positive_weights;
			this.positive_weights_sum = json.positive_weights_sum;
			if (!json.negative_weights) throw new Error("No negative weights in json: "+JSON.stringify(json));
			this.negative_weights = json.negative_weights;
			this.negative_weights_sum = json.negative_weights_sum;
		}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.Winnow.prototype.perceive_features"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>perceive_features (features, continuous_output, positive_weights_for_classification, negative_weights_for_classification, explain)](#apidoc.element.limdu.classifiers.Winnow.prototype.perceive_features)
- description and source-code
```javascript
perceive_features = function (features, continuous_output, positive_weights_for_classification, negative_weights_for_classification, explain) {
			var score = 0;
			var explanations = [];
			for (var feature in features) {
				if (feature in positive_weights_for_classification) {
					var positive_weight = positive_weights_for_classification[feature];
					if (!isFinite(positive_weight)) {
						console.dir(positive_weights_for_classification);
						throw new Error("positive_weight["+feature+"]="+positive_weight);
					}
					var negative_weight = negative_weights_for_classification[feature];
					if (!isFinite(negative_weight)) {
						console.dir(negative_weights_for_classification);
						throw new Error("negative_weight["+feature+"]="+negative_weight);
					}
					var net_weight = positive_weight-negative_weight;
					var value = features[feature];
					if (isNaN(value)) {
						console.dir(features);
						throw new Error("score is NaN! features["+feature+"]="+value+" net_weight="+positive_weight+"-"+negative_weight+"="+net_weight
);
					}
					var relevance = value * net_weight;
					score += relevance;
					if (isNaN(score))
						throw new Error("score is NaN! features["+feature+"]="+value+" net_weight="+positive_weight+"-"+negative_weight+"="+net_weight
);
					if (explain>0) explanations.push(
							{
								feature: feature,
								value: value,
								weight: sprintf("+%1.3f-%1.3f=%1.3f",positive_weight,negative_weight,net_weight),
								relevance: relevance,
							}
					);
				}
			}
			if (isNaN(score))
				throw new Error("score is NaN! features="+JSON.stringify(features));
			score -= this.threshold;

			if (this.debug) console.log("> perceive_features ",JSON.stringify(features)," = ",score);
			var result = (continuous_output? score: (score > 0 ? 1 : 0));
			if (explain>0) {
				explanations.sort(function(a,b){return Math.abs(b.relevance)-Math.abs(a.relevance); });
				explanations.splice(explain, explanations.length-explain);  // "explain" is the max length of explanation.
				
				if (!this.detailed_explanations) {
					explanations = explanations.map(function(e) {
						return sprintf("%s%+1.2f", e.feature, e.relevance);
					});
				}
				
				result = {
					classification: result,
					explanation: explanations,
				};
			}
			return result;
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.Winnow.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>toJSON (folder)](#apidoc.element.limdu.classifiers.Winnow.prototype.toJSON)
- description and source-code
```javascript
toJSON = function (folder) {
			return {
				positive_weights: this.positive_weights,
				negative_weights: this.negative_weights,
				positive_weights_sum: this.positive_weights_sum,
				negative_weights_sum: this.negative_weights_sum,
			}
		}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.Winnow.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.Winnow.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
//			var normalized_inputs = [];
			for (var i=0; i<dataset.length; ++i)
				this.editFeatureValues(dataset[i].input, /*remove_unknown_features=*/false);
//				normalized_inputs[i] = this.normalized_features(dataset[i].input, /*remove_unknown_features=*/false);
	
			for (var r=0; r<=this.retrain_count; ++r)
				for (var i=0; i<dataset.length; ++i)
					this.train_features(dataset[i].input, dataset[i].output);
		}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.Winnow.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>trainOnline (features, expected)](#apidoc.element.limdu.classifiers.Winnow.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (features, expected) {
			this.editFeatureValues(features, /*remove_unknown_features=*/false);
			return this.train_features(features, expected);
				//this.normalized_features(features, /*remove_unknown_features=*/false), expected);
		}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```

#### <a name="apidoc.element.limdu.classifiers.Winnow.prototype.train_features"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.Winnow.prototype.</span>train_features (features, expected)](#apidoc.element.limdu.classifiers.Winnow.prototype.train_features)
- description and source-code
```javascript
train_features = function (features, expected) {
			if (this.debug) console.log("train_features "+JSON.stringify(features)+" , "+expected);
			for (feature in features) {
				if (!(feature in this.positive_weights))
					this.positive_weights[feature] = this.default_positive_weight;
				if (!(feature in this.negative_weights))
					this.negative_weights[feature] = this.default_negative_weight;
			}

			if (this.debug) console.log('> this.positive_weights  ',JSON.stringify(this.positive_weights),', this.negative_weights: ',JSON
.stringify(this.negative_weights));

			var score = this.perceive_features(features, /*continuous_output=*/true, this.positive_weights, this.negative_weights);
				 // always use the running 'weights' vector for training, and NOT the weights_sum!

			//if (this.debug) console.log('> training ',features,', expecting: ',expected, ' got score=', score);
			
			if ((expected && score<=this.margin) || (!expected && score>=-this.margin)) {
				// Current model is incorrect - adjustment needed!
				if (expected) {
					for (var feature in features) {
						var value = features[feature];
						this.positive_weights[feature] *= (this.promotion * (1 + value));
						this.negative_weights[feature] *= (this.demotion * (1 - value));
					}
				} else {
					for (var feature in features) {
						var value = features[feature];
						this.positive_weights[feature] *= (this.demotion * (1 - value));
						this.negative_weights[feature] *= (this.promotion * (1 + value));
					}
				}
				if (this.debug) console.log('--> this.positive_weights',JSON.stringify(this.positive_weights),', this.negative_weights: ',JSON
.stringify(this.negative_weights));
				return false;
			} else {
				if (this.do_averaging) {
					hash.add(this.positive_weights_sum, this.positive_weights);
					hash.add(this.negative_weights_sum, this.negative_weights);
				}
				return true;
			}
		}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.classifiers.kNN"></a>[module limdu.classifiers.kNN](#apidoc.module.limdu.classifiers.kNN)

#### <a name="apidoc.element.limdu.classifiers.kNN.kNN"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.</span>kNN (opts)](#apidoc.element.limdu.classifiers.kNN.kNN)
- description and source-code
```javascript
kNN = function (opts) {
	this.k = opts.k
	this.mode = opts.mode
	this.distanceFunctionList = opts.distanceFunctionList
	this.distanceWeightening = opts.distanceWeightening
	this.labels = []
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.classifiers.kNN.prototype"></a>[module limdu.classifiers.kNN.prototype](#apidoc.module.limdu.classifiers.kNN.prototype)

#### <a name="apidoc.element.limdu.classifiers.kNN.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>classify (sample, explain)](#apidoc.element.limdu.classifiers.kNN.prototype.classify)
- description and source-code
```javascript
classify = function (sample, explain) {

		var trainset = _.map(this.dataset, function(value){ return {
																	'input': this.complement(value['input']),
																	'output': value['output']
																	}
																 }, this);

		// is canceled due to "okay is fine"
		// var eq = _.filter(trainset, function(value){ return _.isEqual(value['input'], sample); });
		
		// if (eq.length != 0)
			// return {
				 	// 'classification': (eq[0]['output'] == 1 ? 1 : -1),
				 	// 'explanation': 'same'
		   			// }
		
		var distances = _.map(trainset, function(value){ return {
																'input'   : value['input'],
																'output'  : value['output'],
																'distance': _.reduce(this.distanceFunctionList, function(memo, df){ return memo + df(sample, value['input']); },
0),
																'score':    _.reduce(this.distanceFunctionList, function(memo, df){ return memo + df(sample, value['input']); },
0),

																// 'distance': dfmap[this.distanceFunction](sample, value['input']),
																// 'score'   : this.distanceWeightening(_.reduce(this.distanceFunctionList, function(memo, df){ return memo + df
(sample, value['input']); }, 0))
																}
																}, this);

		var distances = _.sortBy(distances, function(num){ return num['distance']; })

		// eliminate Infinite and null

		var distances = _.filter(distances, function(num){ return !isNaN(parseFloat(num['distance'])) && isFinite(num['distance']) });
		
		if (distances.length == 0)
		{
			if (this.mode == 'binary')
				return {'classification': -1, 'explanation': 'not number'}
		}

		var metrics = _.unique(_.sortBy(_.pluck(distances, 'distance')))
		var margin = metrics[this.k]
		var real_k = distances.length - _.find(distances.reverse(), function(num){ return num['distance'] == margin })
		var knn = distances.slice(0, real_k)

		var output = _.groupBy(knn, function(num){ return num['output'] })

		if (this.mode == 'multi')
		{
			return {
					 'classes': Object.keys(output),
					 'explanation': output
			  		}
		}

		var thelabel = {'label': -1, 'score': -1}

		_.each(output, function(value, label, list){
			var sum = _.reduce(value, function(memo, num){ return memo + num['score']; }, 0);
			if (sum > thelabel['score'])
				{
					thelabel['score'] = sum	
					thelabel['label'] = label	
				}
		}, this)

		// _.each(knn, function(val, key, list){
			// console.log(val)
			// console.log(this.translaterow(val['input']))
		// }, this)

		if (this.mode == 'binary')
			return {
					 'classification': (thelabel['label'] == 1 ? thelabel['score'] : (-1) * thelabel['score']),
					 'explanation': this.translatetrain(knn)
			  		}
		}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.kNN.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.kNN.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.kNN.prototype.complement"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>complement (input)](#apidoc.element.limdu.classifiers.kNN.prototype.complement)
- description and source-code
```javascript
complement = function (input) {
		var len = this.featureLookupTable['featureIndexToFeatureName'].length
		_(len - input.length).times(function(n){
			input.push(0)
		})
		return input
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.kNN.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.kNN.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
	}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.kNN.prototype.getAllClasses"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.kNN.prototype.getAllClasses)
- description and source-code
```javascript
getAllClasses = function () {
	}
```
- example usage
```shell
...
		if (this.pastTrainingSamples) this.pastTrainingSamples = json.pastTrainingSamples;
		this.featureDocumentFrequency = json.featureDocumentFrequency;
		this.documentCount = json.documentCount;
		/* Note: the feature extractors are functions - they should be created at initialization - they are not deserializable! */
	},

	getAllClasses: function() {  // relevant for multilabel classifiers
		return this.classifier.getAllClasses();
	},
}  // end of EnhancedClassifier prototype


var stringifyClass = function (aClass) {
	return (_(aClass).isString()? aClass: JSON.stringify(aClass));
}
...
```

#### <a name="apidoc.element.limdu.classifiers.kNN.prototype.setFeatureLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.kNN.prototype.setFeatureLookupTable)
- description and source-code
```javascript
setFeatureLookupTable = function (featureLookupTable) {
		this.featureLookupTable = featureLookupTable
	}
```
- example usage
```shell
...

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
	this.tfidf = new opts.TfIdfImpl
...
```

#### <a name="apidoc.element.limdu.classifiers.kNN.prototype.stringifyClass"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>stringifyClass (aClass)](#apidoc.element.limdu.classifiers.kNN.prototype.stringifyClass)
- description and source-code
```javascript
stringifyClass = function (aClass) {
		return (_(aClass).isString()? aClass: JSON.stringify(aClass));
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.kNN.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.kNN.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
	}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.kNN.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.kNN.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
		this.dataset = dataset
	}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.kNN.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>trainOnline (sample, labels)](#apidoc.element.limdu.classifiers.kNN.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (sample, labels) {
	}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```

#### <a name="apidoc.element.limdu.classifiers.kNN.prototype.translaterow"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>translaterow (row)](#apidoc.element.limdu.classifiers.kNN.prototype.translaterow)
- description and source-code
```javascript
translaterow = function (row)
	{
		var output = {}

		_.each(row, function(value, key, list){
			if (value != 0)
				output[this.featureLookupTable['featureIndexToFeatureName'][key]] = value
		}, this)

		return output
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.kNN.prototype.translatetrain"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.kNN.prototype.</span>translatetrain (input)](#apidoc.element.limdu.classifiers.kNN.prototype.translatetrain)
- description and source-code
```javascript
translatetrain = function (input)
	{
		if (this.featureLookupTable)
		{
			_.each(input, function(value, key, list){
				input[key]['input'] = this.translaterow(value['input'])
			}, this)
			return input
		}
		else
		return input

	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.classifiers.multilabel"></a>[module limdu.classifiers.multilabel](#apidoc.module.limdu.classifiers.multilabel)

#### <a name="apidoc.element.limdu.classifiers.multilabel.Adaboost"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>Adaboost (opts)](#apidoc.element.limdu.classifiers.multilabel.Adaboost)
- description and source-code
```javascript
Adaboost = function (opts) {
	if (!Adaboost.isInstalled()) {
		var msg = "Cannot find the executable 'icsiboost'.";
		console.error(msg)
		throw new Error(msg);
	}

	this.set_of_labels = []
	this.text_expert = 'ngram'
	this.assigner = crypto.randomBytes(20).toString('hex');
	this.folder = "icsiboost_data"

	this.ngram_length = opts.ngram_length || 2
	this.iterations = opts.iterations || 2000
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinaryRelevance"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>BinaryRelevance (opts)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance)
- description and source-code
```javascript
BinaryRelevance = function (opts) {
	if (!opts.binaryClassifierType) {
		console.dir(opts);
		throw new Error("opts.binaryClassifierType not found");
	}
	this.binaryClassifierType = opts.binaryClassifierType;
	this.debug = opts.debug || false
	this.mapClassnameToClassifier = {};
}
```
- example usage
```shell
...
In binary classification, the output is 0 or 1;

In multi-label classification, the output is a set of zero or more labels.

'''js
var MyWinnow = limdu.classifiers.Winnow.bind(0, {retrain_count: 10});

var intentClassifier = new limdu.classifiers.multilabel.BinaryRelevance({
	binaryClassifierType: MyWinnow
});

intentClassifier.trainBatch([
	{input: {I:1,want:1,an:1,apple:1}, output: "APPLE"},
	{input: {I:1,want:1,a:1,banana:1}, output: "BANANA"},
	{input: {I:1,want:1,chips:1}, output: "CHIPS"}
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinarySegmentation"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>BinarySegmentation (opts)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation)
- description and source-code
```javascript
BinarySegmentation = function (opts) {
	if (!('binaryClassifierType' in opts)) {
		console.dir(opts);
		throw new Error("opts must contain binaryClassifierType");
	}
	if (!opts.binaryClassifierType) {
		console.dir(opts);
		throw new Error("opts.binaryClassifierType is null");
	}

	this.binaryClassifierType = opts.binaryClassifierType;
	this.classifier = new this.binaryClassifierType();

	switch (opts.segmentSplitStrategy) {
	case 'shortestSegment': this.segmentSplitStrategy = this.shortestSegmentSplitStrategy; break;
	case 'longestSegment':  this.segmentSplitStrategy = this.longestSegmentSplitStrategy;  break;
	case 'cheapestSegment':  this.segmentSplitStrategy = this.cheapestSegmentSplitStrategy;  break;
	default: this.segmentSplitStrategy = null;
	}
	
	this.mapClassnameToClassifier = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>CrossLanguageModel (opts)](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel)
- description and source-code
```javascript
CrossLanguageModel = function (opts) {
	this.model = new CrossLanguageModel(opts);
	this.labelFeatureExtractor = opts.labelFeatureExtractor;
	this.threshold = opts.threshold || 0;
	this.allLabels = {};
	this.allLabelsFeatures = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Homer"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>Homer (opts)](#apidoc.element.limdu.classifiers.multilabel.Homer)
- description and source-code
```javascript
Homer = function (opts) {
	opts = opts || {};
	if (!opts.multilabelClassifierType) {
		console.dir(opts);
		throw new Error("opts.multilabelClassifierType is null");
	}
	this.multilabelClassifierType = opts.multilabelClassifierType;
	
	this.splitLabel = opts.splitLabel || function(label)      {return label.split(/@/);}
	this.joinLabel  = opts.joinLabel  || function(superlabel) {return superlabel.join("@");}
	
	this.root = {
		superlabelClassifier: this.newMultilabelClassifier(),
		mapSuperlabelToBranch: {}
	}
	
	this.allClasses = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MetaLabeler"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>MetaLabeler (opts)](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler)
- description and source-code
```javascript
MetaLabeler = function (opts) {
	if (!opts.rankerType) {
		console.dir(opts);
		throw new Error("opts.rankerType not found");
	}
	if (!opts.counterType) {
		console.dir(opts);
		throw new Error("opts.counterType not found");
	}
	this.ranker = new opts.rankerType();
	this.counter = new opts.counterType();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>MulticlassSegmentation (opts)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation)
- description and source-code
```javascript
MulticlassSegmentation = function (opts) {
	if (!opts.multiclassClassifierType) {
		console.dir(opts);
		throw new Error("opts.multiclassClassifierType not found");
	}
	this.multiclassClassifierType = opts.multiclassClassifierType;
	this.featureExtractor = FeaturesUnit.normalize(opts.featureExtractor);
	
	this.multiclassClassifier = new this.multiclassClassifierType();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PartialClassification"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>PartialClassification (opts)](#apidoc.element.limdu.classifiers.multilabel.PartialClassification)
- description and source-code
```javascript
PartialClassification = function (opts) {
	
	opts = opts || {};
	if (!opts.multilabelClassifierType) {
		console.dir(opts);
		throw new Error("opts.multilabelClassifierType is null");
	}

	if (!opts.numberofclassifiers) {
		console.dir(opts);
		throw new Error("opts.numberofclassifiers is null");
	}

	// this.splitLabel = opts.splitLabel || function(label)      {return label.split(/@/);}
	this.classifier = this.intializeClassifiers(opts.numberofclassifiers, opts.multilabelClassifierType)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PassiveAggressive"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>PassiveAggressive (opts)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive)
- description and source-code
```javascript
PassiveAggressive = function (opts) {
	this.retrain_count = opts.retrain_count || 10;
	this.Constant = opts.Constant || 5.0;
	this.weights = {
		//DUMMY_CLASS:{}
	};
	this.weights_sum = {
		//DUMMY_CLASS:{}
	};
	this.seenFeatures = {};
	this.num_iterations = 0
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.</span>ThresholdClassifier (opts)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier)
- description and source-code
```javascript
ThresholdClassifier = function (opts) {
	
	opts = opts || {};

	if (!('multiclassClassifierType' in opts)) {
		console.dir(opts);
		throw new Error("opts must contain multiclassClassifierType");
	}
	if (!opts.multiclassClassifierType) {
		console.dir(opts);
		throw new Error("opts.multiclassClassifierType is null");
	}

	if (!('evaluateMeasureToMaximize' in opts)) {
		console.dir(opts);
		throw new Error("opts must contain evaluateMeasureToMaximize");
	}
	if (!opts.evaluateMeasureToMaximize) {
		console.dir(opts);
		throw new Error("opts.evaluateMeasureToMaximize is null");
	}
	if (!opts.numOfFoldsForThresholdCalculation) {
		console.dir(opts);
		throw new Error("opts.numOfFoldsForThresholdCalculation is null");
	}
	
	this.multiclassClassifier = new opts.multiclassClassifierType();

	// [F1, Accuracy]	
	this.evaluateMeasureToMaximize = opts.evaluateMeasureToMaximize;

	// constant size of validation set
	this.devsetsize = 0.1

	// > 1, n - fold cross - validation, otherwise validation set
	this.numOfFoldsForThresholdCalculation = opts.numOfFoldsForThresholdCalculation
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.classifiers.multilabel.Adaboost.prototype"></a>[module limdu.classifiers.multilabel.Adaboost.prototype](#apidoc.module.limdu.classifiers.multilabel.Adaboost.prototype)

#### <a name="apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>classify (sample, explain)](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.classify)
- description and source-code
```javascript
classify = function (sample, explain) {

		if (this.set_of_labels.length == 1) {return this.set_of_labels[0]}

		fs.writeFileSync("./"+this.folder+"/"+this.assigner+".test", sample.replace(/\,/g,'')+"\n")
		fs.writeFileSync("./"+this.folder+"/"+this.assigner+".test", sample+"\n")
		var result = execSync("icsiboost -S ./"+this.folder+"/"+this.assigner +" -W "+this.ngram_length+" -N "+this.text_expert+" -C < ./"+
this.folder+"/"+this.assigner+".test > ./"+this.folder+"/"+this.assigner+".output")
		var stats = fs.readFileSync("./"+this.folder+"/"+this.assigner+".output", "utf8");

		set_of_labels = this.set_of_labels

		stats = stats.replace(/^\s+|\s+$/g, "");
		ar = stats.split(" ")

		actual = ar.slice(ar.length/2, ar.length)

		actual1 = []

		_.each(actual, function(value, key){
			if (value>0) {
				actual1.push(set_of_labels[key])}
			})
	
		return actual1
	}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
	}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.getAllClasses"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.getAllClasses)
- description and source-code
```javascript
getAllClasses = function () {
	}
```
- example usage
```shell
...
		if (this.pastTrainingSamples) this.pastTrainingSamples = json.pastTrainingSamples;
		this.featureDocumentFrequency = json.featureDocumentFrequency;
		this.documentCount = json.documentCount;
		/* Note: the feature extractors are functions - they should be created at initialization - they are not deserializable! */
	},

	getAllClasses: function() {  // relevant for multilabel classifiers
		return this.classifier.getAllClasses();
	},
}  // end of EnhancedClassifier prototype


var stringifyClass = function (aClass) {
	return (_(aClass).isString()? aClass: JSON.stringify(aClass));
}
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.setFeatureLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.setFeatureLookupTable)
- description and source-code
```javascript
setFeatureLookupTable = function (featureLookupTable) {
	
	}
```
- example usage
```shell
...

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
	this.tfidf = new opts.TfIdfImpl
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.stringifyClass"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>stringifyClass (aClass)](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.stringifyClass)
- description and source-code
```javascript
stringifyClass = function (aClass) {
		return (_(aClass).isString()? aClass: JSON.stringify(aClass));
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
	}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {

		set_of_labels = []
		_.times(1, function(){dataset = _.shuffle(dataset)})
		_.each(dataset, function(value, key, list){
			_.each(value['output'], function(value1, key, list){
				set_of_labels.push(this.stringifyClass(value1))
			},this)
		}, this);

		this.set_of_labels = _.uniq(set_of_labels)

		if (this.set_of_labels.length == 1) {return 0}

		dataset = _.map(dataset, function(value){
			values = []
				_.each(value['output'], function(value1, key, list){
				values.push(this.set_of_labels.indexOf(this.stringifyClass(value1))+1)
			}, this);

			return {'input':value['input'], 'output': values}
		}, this);
	
		ar = []
		_.times(this.set_of_labels.length, function(n){ar.push(n+1)})

  		try {(!fs.statSync(this.folder).isDirectory())}
  		catch(e) {fs.mkdirSync(this.folder)}
  			
		names = ar.join()+".\nsentence:text:expert_type="+this.text_expert+" expert_length="+this.ngram_length+"."
	 	fs.writeFileSync("./"+this.folder+"/"+this.assigner+'.names', names)

		set = {}
		dataset = partitions.partition(dataset, 1, Math.round(dataset.length*0.3))
		set['data'] = dataset['train']
		set['dev']  = dataset['test']	

		_.each(set, function(valueset, key1, list){
			str = ""
			_.each(valueset, function(value, key, list){
					if (value['input'].length <= 1) return
	    			str += value['input'].replace(/\,/g,'') + ',' + value['output'].join(" ")+ ".\n"
	    			//str += value['input']+ ',' + value['output'].join(" ")+ ".\n"
	    		})

			fs.writeFileSync("./"+this.folder+"/"+this.assigner+"."+key1, str)
		}, this)

		var result = execSync("icsiboost -S ./"+this.folder+"/"+this.assigner+" -n "+this.iterations)
		console.log(result)
	}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Adaboost.prototype.</span>trainOnline (sample, labels)](#apidoc.element.limdu.classifiers.multilabel.Adaboost.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (sample, labels) {
	
	}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```



# <a name="apidoc.module.limdu.classifiers.multilabel.BinaryRelevance.prototype"></a>[module limdu.classifiers.multilabel.BinaryRelevance.prototype](#apidoc.module.limdu.classifiers.multilabel.BinaryRelevance.prototype)

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>classify (sample, explain, withScores)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.classify)
- description and source-code
```javascript
classify = function (sample, explain, withScores) {
		var labels = []
		var scores = []
		var explanations = [];
		var positive_explanations = {};
		var negative_explanations = []

		for (var label in this.mapClassnameToClassifier) {
			var classifier = this.mapClassnameToClassifier[label];

			if (this.debug) console.dir("Classify for class="+label)
			
			// fs.writeFileSync('/tmp/labels/'+label, JSON.stringify(classifier.getFeatures(), null, 4), 'utf8');

			var scoreWithExplain = classifier.classify(sample, explain, withScores);
			if (this.debug) console.log(JSON.stringify(scoreWithExplain, null, 4))

			var score = scoreWithExplain.explanation?  scoreWithExplain.classification: scoreWithExplain;
			if (this.debug) console.dir("score="+score)

			explanations_string = scoreWithExplain.explanation

			// if (score>0.5)
			if (score>0)
				{
				labels.push([label, score])
				if (explanations_string) positive_explanations[label]=explanations_string;
				}
			else
				{
				if (explanations_string) negative_explanations.push([label, score, explanations_string])
				}

			scores.push([label,score])
		}

		if (this.debug) console.dir(scores)

		if (explain>0)
		{
			scores = _.sortBy(scores, function(num){ return num[1] }).reverse()
			var scores_hash = _.object(scores)

			negative_explanations = _.sortBy(negative_explanations, function(num){ return num[1] }).reverse()
			negative_explanations = _.map(negative_explanations, function(num){ return [num[0],num[2]] });

			var negative_explanations_hash = _.object(negative_explanations)
		}

		labels = _.sortBy(labels, function(num){ return num[1] });
		labels = _.map(labels.reverse(), function(num){ return num[0] });

		return (explain>0?
			{
				classes: labels,
				scores: scores_hash,
				explanation: {
					positive: positive_explanations,
					negative: negative_explanations_hash,
				}
			}:
			labels);
	}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.classifyBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>classifyBatch (testSet)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.classifyBatch)
- description and source-code
```javascript
classifyBatch = function (testSet) {
		var labels = []
		var results = {}
		var output = []

		for (var label in this.mapClassnameToClassifier) {
			var classifier = this.mapClassnameToClassifier[label]
			var scoreWithExplain = classifier.classifyBatch(testSet)
			results[label] = scoreWithExplain
		}

		_.each(testSet, function(value, key, list){
			testSet[key]['output'] = []
			_.each(results, function(ar, label, list){
				if (ar[key]!=0)
					testSet[key]['output'].push(label)
			}, this)
		}, this)

		return testSet
	}
```
- example usage
```shell
...
            _.each(testSet, function(value, key, list){
                testSet[key]["input"] = this.normalizedSample(testSet[key]["input"])
                var features = this.sampleToFeatures(testSet[key]["input"], this.featureExtractors, this.stopwords);
                this.editFeatureValues(features, /*remove_unknown_features=*/false);
                var array = this.featuresToArray(features);
                testSet[key]["input"] = array
            }, this)
            return this.classifier.classifyBatch(testSet);
        },
	
	classifyPartAsync: function(sample, explain, callback) {
		this.sampleToFeaturesAsync(sample, this.featureExtractors, (function(err, results){
			this.editFeatureValues(features, /*remove_unknown_features=*/false);
			var array = this.featuresToArray(features);
			var classification = this.classifier.classify(array, explain);
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
		for (var label in json) {
			this.mapClassnameToClassifier[label] = new this.binaryClassifierType();
			this.mapClassnameToClassifier[label].fromJSON(json[label]);
		}
	}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.getAllClasses"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.getAllClasses)
- description and source-code
```javascript
getAllClasses = function () {
		return Object.keys(this.mapClassnameToClassifier);
	}
```
- example usage
```shell
...
		if (this.pastTrainingSamples) this.pastTrainingSamples = json.pastTrainingSamples;
		this.featureDocumentFrequency = json.featureDocumentFrequency;
		this.documentCount = json.documentCount;
		/* Note: the feature extractors are functions - they should be created at initialization - they are not deserializable! */
	},

	getAllClasses: function() {  // relevant for multilabel classifiers
		return this.classifier.getAllClasses();
	},
}  // end of EnhancedClassifier prototype


var stringifyClass = function (aClass) {
	return (_(aClass).isString()? aClass: JSON.stringify(aClass));
}
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.makeSureClassifierExists"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>makeSureClassifierExists (label)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.makeSureClassifierExists)
- description and source-code
```javascript
makeSureClassifierExists = function (label) {
		if (!this.mapClassnameToClassifier[label]) { // make sure classifier exists
			this.mapClassnameToClassifier[label] = new this.binaryClassifierType();
			if (this.featureLookupTable && this.mapClassnameToClassifier[label].setFeatureLookupTable)
				this.mapClassnameToClassifier[label].setFeatureLookupTable(this.featureLookupTable);
			
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.setFeatureLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.setFeatureLookupTable)
- description and source-code
```javascript
setFeatureLookupTable = function (featureLookupTable) {
		//console.log("BR setFeatureLookupTable "+featureLookupTable);
		this.featureLookupTable = featureLookupTable;
		for (var label in this.mapClassnameToClassifier)
			if (featureLookupTable && this.mapClassnameToClassifier[label].setFeatureLookupTable)
				this.mapClassnameToClassifier[label].setFeatureLookupTable(featureLookupTable);
	}
```
- example usage
```shell
...

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
	this.tfidf = new opts.TfIdfImpl
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
		var result = {};
		for (var label in this.mapClassnameToClassifier) {
			var binaryClassifier = this.mapClassnameToClassifier[label];
			if (!binaryClassifier.toJSON) {
				console.dir(binaryClassifier);
				console.log("prototype: ");
				console.dir(binaryClassifier.__proto__);
				throw new Error("this binary classifier does not have a toJSON function");
			}
			result[label] = binaryClassifier.toJSON();
		}
		return result;
	}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
		// this variable will hold a dataset for each binary classifier:
		var mapClassnameToDataset = {};

		// create positive samples for each class:
		for (var d in dataset) {
			var sample = dataset[d].input;
			dataset[d].output = multilabelutils.normalizeOutputLabels(dataset[d].output);
			var labels = dataset[d].output;

			for (var l in labels) {
				var positiveLabel  = labels[l];
				this.makeSureClassifierExists(positiveLabel);
				if (!(positiveLabel in mapClassnameToDataset)) // make sure dataset for this class exists
					mapClassnameToDataset[positiveLabel] = [];
				mapClassnameToDataset[positiveLabel].push({
					input : sample,
					output : 1
				})
			}
		}

		// create negative samples for each class (after all labels are in the array):
		for (var d in dataset) {
			var sample = dataset[d].input;
			var labels = dataset[d].output;
			for (var negativeLabel in this.mapClassnameToClassifier) {
				if (!(negativeLabel in mapClassnameToDataset)) // make sure dataset for this class exists
					mapClassnameToDataset[negativeLabel] = [];
				if (labels.indexOf(negativeLabel)<0)
					mapClassnameToDataset[negativeLabel].push({
						input : sample,
						output : 0
					});
			}
		}

		// train all classifiers:
		for (var label in mapClassnameToDataset) {
			if (this.debug) console.dir("TRAIN class="+label);
			this.mapClassnameToClassifier[label]
					.trainBatch(mapClassnameToDataset[label]);
		}
	}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinaryRelevance.prototype.</span>trainOnline (sample, labels)](#apidoc.element.limdu.classifiers.multilabel.BinaryRelevance.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (sample, labels) {
		labels = multilabelutils.normalizeOutputLabels(labels);
		for (var l in labels) {
			var positiveLabel = labels[l];
			this.makeSureClassifierExists(positiveLabel);
			this.mapClassnameToClassifier[positiveLabel].trainOnline(sample, 1);
		}
		for (var negativeLabel in this.mapClassnameToClassifier) {
			if (labels.indexOf(negativeLabel)<0)
				this.mapClassnameToClassifier[negativeLabel].trainOnline(sample, 0);
		}
	}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```



# <a name="apidoc.module.limdu.classifiers.multilabel.BinarySegmentation.prototype"></a>[module limdu.classifiers.multilabel.BinarySegmentation.prototype](#apidoc.module.limdu.classifiers.multilabel.BinarySegmentation.prototype)

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.bestClassOfSegment"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>bestClassOfSegment (segment, explain)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.bestClassOfSegment)
- description and source-code
```javascript
bestClassOfSegment = function (segment, explain) {
		var classes = this.classifySegment(segment, explain);
		if (classes.classes.length==0) {
			// FEATURES
			return ['', 0, ''];
			// return ['', 0];
		} else {
			// HERE
			// console.log([classes.classes[0], classes.scores[classes.classes[0]]])
			// FEATURES
			return [classes.classes[0], classes.scores[classes.classes[0]], classes['explanation']['positive']];
			// return [classes.classes[0], classes.scores[classes.classes[0]]];
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.cheapestSegmentSplitStrategy"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>cheapestSegmentSplitStrategy (words, accumulatedClasses, explain, explanations)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.cheapestSegmentSplitStrategy)
- description and source-code
```javascript
cheapestSegmentSplitStrategy = function (words, accumulatedClasses, explain, explanations) {

		//for (var start=0; start<=words.length; ++start) {
		//	for (var end=start+1; end<=words.length; ++end) {
		//		var segment = words.slice(start,end).join(" ");

		//		var bestClassAndProbability = this.bestClassOfSegment(segment, explain);
		//		if (bestClassAndProbability[1] != Infinity)
		//		{
		//			var bestClass = bestClassAndProbability[0];
		//			var bestClassProbability = bestClassAndProbability[1];
			//		digraph.add(start, end, -bestClassProbability);
		//		}
		//	}
		//}

		var cheapest_paths = require("graph-paths").cheapest_paths;

                var mini = Infinity
                _(words.length).times(function(nn){
                   cheapestSegmentClassificationCosts = cheapest_paths(segmentClassificationCosts, nn);
                       _.each(cheapestSegmentClassificationCosts, function(value, key, list){
                             if (value.cost<mini)
                               {
                                mini = value.cost
	                            cheapestSentenceClassificationCost = value
                                 }
                         }, this)
                 }, this)

     cheapestSegmentClassificationCosts = cheapest_paths(segmentClassificationCosts, 0);
     cheapestSentenceClassificationCost = cheapestSegmentClassificationCosts[words.length];


        var path = cheapestSentenceClassificationCost.path;


		for (var i=0; i<path.length-1; ++i) {
			// var segment = words.slice(cheapestClassificationPath[i],cheapestClassificationPath[i+1]).join(" ");
			var segment = words.slice(path[i],path[i+1]).join(" ");
			//HERE
			var segmentClassesWithExplain = this.classifySegment(segment, explain);
			var segmentClasses = (segmentClassesWithExplain.classes? segmentClassesWithExplain.classes: segmentClassesWithExplain);
			
			if (segmentClasses.length>0)
				accumulatedClasses[segmentClasses[0]] = true;

			// explanations = []
			if (explain>0) {
					if (segmentClasses.length>0)
						explanations.push([segmentClasses[0], segment, [path[i], path[i+1]],segmentClassesWithExplain['explanation']['positive']])

			};
			
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>classify (sentence, explain)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.classify)
- description and source-code
```javascript
classify = function (sentence, explain) {

		// sentence = "['start'] " + sentence + " ['end']"
		var minWordsToSplit = 2;
		var words = sentence.split(/ /);
		// var words = tokenizer.tokenize(sentence);
		if (this.segmentSplitStrategy && words.length>=minWordsToSplit) {
			var accumulatedClasses = {};
			var explanations = [];
			this.segmentSplitStrategy(words, accumulatedClasses, explain, explanations);
			
			var classes = Object.keys(accumulatedClasses);

			return (explain>0?	{
				classes: classes,
				explanation: explanations
			}:
			classes);
		} else {
			classification = this.bestClassOfSegment(sentence, explain)
			// classification = this.classifySegment(sentence, explain);
			//HERER

			// console.log(sentence)
			// console.log(classification)
			// process.exit(0)
			// process.exit(0)

			return (explain>0?	{
				classes: classification[0],
				// FEATURES
				explanation: [[classification[0], sentence, [0,sentence.length-1], classification[2]]]
				// explanation: [[classification[0], sentence, [0,sentence.length-1]]]

			}:
			classification[0]);
			// return {classes: classification[0],
					// explanation: [[classification[0], sentence, [0,sentence.length-1]]]}
			// return {classes: classification.classes[0]}
		}
	}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.classifySegment"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>classifySegment (segment, explain)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.classifySegment)
- description and source-code
```javascript
classifySegment = function (segment, explain) {
			var classification = this.classifier.classify(segment, explain, true);
			// console.log(classification)
			// if (classification.classes.length != 0)
			{
				// HERE
				// console.log(segment)
				// console.log(classification['classes'])
				// console.log(classification['scores'])
				// console.log(classification['explanation']['positive'])
				// console.log(classification['explanation']['negative'])
				// // console.log()
				// process.exit(0)
				// console.log(classification['explanation']['negative']['Query'])
				// console.log(classification['explanation']['negative']['10%'])
			}


			// if ((segment == "Leased car")&&('With leased car' in classification['explanation']['negative']))
				{
				// console.log(classification['explanation']['negative']['With leased car'])
				// console.log("______________________________________")
				// process.exit(0)

				}
			return classification
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>fromJSON (json, callback)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json, callback) {
		for ( var aClass in json) {
			this.mapClassnameToClassifier[aClass] = new this.binaryClassifierType();
			this.mapClassnameToClassifier[aClass].fromJSON(json[aClass]);
		}
	}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.longestSegmentSplitStrategy"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>longestSegmentSplitStrategy (words, accumulatedClasses, explain, explanations)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.longestSegmentSplitStrategy)
- description and source-code
```javascript
longestSegmentSplitStrategy = function (words, accumulatedClasses, explain, explanations) {
		var currentStart = 0;
		var segment = null;
		var segmentClassesWithExplain = null;
		var segmentClasses = null;
		for (var currentEnd=1; currentEnd<=words.length; ++currentEnd) {
			var nextSegment = words.slice(currentStart,currentEnd).join(" ");
			var nextSegmentClassesWithExplain = this.classifySegment(nextSegment, explain);
			var nextSegmentClasses = (nextSegmentClassesWithExplain.classes? nextSegmentClassesWithExplain.classes: nextSegmentClassesWithExplain
);
			//console.log("\t"+JSON.stringify(nextSegment) +" -> "+nextSegmentClasses)
			nextSegmentClasses.sort();

			if (segmentClasses && segmentClasses.length==1 && (nextSegmentClasses.length>1 || !_(nextSegmentClasses).isEqual(segmentClasses
))) {
				// greedy algorithm: found a section with a single class - cut it and go on
				accumulatedClasses[segmentClasses[0]]=true;
				currentStart = currentEnd-1;
				if (explain>0) {
					explanations.push(segment);
					explanations.push(segmentClassesWithExplain.explanation);
				};
			}

			segment = nextSegment;
			segmentClassesWithExplain = nextSegmentClassesWithExplain;
			segmentClasses = nextSegmentClasses;
		}
		
		// add the classes of the last section:
		for (var i in segmentClasses)
			accumulatedClasses[segmentClasses[i]]=true;
		if (explain>0) {
			explanations.push(segment);
			explanations.push(segmentClassesWithExplain.explanation);
		};
		<span class="apidocCodeCommentSpan">/*if (words.length>20)  {
			console.dir(explanations);
			process.exit(1);
		}*/
</span>	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.setFeatureLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.setFeatureLookupTable)
- description and source-code
```javascript
setFeatureLookupTable = function (featureLookupTable) {
		if (featureLookupTable)
			// this.featureLookupTable = featureLookupTable
			if (this.classifier.setFeatureLookupTable)
				this.classifier.setFeatureLookupTable(featureLookupTable);  // for generating clearer explanations only
		// }
	}
```
- example usage
```shell
...

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
	this.tfidf = new opts.TfIdfImpl
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.shortestSegmentSplitStrategy"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>shortestSegmentSplitStrategy (words, accumulatedClasses, explain, explanations)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.shortestSegmentSplitStrategy)
- description and source-code
```javascript
shortestSegmentSplitStrategy = function (words, accumulatedClasses, explain, explanations) {
		var currentStart = 0;
		for (var currentEnd=1; currentEnd<=words.length; ++currentEnd) {
			var segment = words.slice(currentStart,currentEnd).join(" ");
			var segmentClassesWithExplain = this.classifySegment(segment, explain);
			var segmentClasses = (segmentClassesWithExplain.classes? segmentClassesWithExplain.classes: segmentClassesWithExplain);

			if (segmentClasses.length==1) {
				// greedy algorithm: found a section with a single class - cut it and go on
				accumulatedClasses[segmentClasses[0]]=true;
				currentStart = currentEnd;
				if (explain>0) {
					explanations.push(segment);
					explanations.push(segmentClassesWithExplain.explanation);
				};
			}
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>toJSON (callback)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.toJSON)
- description and source-code
```javascript
toJSON = function (callback) {
		var result = {};
		for ( var aClass in this.mapClassnameToClassifier) {
			var binaryClassifier = this.mapClassnameToClassifier[aClass];
			if (!binaryClassifier.toJSON) {
				console.dir(binaryClassifier);
				console.log("prototype: ");
				console.dir(binaryClassifier.__proto__);
				throw new Error("this binary classifier does not have a toJSON function");
			}
			result[aClass] = binaryClassifier.toJSON(callback);
		}
		return result;
	}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
		// add ['start'] and ['end'] as a try to resolve Append:previous FP
		_.map(dataset, function(num){
			num['input'] = "['start'] "+ num['input'] + " ['end']"
			return num });

		this.classifier.trainBatch(dataset)
	}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.BinarySegmentation.prototype.</span>trainOnline (sample, classes)](#apidoc.element.limdu.classifiers.multilabel.BinarySegmentation.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (sample, classes) {
		sample = this.sampleToFeatures(sample, this.featureExtractors);
		classes = hash.normalized(classes);
		for (var positiveClass in classes) {
			this.makeSureClassifierExists(positiveClass);
			this.mapClassnameToClassifier[positiveClass].trainOnline(sample, 1);
		}
		for (var negativeClass in this.mapClassnameToClassifier) {
			if (!classes[negativeClass])
				this.mapClassnameToClassifier[negativeClass].trainOnline(sample, 0);
		}
	}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```



# <a name="apidoc.module.limdu.classifiers.multilabel.CrossLanguageModel.prototype"></a>[module limdu.classifiers.multilabel.CrossLanguageModel.prototype](#apidoc.module.limdu.classifiers.multilabel.CrossLanguageModel.prototype)

#### <a name="apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.CrossLanguageModel.prototype.</span>classify (features, explain, withScores)](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.classify)
- description and source-code
```javascript
classify = function (features, explain, withScores) {
		var scoresVector = [];
		for (var labelString in this.allLabels) {
			var label = this.allLabels[labelString];
			var labelFeatures = this.allLabelsFeatures[labelString];
			if (!labelFeatures)
				throw new Error("label features for "+labelString+" are undefined");
			var similarity = -this.model.divergence(features, labelFeatures);
			scoresVector.push([label, similarity]);
		}
		scoresVector.sort(function(a,b) {return b[1]-a[1]}); // sort by decreasing score
		
		return multilabelutils.mapScoresVectorToMultilabelResult(scoresVector, explain, withScores, this.threshold);
	}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.CrossLanguageModel.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.CrossLanguageModel.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
		this.allLabels = json.allLabels;
		this.model.fromJSON(json);
	}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.getAllClasses"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.CrossLanguageModel.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.getAllClasses)
- description and source-code
```javascript
getAllClasses = function () {
		return Object.keys(this.allLabels);
	}
```
- example usage
```shell
...
		if (this.pastTrainingSamples) this.pastTrainingSamples = json.pastTrainingSamples;
		this.featureDocumentFrequency = json.featureDocumentFrequency;
		this.documentCount = json.documentCount;
		/* Note: the feature extractors are functions - they should be created at initialization - they are not deserializable! */
	},

	getAllClasses: function() {  // relevant for multilabel classifiers
		return this.classifier.getAllClasses();
	},
}  // end of EnhancedClassifier prototype


var stringifyClass = function (aClass) {
	return (_(aClass).isString()? aClass: JSON.stringify(aClass));
}
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.labelsToFeatures"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.CrossLanguageModel.prototype.</span>labelsToFeatures (labels)](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.labelsToFeatures)
- description and source-code
```javascript
labelsToFeatures = function (labels) {
		if (!Array.isArray(labels))  labels = [labels];
		var features = {};
		for (var i in labels) {
			var label = labels[i];
			var labelString = multilabelutils.stringifyIfNeeded(label);
			var labelFeatures = {};
			if (this.labelFeatureExtractor) {
				this.labelFeatureExtractor(label, labelFeatures);
			} else if (_.isObject(label)) {
				labelFeatures = label;
			} else {
				labelFeatures[label] = true;
			}
			this.allLabels[labelString] = label;
			this.allLabelsFeatures[labelString] = labelFeatures;
			features = util._extend(features, labelFeatures);
		}
		return features;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.CrossLanguageModel.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
		return {
			allLabels: this.allLabels,
			model: this.model.toJSON(),
		}
	}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.CrossLanguageModel.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
		dataset = dataset.map(function(datum) {
			return {
				input: datum.input,
				output: this.labelsToFeatures(datum.output),
			}
		}, this);
		this.model.trainBatch(dataset);
	}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.CrossLanguageModel.prototype.</span>trainOnline (features, labels)](#apidoc.element.limdu.classifiers.multilabel.CrossLanguageModel.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (features, labels) {
		this.model.trainOnline(
			features, // input features
			this.labelsToFeatures(labels)); // output features
	}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```



# <a name="apidoc.module.limdu.classifiers.multilabel.Homer.prototype"></a>[module limdu.classifiers.multilabel.Homer.prototype](#apidoc.module.limdu.classifiers.multilabel.Homer.prototype)

#### <a name="apidoc.element.limdu.classifiers.multilabel.Homer.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>classify (sample, explain)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.classify)
- description and source-code
```javascript
classify = function (sample, explain) {
		var splitLabels = this.classifyRecursive(sample, explain, this.root);
		//console.log("splitLabels:"+JSON.stringify(splitLabels));
		if (explain>0) {
			splitLabels.classes = splitLabels.classes.map(this.joinLabel);
		} else {
			splitLabels = splitLabels.map(this.joinLabel);
		}
		return splitLabels;
	}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Homer.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Homer.prototype.classifyRecursive"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>classifyRecursive (sample, explain, treeNode, depth)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.classifyRecursive)
- description and source-code
```javascript
classifyRecursive = function (sample, explain, treeNode, depth) {
		if (!depth) depth = 1;
		// classify the superlabel
		var superlabelsWithExplain = treeNode.superlabelClassifier.classify(sample, explain);
		var superlabels = (explain>0? superlabelsWithExplain.classes: superlabelsWithExplain);
		
		var splitLabels = [];
		if (explain>0) {
			var explanations = ["depth="+depth+": "+superlabels, superlabelsWithExplain.explanation];
		}

		// for all superlabels that were classified, may be there are more than one that were classified with it
		for (var i in superlabels) {
			var superlabel = superlabels[i];
			var splitLabel = [superlabel];
			
			// classifier of [Offer] types / second level / classifies Offer's parameters
			var branch = treeNode.mapSuperlabelToBranch[superlabel];
			
			if (branch) {
				
				// [ [ 'Without leased car' ] ]
				var branchLabelsWithExplain = this.classifyRecursive(sample, explain, branch, depth+1);
				
				var branchLabels = (explain>0? branchLabelsWithExplain.classes: branchLabelsWithExplain);
					
				for (var j in branchLabels)
					splitLabels.push(splitLabel.concat(branchLabels[j]));
				if (explain>0)
					explanations = explanations.concat(branchLabelsWithExplain.explanation);
			} else {
				splitLabels.push(splitLabel);
			}
		}
		return (explain>0?
				{classes: splitLabels, explanation: explanations}:
				splitLabels);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Homer.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
		this.allClasses = json.allClasses;
		this.root = this.fromJSONRecursive(json);
	}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Homer.prototype.fromJSONRecursive"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>fromJSONRecursive (treeNodeJson)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.fromJSONRecursive)
- description and source-code
```javascript
fromJSONRecursive = function (treeNodeJson) {
		var treeNode = {
			mapSuperlabelToBranch: {}
		};
		treeNode.superlabelClassifier =  this.newMultilabelClassifier();
		treeNode.superlabelClassifier.fromJSON(treeNodeJson.superlabelClassifier);
		for (var superlabel in treeNodeJson.mapSuperlabelToBranch)
			treeNode.mapSuperlabelToBranch[superlabel] =
				this.fromJSONRecursive(treeNodeJson.mapSuperlabelToBranch[superlabel]);
		return treeNode;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Homer.prototype.getAllClasses"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.getAllClasses)
- description and source-code
```javascript
getAllClasses = function () {
		return Object.keys(this.allClasses);
	}
```
- example usage
```shell
...
		if (this.pastTrainingSamples) this.pastTrainingSamples = json.pastTrainingSamples;
		this.featureDocumentFrequency = json.featureDocumentFrequency;
		this.documentCount = json.documentCount;
		/* Note: the feature extractors are functions - they should be created at initialization - they are not deserializable! */
	},

	getAllClasses: function() {  // relevant for multilabel classifiers
		return this.classifier.getAllClasses();
	},
}  // end of EnhancedClassifier prototype


var stringifyClass = function (aClass) {
	return (_(aClass).isString()? aClass: JSON.stringify(aClass));
}
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Homer.prototype.newMultilabelClassifier"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>newMultilabelClassifier ()](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.newMultilabelClassifier)
- description and source-code
```javascript
newMultilabelClassifier = function () {
		var classifier = new this.multilabelClassifierType();
		if (this.featureLookupTable && classifier.setFeatureLookupTable)
			classifier.setFeatureLookupTable(this.featureLookupTable);
		return classifier;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Homer.prototype.setFeatureLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.setFeatureLookupTable)
- description and source-code
```javascript
setFeatureLookupTable = function (featureLookupTable) {
		//console.log("HOMER setFeatureLookupTable "+featureLookupTable);
		this.featureLookupTable = featureLookupTable;
		this.setFeatureLookupTableRecursive(featureLookupTable, this.root);
	}
```
- example usage
```shell
...

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
	this.tfidf = new opts.TfIdfImpl
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Homer.prototype.setFeatureLookupTableRecursive"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>setFeatureLookupTableRecursive (featureLookupTable, treeNode)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.setFeatureLookupTableRecursive)
- description and source-code
```javascript
setFeatureLookupTableRecursive = function (featureLookupTable, treeNode) {
		if (treeNode.superlabelClassifier && treeNode.superlabelClassifier.setFeatureLookupTable)
			treeNode.superlabelClassifier.setFeatureLookupTable(featureLookupTable);
		for (var superlabel in treeNode.mapSuperlabelToBranch)
			this.setFeatureLookupTableRecursive(featureLookupTable, treeNode.mapSuperlabelToBranch[superlabel]);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Homer.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
		var json = this.toJSONRecursive(this.root);
		json.allClasses = this.allClasses;
		return json;
	}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Homer.prototype.toJSONRecursive"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>toJSONRecursive (treeNode)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.toJSONRecursive)
- description and source-code
```javascript
toJSONRecursive = function (treeNode) {
		var treeNodeJson = {
			superlabelClassifier: treeNode.superlabelClassifier.toJSON(),
			mapSuperlabelToBranch: {}
		};
		for (var superlabel in treeNode.mapSuperlabelToBranch) {
			treeNodeJson.mapSuperlabelToBranch[superlabel] = this.toJSONRecursive(treeNode.mapSuperlabelToBranch[superlabel]);
		}
		return treeNodeJson;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Homer.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
		dataset = dataset.map(function(datum) {
			var normalizedLabels = multilabelutils.normalizeOutputLabels(datum.output);
			for (var i in normalizedLabels)
				this.allClasses[normalizedLabels[i]]=true;
			return {
				input: datum.input,
				output: normalizedLabels.map(this.splitLabel)
			}
		}, this);
		
		// [ [ 'Offer', 'Leased Car', 'Without leased car' ], [ 'Offer', 'Working Hours', '9 hours' ] ]
		
		return this.trainBatchRecursive(dataset, this.root);
	}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Homer.prototype.trainBatchRecursive"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>trainBatchRecursive (dataset, treeNode)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.trainBatchRecursive)
- description and source-code
```javascript
trainBatchRecursive = function (dataset, treeNode) {
		var superlabelsDataset = [];
		var mapSuperlabelToRestDataset = {};
		dataset.forEach(function(datum) {
			var splitLabels = datum.output;	// [ [ 'Offer', 'Leased Car', 'Without leased car' ], [ 'Offer', 'Working Hours', '9 hours' ] ]
			var superlabels = {};           // the first parts of each of the splitLabels
			var mapSuperlabelToRest = {};   // each value is a list of continuations of the key.
			for (var i in splitLabels) {
				var splitLabel = splitLabels[i];//[ 'Offer', 'Leased Car', 'Without leased car' ]
				var superlabel = splitLabel[0];
				superlabels[superlabel] = true; //superlabels['Offer'] = true
				if (splitLabel.length>1) { 		// if it have more than one label (superlabel)
					if (!mapSuperlabelToRest[superlabel])
						mapSuperlabelToRest[superlabel] = [];
					mapSuperlabelToRest[superlabel].push(splitLabel.slice(1));//['Leased Car', 'Without leased car']
				}
			}

<span class="apidocCodeCommentSpan">/*			Sample of mapSuperlabelToRest
			{ Offer:
			[ [ 'Leased Car', 'Without leased car' ],
   			  [ 'Working Hours', '9 hours' ] ] }

			Sample of superlabelsDataset, initial dataset with superlabel instead of entire output
			'. [end]': 0.965080896043587 },
			output: [ 'Offer' ] } ]
*/
</span>			superlabelsDataset.push({
				input: datum.input,
				output: Object.keys(superlabels)
			});		

			for (var superlabel in mapSuperlabelToRest) {
				if (!(superlabel in mapSuperlabelToRestDataset))
					mapSuperlabelToRestDataset[superlabel] = [];
				mapSuperlabelToRestDataset[superlabel].push({
					input: datum.input,
					output: mapSuperlabelToRest[superlabel]
				});
			}
		}, this);
		
/*		Sample of mapSuperlabelToRestDataset
		{ Offer: [ { input: [Object], output: [["Leased Car","Without leased car"],["Working Hours","9 hours"]] } ] }
*/

		// train the classifier only on superlabels
		treeNode.superlabelClassifier.trainBatch(superlabelsDataset);

		for (var superlabel in mapSuperlabelToRestDataset) {
			if (!(superlabel in treeNode.mapSuperlabelToBranch)) {
				treeNode.mapSuperlabelToBranch[superlabel] = {
					superlabelClassifier: this.newMultilabelClassifier(),
					mapSuperlabelToBranch: {}
				}
			}
/*			train the next level classifier for a give superlabel classifier superlabel (from loop)
			with the dataset from new structure mapSuperlabelToRestDataset (see above)
*/			this.trainBatchRecursive(mapSuperlabelToRestDataset[superlabel], treeNode.mapSuperlabelToBranch[superlabel]);
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Homer.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>trainOnline (sample, labels)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (sample, labels) {
		labels = multilabelutils.normalizeOutputLabels(labels);
		
		for (var i in labels)
			this.allClasses[labels[i]]=true;
		
		return this.trainOnlineRecursive(
				sample,
				labels.map(this.splitLabel),
				this.root);
	}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.Homer.prototype.trainOnlineRecursive"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.Homer.prototype.</span>trainOnlineRecursive (sample, splitLabels, treeNode)](#apidoc.element.limdu.classifiers.multilabel.Homer.prototype.trainOnlineRecursive)
- description and source-code
```javascript
trainOnlineRecursive = function (sample, splitLabels, treeNode) {
		var superlabels = {}; // the first parts of each of the splitLabels
		var mapSuperlabelToRest = {};   // each value is a list of continuations of the key.
		for (var i in splitLabels) {
			var splitLabel = splitLabels[i];
			var superlabel = splitLabel[0];
			superlabels[superlabel] = true;
			if (splitLabel.length>1) {
				if (!mapSuperlabelToRest[superlabel])
					mapSuperlabelToRest[superlabel] = [];
				mapSuperlabelToRest[superlabel].push(splitLabel.slice(1));
			}
		}

		treeNode.superlabelClassifier.trainOnline(sample, Object.keys(superlabels));
		for (var superlabel in mapSuperlabelToRest) {
			if (!(superlabel in treeNode.mapSuperlabelToBranch)) {
				treeNode.mapSuperlabelToBranch[superlabel] = {
					superlabelClassifier: this.newMultilabelClassifier(),
					mapSuperlabelToBranch: {}
				}
			}
			this.trainOnlineRecursive(sample, mapSuperlabelToRest[superlabel], treeNode.mapSuperlabelToBranch[superlabel]);
		}
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.classifiers.multilabel.MetaLabeler.prototype"></a>[module limdu.classifiers.multilabel.MetaLabeler.prototype](#apidoc.module.limdu.classifiers.multilabel.MetaLabeler.prototype)

#### <a name="apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MetaLabeler.prototype.</span>classify (sample, explain)](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.classify)
- description and source-code
```javascript
classify = function (sample, explain) {
		var rankedLabelsWithExplain = this.ranker.classify(sample, explain, /*withScores=*/true);
		var rankedLabels = (explain>0? rankedLabelsWithExplain.classes: rankedLabelsWithExplain);
		var labelCountWithExplain = this.counter.classify(sample, explain, /*withScores=*/true);
		var labelCount = (explain>0? labelCountWithExplain.classes[0][0]: labelCountWithExplain[0][0]);
		if (_.isString(labelCount)) labelCount = parseInt(labelCount);
		
		// Pick the labelCount most relevant labels from the list returned by the ranker:
		var positiveLabelsWithScores = rankedLabels.slice(0, labelCount);

		var positiveLabels = positiveLabelsWithScores

		if (positiveLabelsWithScores.length != 0)
			if (_.isArray(positiveLabelsWithScores[0]))
				var positiveLabels = positiveLabelsWithScores.map(function(labelWithScore) {return labelWithScore[0]});
		
		return (explain>0? {
			classes: positiveLabels,
			explanation: {
				ranking: rankedLabelsWithExplain.explanation,
				counting: labelCountWithExplain.explanation
			}
		}:
		positiveLabels)
	}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MetaLabeler.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MetaLabeler.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
	}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.getAllClasses"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MetaLabeler.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.getAllClasses)
- description and source-code
```javascript
getAllClasses = function () {
		return this.ranker.getAllClasses();
	}
```
- example usage
```shell
...
		if (this.pastTrainingSamples) this.pastTrainingSamples = json.pastTrainingSamples;
		this.featureDocumentFrequency = json.featureDocumentFrequency;
		this.documentCount = json.documentCount;
		/* Note: the feature extractors are functions - they should be created at initialization - they are not deserializable! */
	},

	getAllClasses: function() {  // relevant for multilabel classifiers
		return this.classifier.getAllClasses();
	},
}  // end of EnhancedClassifier prototype


var stringifyClass = function (aClass) {
	return (_(aClass).isString()? aClass: JSON.stringify(aClass));
}
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.setFeatureLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MetaLabeler.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.setFeatureLookupTable)
- description and source-code
```javascript
setFeatureLookupTable = function (featureLookupTable) {
		if (this.ranker.setFeatureLookupTable)
			this.ranker.setFeatureLookupTable(featureLookupTable);
		if (this.counter.setFeatureLookupTable)
			this.counter.setFeatureLookupTable(featureLookupTable);
	}
```
- example usage
```shell
...

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
	this.tfidf = new opts.TfIdfImpl
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MetaLabeler.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
	}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MetaLabeler.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
		// The ranker is just trained by the given set of labels relevant to each sample:
		this.ranker.trainBatch(dataset);

		// The counter is trained by the *number* of labels relevant to each sample:
		var labelCountDataset = dataset.map(function(datum) {
			var labelCount = (Array.isArray(datum.output)? datum.output.length: 1);
			return {
				input: datum.input,
				output: labelCount
			};
		});
		this.counter.trainBatch(labelCountDataset);
	}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MetaLabeler.prototype.</span>trainOnline (sample, labels)](#apidoc.element.limdu.classifiers.multilabel.MetaLabeler.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (sample, labels) {
		// The ranker is just trained by the given set of relevant labels:
		this.ranker.trainOnline(sample, labels);

		// The counter is trained by the *number* of relevant labels:
		var labelCount = (Array.isArray(labels)? labels: Object.keys(labels)).length;
		this.counter.trainOnline(sample, labelCount);
	}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```



# <a name="apidoc.module.limdu.classifiers.multilabel.MulticlassSegmentation.prototype"></a>[module limdu.classifiers.multilabel.MulticlassSegmentation.prototype](#apidoc.module.limdu.classifiers.multilabel.MulticlassSegmentation.prototype)

#### <a name="apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.bestClassOfSegment"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>bestClassOfSegment (segment)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.bestClassOfSegment)
- description and source-code
```javascript
bestClassOfSegment = function (segment) {
		var sample = this.sampleToFeatures(segment, this.featureExtractor);
		var classification = this.multiclassClassifier.classify(sample, 1);
		//console.log(segment+": ");	console.dir(classification)
		return classification;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.cheapestSegmentSplitStrategy"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>cheapestSegmentSplitStrategy (words, accumulatedClasses, explain, explanations)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.cheapestSegmentSplitStrategy)
- description and source-code
```javascript
cheapestSegmentSplitStrategy = function (words, accumulatedClasses, explain, explanations) {
		
		// Calculate the cost of classification of the segment from i to j.
		// (Cost = - log probability).
		var segmentClassificationCosts = [];  // best cost to classify segment [i,j]
		for (var start=0; start<=words.length; ++start) {
			segmentClassificationCosts[start] = [];
			for (var end=0; end<start; ++end)
				segmentClassificationCosts[start][end]=Infinity;
			segmentClassificationCosts[start][start]=0;
			for (var end=start+1; end<=words.length; ++end) {
				var segment = words.slice(start,end).join(" ");
				var classification = this.bestClassOfSegment(segment);
				segmentClassificationCosts[start][end] = -Math.log(classification.probability);
			}
		}
		//console.log(words+":  ");		console.log("segmentClassificationCosts");		console.dir(segmentClassificationCosts);
		var cheapest_paths = require("graph-paths").cheapest_paths;
		cheapestSegmentClassificationCosts = cheapest_paths(segmentClassificationCosts, 0);
		cheapestSentenceClassificationCost = cheapestSegmentClassificationCosts[words.length];
		if (!cheapestSentenceClassificationCost)
			throw new Error("cheapestSegmentClassificationCosts["+words.length+"] is empty");
		//console.log("cheapestSentenceClassificationCost");		console.dir(cheapestSentenceClassificationCost);
		
		var cheapestClassificationPath = cheapestSentenceClassificationCost.path;
		explanations.push(cheapestSentenceClassificationCost);
		for (var i=0; i<cheapestClassificationPath.length-1; ++i) {
			var segment = words.slice(cheapestClassificationPath[i],cheapestClassificationPath[i+1]).join(" ");
			//console.log(segment+":  ");
			var segmentCategoryWithExplain = this.classifySegment(segment, explain);
			//console.dir(segmentCategoryWithExplain);
			var segmentCategory = (segmentCategoryWithExplain.category? segmentCategoryWithExplain.category: segmentCategoryWithExplain);
			accumulatedClasses[segmentCategory]=true;
			if (explain>0) {
				explanations.push(segment);
				explanations.push(segmentCategoryWithExplain.explanation);
			};
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>classify (sentence, explain)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.classify)
- description and source-code
```javascript
classify = function (sentence, explain) {
		var minWordsToSplit = 2;
		var words = sentence.split(/ /);
		if (words.length>=minWordsToSplit) {
			var accumulatedClasses = {};
			var explanations = [];
			this.cheapestSegmentSplitStrategy(words, accumulatedClasses, explain, explanations);
			
			var classes = Object.keys(accumulatedClasses);
			return (explain>0?	{
				classes: classes,
				explanation: explanations
			}:
			classes);
		} else {
			return this.classifySegment(sentence, explain);
		}
	}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.classifySegment"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>classifySegment (segment, explain)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.classifySegment)
- description and source-code
```javascript
classifySegment = function (segment, explain) {
		var sample = this.sampleToFeatures(segment, this.featureExtractor);
		return this.multiclassClassifier.classify(sample, explain);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
		this.multiclassClassifier.fromJSON(json);
	}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.sampleToFeatures"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>sampleToFeatures (sample, featureExtractor)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.sampleToFeatures)
- description and source-code
```javascript
sampleToFeatures = function (sample, featureExtractor) {
		var features = sample;
		if (featureExtractor) {
			try {
				features = {};
				featureExtractor(sample, features);
			} catch (err) {
				throw new Error("Cannot extract features from '"+JSON.stringify(sample)+"': "+JSON.stringify(err));
			}
		}
		return features;
	}
```
- example usage
```shell
...
	 * Tell the classifier that the given sample belongs to the given classes.
	 * @param sample a document.
	 * @param classes an array whose VALUES are classes.
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
		return this.multiclassClassifier.toJSON();
	}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
		for ( var i = 0; i < dataset.length; ++i) {
			dataset[i] = {
				input: this.sampleToFeatures(dataset[i].input, this.featureExtractor),
				output: (Array.isArray(dataset[i].output)? dataset[i].output[0]: dataset[i].output)
			};
		}
		
		this.multiclassClassifier.trainBatch(dataset);
	}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.MulticlassSegmentation.prototype.</span>trainOnline (sample, classes)](#apidoc.element.limdu.classifiers.multilabel.MulticlassSegmentation.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (sample, classes) {
		sample = this.sampleToFeatures(sample, this.featureExtractor);
		var category = (Array.isArray(classes)? classes[0]: classes);
		this.multiclassClassifier.trainOnline(sample, category);
		<span class="apidocCodeCommentSpan">/*for (var positiveClass in classes) {
			this.makeSureClassifierExists(positiveClass);
			this.mapClassnameToClassifier[positiveClass].trainOnline(sample, 1);
		}
		for (var negativeClass in this.mapClassnameToClassifier) {
			if (!classes[negativeClass])
				this.mapClassnameToClassifier[negativeClass].trainOnline(sample, 0);
		}*/
</span>	}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```



# <a name="apidoc.module.limdu.classifiers.multilabel.PartialClassification.prototype"></a>[module limdu.classifiers.multilabel.PartialClassification.prototype](#apidoc.module.limdu.classifiers.multilabel.PartialClassification.prototype)

#### <a name="apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>classify (sample, explain, continuous_output)](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.classify)
- description and source-code
```javascript
classify = function (sample, explain, continuous_output) {
				
		var labels = []
		var explanation = []
		var scores = {}
		
	 	_.each(this.classifier, function(classif, key, list){
	 		var value = classif.classify(sample, explain, continuous_output)
	 	 	if (explain>0)
	 	 		labels.push(value.classes)
	 	 	else
				labels.push(value)
	 	 	explanation.push(value.explanation)
	 	 	scores = _.extend(scores, value.scores)
	 	})

		if (explain>0)
			{
				var positive = {}
				var negative = {}

				_.each(_.pluck(explanation, 'positive'), function(value, key, list){
					positive = _.extend(positive, value)
					}, this)

				_.each(_.pluck(explanation, 'negative'), function(value, key, list){
					negative = _.extend(negative, value)
					}, this)
			

			if (_.keys(negative)!=0)
				explanation = {
					positive: positive,
					negative: negative,
				}
			}

		return (explain>0?
			{
				classes: labels,
				scores: scores,
				explanation: explanation
			}:
			labels);

		
		// console.log(JSON.stringify(explanation, null, 4))
		// return (explain>0?
		// 	{
		// 		classes: labels,
		// 		scores: scores,
		// 		explanation: explanation
		// 	}:
		// 	labels);

	}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
		throw new Error("No implementation in PartialClassification");
	}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.getAllClasses"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.getAllClasses)
- description and source-code
```javascript
getAllClasses = function () {
		throw new Error("No implementation in PartialClassification");
	}
```
- example usage
```shell
...
		if (this.pastTrainingSamples) this.pastTrainingSamples = json.pastTrainingSamples;
		this.featureDocumentFrequency = json.featureDocumentFrequency;
		this.documentCount = json.documentCount;
		/* Note: the feature extractors are functions - they should be created at initialization - they are not deserializable! */
	},

	getAllClasses: function() {  // relevant for multilabel classifiers
		return this.classifier.getAllClasses();
	},
}  // end of EnhancedClassifier prototype


var stringifyClass = function (aClass) {
	return (_(aClass).isString()? aClass: JSON.stringify(aClass));
}
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.intializeClassifiers"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>intializeClassifiers (numberofclassifiers, multilabelClassifierType)](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.intializeClassifiers)
- description and source-code
```javascript
intializeClassifiers = function (numberofclassifiers, multilabelClassifierType) {
		classifier = []
	_(numberofclassifiers).times(function(n){
		classif = new multilabelClassifierType;
		classifier.push(classif);
 	});
 	return classifier
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.setFeatureLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.setFeatureLookupTable)
- description and source-code
```javascript
setFeatureLookupTable = function (featureLookupTable) {
		_.each(this.classifier, function(classif, key, list){
	 		classif.setFeatureLookupTable(featureLookupTable)
	 	})
	}
```
- example usage
```shell
...

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
	this.tfidf = new opts.TfIdfImpl
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
		throw new Error("No implementation in PartialClassification");
	}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
		num_of_classifiers = 0

		_.each(dataset, function(value, key, list){
			num_of_classifiers =  Math.max(num_of_classifiers, (value['output']).length)
		}, this);

			
		_(num_of_classifiers).times(function(n){
			data = []
			_.each(dataset, function(value, key, list){
				if (value.output.length - 1 >= n)
					{
						value1 = _.clone(value)
						value1['output'] = value.output[n]
						data.push(value1)
					}

			 },this)

			// classifier = new this.multilabelClassifierType();
			this.classifier[n].trainBatch(data)
			// classifier.trainBatch(data)
			// this.classifier.push(classifier)
			}, this)
	
	}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PartialClassification.prototype.</span>trainOnline (sample, labels)](#apidoc.element.limdu.classifiers.multilabel.PartialClassification.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (sample, labels) {
		throw new Error("PartialClassification does not support online training");
	}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```



# <a name="apidoc.module.limdu.classifiers.multilabel.PassiveAggressive.prototype"></a>[module limdu.classifiers.multilabel.PassiveAggressive.prototype](#apidoc.module.limdu.classifiers.multilabel.PassiveAggressive.prototype)

#### <a name="apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.addClasses"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>addClasses (classes)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.addClasses)
- description and source-code
```javascript
addClasses = function (classes) {
		classes = hash.normalized(classes);
		for (var aClass in classes) {
			if (!(aClass in this.weights)) {
				this.weights[aClass]={};
				this.weights_sum[aClass]={};
			}
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>classify (features, explain, withScores)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.classify)
- description and source-code
```javascript
classify = function (features, explain, withScores) {
		this.editFeatureValues(features, /*remove_unknown_features=*/true);
		var scoresVector = this.predict(features, /*averaging=*/true, explain);
		return multilabelutils.mapScoresVectorToMultilabelResult(scoresVector, explain, withScores, /*threshold=*/0);
	}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.editFeatureValues"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>editFeatureValues (features, remove_unknown_features)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.editFeatureValues)
- description and source-code
```javascript
editFeatureValues = function (features, remove_unknown_features) {
//		console.log("before: "+util.inspect(features));
//		if (!('bias' in features))
//			features['bias'] = 1.0;
//		if (remove_unknown_features) {
//			for (var feature in features)
//				if (!(feature in this.seenFeatures))
//					delete features[feature];
//		}
//		hash.normalize_sum_of_values_to_1(features);
//		console.log("after: "+util.inspect(features));
	}
```
- example usage
```shell
...
	 */
	trainOnline: function(sample, classes) {
		classes = normalizeClasses(classes, this.labelLookupTable);
		sample = this.normalizedSample(sample);
		var features = this.sampleToFeatures(sample, this.featureExtractors);
		this.countFeatures(features);
		this.trainSpellChecker(features);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		var array = this.featuresToArray(features);
		this.classifier.trainOnline(array, classes);
		if (this.pastTrainingSamples)
			this.pastTrainingSamples.push({input: sample, output: classes});
	},

	/**
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>fromJSON (json, callback)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json, callback) {
		this.weights_sum = json.weights_sum;
		this.weights = json.weights;
		this.num_iterations = json.num_iterations;
	}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.getAllClasses"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.getAllClasses)
- description and source-code
```javascript
getAllClasses = function () {
		return Object.keys(this.weights);
	}
```
- example usage
```shell
...
		if (this.pastTrainingSamples) this.pastTrainingSamples = json.pastTrainingSamples;
		this.featureDocumentFrequency = json.featureDocumentFrequency;
		this.documentCount = json.documentCount;
		/* Note: the feature extractors are functions - they should be created at initialization - they are not deserializable! */
	},

	getAllClasses: function() {  // relevant for multilabel classifiers
		return this.classifier.getAllClasses();
	},
}  // end of EnhancedClassifier prototype


var stringifyClass = function (aClass) {
	return (_(aClass).isString()? aClass: JSON.stringify(aClass));
}
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.predict"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>predict (features, averaging, explain)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.predict)
- description and source-code
```javascript
predict = function (features, averaging, explain) {
		var weights_for_classification = (averaging? this.weights_sum: this.weights);
		var scores = {};
		if (explain>0) var explanations = [];
		
//		for (var feature in features) {
//			if (feature in weights_for_classification) {
//				var weight = weights_for_classification[feature];
//				var value = features[feature];
//				var relevance = value * weight;
//				score += relevance;
//				if (explain>0) explanations.push(this.detailed_explanations?
//						{
//							feature: feature,
//							value: value,
//							weight: weight,
//							relevance: relevance,
//						}:
//						sprintf("%s%+1.2f*%+1.2f=%+1.2f", feature, value, weight, relevance);
//				);
//			}
//		}
		
		scores = hash.inner_product_matrix(features, weights_for_classification); // scores is a map: category=>score
		var scoresVector = _.pairs(scores); // scoresVector is an array of pairs [category,score]
		scoresVector.sort(function(a,b) {return b[1]-a[1]}); // sort by decreasing score
		return scoresVector;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>toJSON (callback)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.toJSON)
- description and source-code
```javascript
toJSON = function (callback) {
		return {
			weights_sum: this.weights_sum,
			weights: this.weights,
			num_iterations: this.num_iterations,
		}
	}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {
		// preprocessing: add all the classes in the dataset to the weights vector;
		dataset.forEach(function(datum) {
			this.addClasses(datum.output);
			this.editFeatureValues(datum.input, /*remove_unknown_features=*/false);
		}, this);

		for (var i=0; i<this.retrain_count; ++i)
			dataset.forEach(function(datum) {
				this.update(datum.input, datum.output);
			}, this);
	}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>trainOnline (features, classes)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (features, classes) {
		this.addClasses(classes);
		this.editFeatureValues(features, /*remove_unknown_features=*/false);
		this.update(features, classes);
	}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.update"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.PassiveAggressive.prototype.</span>update (sample, classes)](#apidoc.element.limdu.classifiers.multilabel.PassiveAggressive.prototype.update)
- description and source-code
```javascript
update = function (sample, classes) {
		var classesSet = hash.normalized(classes);

		var ranks = this.predict(sample, /*averaging=*/false);  // pairs of [class,score] sorted by decreasing score

		// find the lowest ranked relevant label r:
		var r = 0
		var r_score = Number.MAX_VALUE
		ranks.forEach(function(labelAndScore) {
			var label = labelAndScore[0];
			var score = labelAndScore[1];
			if ((label in classesSet) && score < r_score) {
				r = label
				r_score = score
			}
		});

		// find the highest ranked irrelevant label s
		var s = 0
		var s_score = -Number.MAX_VALUE
		ranks.reverse();
		ranks.forEach(function(labelAndScore) {
			var label = labelAndScore[0];
			var score = labelAndScore[1];
			if (!(label in classesSet) && score > s_score) {
				s = label;
				s_score = score;
			}
		});

		var loss = Math.max(1.0 - r_score, 0.0) + Math.max(1.0 + s_score, 0.0);
		if (loss > 0) {
			var sample_norm2 = hash.sum_of_square_values(sample);
			var tau = Math.min(this.Constant, loss / sample_norm2);

			if (r_score < Number.MAX_VALUE)
				hash.addtimes(this.weights[r], tau, sample);  // weights[r] += tau*sample
			if (s_score > -Number.MAX_VALUE)
				hash.addtimes(this.weights[s], -tau, sample); // weights[s] -= tau*sample
		}
		// this.weights_sum = (this.weights + this.weights_sum);
		for (category in this.weights)
			hash.add(this.weights_sum[category], this.weights[category]);
		
		hash.add(this.seenFeatures, sample);
		this.num_iterations += 1;
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.classifiers.multilabel.ThresholdClassifier.prototype"></a>[module limdu.classifiers.multilabel.ThresholdClassifier.prototype](#apidoc.module.limdu.classifiers.multilabel.ThresholdClassifier.prototype)

#### <a name="apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.CalculatePerformance"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>CalculatePerformance (list_of_scores, testSet, FN)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.CalculatePerformance)
- description and source-code
```javascript
CalculatePerformance = function (list_of_scores, testSet, FN){

		current_set=[]

		TRUE = 0
		FP = 0
		TP = 0

		result = []
		
		for (var th=0; th<list_of_scores.length; ++th) {

			if (list_of_scores[th][2]=="+") {TP+=1; FN-=1}
			if (list_of_scores[th][2]=="-") {FP+=1;}

			// console.log(list_of_scores[th])
			// console.log("TP "+TP+" FP "+FP+" FN "+FN)

			index_in_testSet = list_of_scores[th][3]

			if (_.isEqual(current_set[index_in_testSet], testSet[index_in_testSet]['output']))
			{TRUE-=1}
			
			if (!current_set[index_in_testSet])
			{current_set[index_in_testSet] = [list_of_scores[th][0]]}
			else
			{current_set[index_in_testSet].push(list_of_scores[th][0])}

 			if (_.isEqual(current_set[index_in_testSet], testSet[index_in_testSet]['output']))
			{TRUE+=1 }
			
 			PRF = calculate_PRF(TP, FP, FN)
 			PRF['Accuracy'] = TRUE/testSet.length
 			PRF['Threshold'] = list_of_scores[th][1]

 			result[list_of_scores[th][1]] = PRF
 			}

			optial_measure=0
			index=Object.keys(result)[0]
			for (i in result)
			{
				if (result[i][this.evaluateMeasureToMaximize] >= optial_measure)
				{
					index = i
					optial_measure = result[i][this.evaluateMeasureToMaximize]
				}
			}

 			return result[index]
 		
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.classify"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>classify (sample, explain)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.classify)
- description and source-code
```javascript
classify = function (sample, explain) {
		return this.multiclassClassifier.classify(sample, explain, /*withScores=*/false);
	}
```
- example usage
```shell
...

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''

Credit: this example uses [brain.js, by Heather Arthur](https://github.com/harthur/brain).


### Online Learning
'''js
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.classifyAndLog"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>classifyAndLog (sample)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.classifyAndLog)
- description and source-code
```javascript
classifyAndLog = function (sample) {
			console.log(sample+" is "+this.classify(sample));
		}
```
- example usage
```shell
...
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
	];
intentClassifier.trainBatch(dataset);

console.log("Original classifier:");
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.trainOnline("I want a doughnut", "dnt");
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifier.retrain();
intentClassifier.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifier.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']

// Serialize the classifier (convert it to a string)
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>fromJSON (json)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
		this.multiclassClassifier.fromJSON(json);
	}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.getAllClasses"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>getAllClasses ()](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.getAllClasses)
- description and source-code
```javascript
getAllClasses = function () {
		return this.multiclassClassifier.getAllClasses();
	}
```
- example usage
```shell
...
		if (this.pastTrainingSamples) this.pastTrainingSamples = json.pastTrainingSamples;
		this.featureDocumentFrequency = json.featureDocumentFrequency;
		this.documentCount = json.documentCount;
		/* Note: the feature extractors are functions - they should be created at initialization - they are not deserializable! */
	},

	getAllClasses: function() {  // relevant for multilabel classifiers
		return this.classifier.getAllClasses();
	},
}  // end of EnhancedClassifier prototype


var stringifyClass = function (aClass) {
	return (_(aClass).isString()? aClass: JSON.stringify(aClass));
}
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.receiveScores"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>receiveScores (dataset)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.receiveScores)
- description and source-code
```javascript
receiveScores = function (dataset) {
		list_of_scores = [];
		FN=0
		for (var i=0; i<dataset.length; ++i)
		{
 			var scoresVector = this.multiclassClassifier.classify(dataset[i].input, false, true);

 			for (score in scoresVector)
 			{
 				if (dataset[i].output.indexOf(scoresVector[score][0])>-1)
 				{
 					scoresVector[score].push("+")
 					FN+=1
 				}
 				else {scoresVector[score].push("-")}

 				scoresVector[score].push(i)	
			}

 			list_of_scores = list_of_scores.concat(scoresVector)
  		}	

  		// list_of_scores = [['d',4],['b',2],['a',1],['c',3]]

		list_of_scores.sort((function(index){
		    return function(a, b){
	        return (a[index] === b[index] ? 0 : (a[index] < b[index] ? 1 : -1));
		    };
		})(1))

		return [list_of_scores, FN]
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.setFeatureLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>setFeatureLookupTable (featureLookupTable)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.setFeatureLookupTable)
- description and source-code
```javascript
setFeatureLookupTable = function (featureLookupTable) {
		if (this.multiclassClassifier.setFeatureLookupTable)
			this.multiclassClassifier.setFeatureLookupTable(featureLookupTable);
	}
```
- example usage
```shell
...

	this.classifier = new opts.classifierType();

	this.inputSplitter = opts.inputSplitter;
	this.setNormalizer(opts.normalizer);
	this.setFeatureExtractor(opts.featureExtractor);
	this.setFeatureExtractorForClassification(opts.featureExtractorForClassification);
	this.setFeatureLookupTable(opts.featureLookupTable);
	this.setLabelLookupTable(opts.labelLookupTable);

	this.multiplyFeaturesByIDF = opts.multiplyFeaturesByIDF;
	this.minFeatureDocumentFrequency = opts.minFeatureDocumentFrequency || 0;
	if (opts.multiplyFeaturesByIDF||opts.minFeatureDocumentFrequency)
		{
	this.tfidf = new opts.TfIdfImpl
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>toJSON ()](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
		return this.multiclassClassifier.toJSON();
	}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.trainBatch"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>trainBatch (dataset)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.trainBatch)
- description and source-code
```javascript
trainBatch = function (dataset) {

		_.times(3, function(n) {dataset = _.shuffle(dataset)})

		if (this.numOfFoldsForThresholdCalculation > 1) {
			thresholds=[]
			best_performances=[]
			average_performances = []
			median_performances = []
			partitions.partitions_consistent(dataset, this.numOfFoldsForThresholdCalculation, (function(trainSet, testSet, index) { 	
				this.multiclassClassifier.trainBatch(trainSet);
				result = this.receiveScores(testSet)
				performance = this.CalculatePerformance(result[0], testSet, result[1])
				best_performances.push(performance)
			}).bind(this))

			this.stats = best_performances
					
			threshold_average = ulist.average(_.pluck(best_performances, 'Threshold'))
			threshold_median = ulist.median(_.pluck(best_performances, 'Threshold'))

			Threshold = threshold_median
		}
		else
		{
			dataset = partitions.partition(dataset, 1, Math.round(dataset.length*this.devsetsize))
			trainSet = dataset['train']
			testSet = dataset['test']
			this.multiclassClassifier.trainBatch(trainSet);
			result = this.receiveScores(testSet)
			performance = this.CalculatePerformance(result[0], testSet, result[1])
			Threshold = performance['Threshold']	
		}

		this.multiclassClassifier.threshold = Threshold
	}
```
- example usage
```shell
...
### Batch Learning - learn from an array of input-output pairs:

'''js
var limdu = require('limdu');

var colorClassifier = new limdu.classifiers.NeuralNetwork();

colorClassifier.trainBatch([
	{input: { r: 0.03, g: 0.7, b: 0.5 }, output: 0},  // black
	{input: { r: 0.16, g: 0.09, b: 0.2 }, output: 1}, // white
	{input: { r: 0.5, g: 0.5, b: 1.0 }, output: 1}   // white
	]);

console.log(colorClassifier.classify({ r: 1, g: 0.4, b: 0 }));  // 0.99 - almost white
'''
...
```

#### <a name="apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.trainOnline"></a>[function <span class="apidocSignatureSpan">limdu.classifiers.multilabel.ThresholdClassifier.prototype.</span>trainOnline (sample, labels)](#apidoc.element.limdu.classifiers.multilabel.ThresholdClassifier.prototype.trainOnline)
- description and source-code
```javascript
trainOnline = function (sample, labels) {
		throw new Error("ThresholdClassifier does not support online training");
	}
```
- example usage
```shell
...
'''js
var birdClassifier = new limdu.classifiers.Winnow({
	default_positive_weight: 1,
	default_negative_weight: 1,
	threshold: 0
});

birdClassifier.trainOnline({'wings': 1, 'flight': 1, 'beak': 1, 'eagle': 1}, 1);  // eagle is a bird (1)
birdClassifier.trainOnline({'wings': 0, 'flight': 0, 'beak': 0, 'dog': 1}, 0);    // dog is not a bird (0)
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1})); // initially, penguin is mistakenly classified
 as 0 - "not a bird"
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 0.5, 'penguin':1}, /*explanation level=*/4)); // why? because
 it does not fly.

birdClassifier.trainOnline({'wings': 1, 'flight': 0, 'beak': 1, 'penguin':1}, 1);  // learn that penguin is a bird, although it
doesn't fly
birdClassifier.trainOnline({'wings': 0, 'flight': 1, 'beak': 0, 'bat': 1}, 0);     // learn that bat is not a bird, although it
does fly
console.dir(birdClassifier.classify({'wings': 1, 'flight': 0, 'beak': 1, 'chicken': 1})); // now, chicken is correctly classified
 as a bird, although it does not fly.
...
```



# <a name="apidoc.module.limdu.features"></a>[module limdu.features](#apidoc.module.limdu.features)

#### <a name="apidoc.element.limdu.features.CollectionOfExtractors"></a>[function <span class="apidocSignatureSpan">limdu.features.</span>CollectionOfExtractors (extractors)](#apidoc.element.limdu.features.CollectionOfExtractors)
- description and source-code
```javascript
CollectionOfExtractors = function (extractors) {
	return function(sample, features) {
		for (var i=0; i<extractors.length; ++i)
			extractors[i](sample, features);
	}
}
```
- example usage
```shell
...
	setFeatureExtractorForClassification: function (featureExtractorForClassification) {
		if (featureExtractorForClassification) {
			if (Array.isArray(featureExtractorForClassification)) {
				featureExtractorForClassification.unshift(this.featureExtractors);
			} else {
				featureExtractorForClassification = [this.featureExtractors, featureExtractorForClassification];
			}
			this.featureExtractorsForClassification = new ftrs.CollectionOfExtractors(featureExtractorForClassification);
		}
	},
	
	setFeatureLookupTable: function(featureLookupTable) {
		if (featureLookupTable) {
			this.featureLookupTable = featureLookupTable;
			if (this.classifier.setFeatureLookupTable)
...
```

#### <a name="apidoc.element.limdu.features.FeatureLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.features.</span>FeatureLookupTable ()](#apidoc.element.limdu.features.FeatureLookupTable)
- description and source-code
```javascript
FeatureLookupTable = function () {
	this.featureIndexToFeatureName = [undefined];
	this.featureNameToFeatureIndex = {undefined: 0};
}
```
- example usage
```shell
...
	binaryClassifierType: limdu.classifiers.SvmJs.bind(0, {C: 1.0})
});

// Initialize a classifier with a feature extractor and a lookup table:
var intentClassifier = new limdu.classifiers.EnhancedClassifier({
	classifierType: TextClassifier,
	featureExtractor: limdu.features.NGramsOfWords(1),  // each word ("1-gram") is a feature
	featureLookupTable: new limdu.features.FeatureLookupTable()
});

// Train and test:
intentClassifier.trainBatch([
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
...
```

#### <a name="apidoc.element.limdu.features.Hypernyms"></a>[function <span class="apidocSignatureSpan">limdu.features.</span>Hypernyms (hypernyms)](#apidoc.element.limdu.features.Hypernyms)
- description and source-code
```javascript
Hypernyms = function (hypernyms) {
	return function(sample, features) {
		hypernyms.forEach(function(hypernym) {
			var matches = null;
			if (!(hypernym.regexp instanceof RegExp))
				hypernym.regexp = new RegExp(hypernym.regexp, "gi");
			if (hypernym.regexp.test(sample))
				features[hypernym.feature]=hypernym.confidence;
		});
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.features.LowerCaseNormalizer"></a>[function <span class="apidocSignatureSpan">limdu.features.</span>LowerCaseNormalizer (sample)](#apidoc.element.limdu.features.LowerCaseNormalizer)
- description and source-code
```javascript
LowerCaseNormalizer = function (sample) {
	return sample.toLowerCase();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.features.NGramsFromArray"></a>[function <span class="apidocSignatureSpan">limdu.features.</span>NGramsFromArray (numOfWords, gap, grams, features)](#apidoc.element.limdu.features.NGramsFromArray)
- description and source-code
```javascript
NGramsFromArray = function (numOfWords, gap, grams, features) {
				for (var i=0; i<numOfWords-1-(gap?1:0); ++i) {
					grams.unshift("[start]");
					grams.push("[end]");
				}
				for (var i=0; i<=grams.length-numOfWords; ++i) {
					sliceOfWords = grams.slice(i, i+numOfWords);
					if (gap) sliceOfWords[1]="-";
					var feature = sliceOfWords.join(" ");
					features[feature.trim()]=1;
				}
				for (var i=0; i<numOfWords-1-(gap?1:0); ++i) {
					grams.pop();
					grams.shift();
				}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.features.NGramsOfLetters"></a>[function <span class="apidocSignatureSpan">limdu.features.</span>NGramsOfLetters (numOfLetters, caseSensitive)](#apidoc.element.limdu.features.NGramsOfLetters)
- description and source-code
```javascript
NGramsOfLetters = function (numOfLetters, caseSensitive) {
	return function(sample, features) {
		if (!caseSensitive) sample=sample.toLowerCase();
		for (var i=0; i<numOfLetters-1; ++i)
			sample = PAD_CHAR+sample+PAD_CHAR;
		for (var firstLetter=0; firstLetter<sample.length-numOfLetters+1; ++firstLetter) {
			var feature = sample.substr(firstLetter, numOfLetters);
			features[feature]=1;
		}
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.features.NGramsOfWords"></a>[function <span class="apidocSignatureSpan">limdu.features.</span>NGramsOfWords (numOfWords, gap)](#apidoc.element.limdu.features.NGramsOfWords)
- description and source-code
```javascript
NGramsOfWords = function (numOfWords, gap) {
			return function(sample, features) {
				var words = sample.split(/[ \t,;:.!?]/).filter(function(a){return !!a}); // all non-empty words
				NGramsFromArray(numOfWords, gap, words, features);
			}
}
```
- example usage
```shell
...
var TextClassifier = limdu.classifiers.multilabel.BinaryRelevance.bind(0, {
	binaryClassifierType: limdu.classifiers.SvmJs.bind(0, {C: 1.0})
});

// Initialize a classifier with a feature extractor and a lookup table:
var intentClassifier = new limdu.classifiers.EnhancedClassifier({
	classifierType: TextClassifier,
	featureExtractor: limdu.features.NGramsOfWords(1),  // each word ("1-gram") is a feature
	featureLookupTable: new limdu.features.FeatureLookupTable()
});

// Train and test:
intentClassifier.trainBatch([
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
...
```

#### <a name="apidoc.element.limdu.features.RegexpNormalizer"></a>[function <span class="apidocSignatureSpan">limdu.features.</span>RegexpNormalizer (normalizations)](#apidoc.element.limdu.features.RegexpNormalizer)
- description and source-code
```javascript
RegexpNormalizer = function (normalizations) {
	return function(sample) {
		normalizations.forEach(function(normalization) {
			var matches = null;
			if (normalization.source instanceof RegExp) {
				if (!normalization.source.global) {
					console.warn("normalization source, "+normalization.source+", is not global - skipping");
					return;
				}
			} else {
				normalization.source = new RegExp(normalization.source,"gi");
			}
			sample = sample.replace(normalization.source, normalization.target);
			//console.log(sample);
		});
		return sample;
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.features.RegexpSplitter"></a>[function <span class="apidocSignatureSpan">limdu.features.</span>RegexpSplitter (regexpString, delimitersToInclude)](#apidoc.element.limdu.features.RegexpSplitter)
- description and source-code
```javascript
RegexpSplitter = function (regexpString, delimitersToInclude) {
	regexpString = "("+regexpString+")";  // to capture the delimiters
	var regexp = new RegExp(regexpString, "i");
	if (!delimitersToInclude) delimitersToInclude = {};
	return function(text) {
		var parts = text.split(regexp);
		var normalizedParts = [];
		for (var i=0; i<parts.length; i+=2) {
			parts[i] = parts[i].trim();
			var part = parts[i];
			if (i+1<parts.length) {
				var delimiter = parts[i+1];
				if (delimitersToInclude[delimiter])
					part += " " + delimiter;
			}
			if (part.length>0)
				normalizedParts.push(part);
		}
		//console.log(text);
		//console.dir(normalizedParts);
		return normalizedParts;
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.features.call"></a>[function <span class="apidocSignatureSpan">limdu.features.</span>call (featureExtractor, sample)](#apidoc.element.limdu.features.call)
- description and source-code
```javascript
call = function (featureExtractor, sample) {
	var features = {};
	featureExtractor(sample, features);
	return features;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.features.normalize"></a>[function <span class="apidocSignatureSpan">limdu.features.</span>normalize (featureExtractorOrArray)](#apidoc.element.limdu.features.normalize)
- description and source-code
```javascript
normalize = function (featureExtractorOrArray) {
	return (!featureExtractorOrArray?
				featureExtractorOrArray:
			Array.isArray(featureExtractorOrArray)?
				new module.exports.CollectionOfExtractors(featureExtractorOrArray):
				featureExtractorOrArray);	
}
```
- example usage
```shell
...
}


EnhancedClassifier.prototype = {

	/** Set the main feature extractor, used for both training and classification. */
	setFeatureExtractor: function (featureExtractor) {
		this.featureExtractors = ftrs.normalize(featureExtractor);
	},
	
	/** Set the main feature extractor, used for both training and classification. */
	setNormalizer: function (normalizer) {
		if (normalizer)
			this.normalizers = (Array.isArray(normalizer)? normalizer: [normalizer]);
	},
...
```



# <a name="apidoc.module.limdu.features.FeatureLookupTable"></a>[module limdu.features.FeatureLookupTable](#apidoc.module.limdu.features.FeatureLookupTable)

#### <a name="apidoc.element.limdu.features.FeatureLookupTable.FeatureLookupTable"></a>[function <span class="apidocSignatureSpan">limdu.features.</span>FeatureLookupTable ()](#apidoc.element.limdu.features.FeatureLookupTable.FeatureLookupTable)
- description and source-code
```javascript
FeatureLookupTable = function () {
	this.featureIndexToFeatureName = [undefined];
	this.featureNameToFeatureIndex = {undefined: 0};
}
```
- example usage
```shell
...
	binaryClassifierType: limdu.classifiers.SvmJs.bind(0, {C: 1.0})
});

// Initialize a classifier with a feature extractor and a lookup table:
var intentClassifier = new limdu.classifiers.EnhancedClassifier({
	classifierType: TextClassifier,
	featureExtractor: limdu.features.NGramsOfWords(1),  // each word ("1-gram") is a feature
	featureLookupTable: new limdu.features.FeatureLookupTable()
});

// Train and test:
intentClassifier.trainBatch([
	{input: "I want an apple", output: "apl"},
	{input: "I want a banana", output: "bnn"},
	{input: "I want chips", output: "cps"},
...
```



# <a name="apidoc.module.limdu.features.FeatureLookupTable.prototype"></a>[module limdu.features.FeatureLookupTable.prototype](#apidoc.module.limdu.features.FeatureLookupTable.prototype)

#### <a name="apidoc.element.limdu.features.FeatureLookupTable.prototype.addFeature"></a>[function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>addFeature (feature)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.addFeature)
- description and source-code
```javascript
addFeature = function (feature) {
		if (!(feature in this.featureNameToFeatureIndex)) {
			var newIndex = this.featureIndexToFeatureName.length;
			this.featureIndexToFeatureName.push(feature);
			this.featureNameToFeatureIndex[feature] = newIndex;
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.features.FeatureLookupTable.prototype.addFeatures"></a>[function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>addFeatures (hash)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.addFeatures)
- description and source-code
```javascript
addFeatures = function (hash) {
		if (hash instanceof Array) {
			for (var index in hash)
				this.addFeature(hash[index]);
		} else if (hash instanceof Object) {
			for (var feature in hash)
				this.addFeature(feature);
		}
		else throw new Error("FeatureLookupTable.addFeatures expects a hash or an array, but got: "+JSON.stringify(hash));
	}
```
- example usage
```shell
...

				var features = this.sampleToFeatures(datum.input, this.featureExtractors);
				
				if (this.tfidf)
					this.tfidf.addDocument(features);
				// this.trainSpellChecker(features);
				if (featureLookupTable)
					featureLookupTable.addFeatures(features);

				datum.input = features;
				return datum;
			}, this);

			dataset = _.compact(dataset)
...
```

#### <a name="apidoc.element.limdu.features.FeatureLookupTable.prototype.addFeaturess"></a>[function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>addFeaturess (hashes)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.addFeaturess)
- description and source-code
```javascript
addFeaturess = function (hashes) {
		for (var i=0; i<hashes.length; ++i)
			this.addFeatures(hashes[i]);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.features.FeatureLookupTable.prototype.arrayToHash"></a>[function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>arrayToHash (array)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.arrayToHash)
- description and source-code
```javascript
arrayToHash = function (array) {
		var hash = {};
		for (var feature in this.featureNameToFeatureIndex) {
			if (array[this.featureNameToFeatureIndex[feature]])
				hash[feature] = array[this.featureNameToFeatureIndex[feature]];
		}
		return hash;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.features.FeatureLookupTable.prototype.arraysToHashes"></a>[function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>arraysToHashes (arrays)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.arraysToHashes)
- description and source-code
```javascript
arraysToHashes = function (arrays) {
		var hashes = [];
		for (var i=0; i<arrays.length; ++i)
			hashes[i] = this.arrayToHash(arrays[i]);
		return hashes;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.features.FeatureLookupTable.prototype.featureToNumber"></a>[function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>featureToNumber (feature)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.featureToNumber)
- description and source-code
```javascript
featureToNumber = function (feature) {
		this.addFeature(feature);
		return this.featureNameToFeatureIndex[feature];
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.features.FeatureLookupTable.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>fromJSON (json)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
		this.featureIndexToFeatureName = json.featureIndexToFeatureName;
		this.featureNameToFeatureIndex = json.featureNameToFeatureIndex;
	}
```
- example usage
```shell
...
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
		};
	},

	fromJSON : function(json) {
		this.classifier.fromJSON(json.classifier);
		if (this.featureLookupTable) {
			this.featureLookupTable.fromJSON(json.featureLookupTable);
			this.setFeatureLookupTable(this.featureLookupTable);
		}
		if (this.labelLookupTable) {
			this.labelLookupTable.fromJSON(json.labelLookupTable);
			this.setLabelLookupTable(this.labelLookupTable);
...
```

#### <a name="apidoc.element.limdu.features.FeatureLookupTable.prototype.hashToArray"></a>[function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>hashToArray (hash)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.hashToArray)
- description and source-code
```javascript
hashToArray = function (hash) {
		this.addFeatures(hash);
		var array = [];
		for (var featureIndex=0; featureIndex<this.featureIndexToFeatureName.length; ++featureIndex)
			array[featureIndex]=0;
		if (hash instanceof Array) {
			for (var i in hash)
				array[this.featureNameToFeatureIndex[hash[i]]] = true;
		} else if (hash instanceof Object) {
			for (var feature in hash)
				array[this.featureNameToFeatureIndex[feature]] = hash[feature];
		}
		else throw new Error("Unsupported type: "+JSON.stringify(hash));
		return array;
	}
```
- example usage
```shell
...
		}
		return sample
	},
	
	featuresToArray: function(features) {
		var array = features;
		if (this.featureLookupTable) {
			array = this.featureLookupTable.hashToArray(features);
		}
		return array;
	},
	
	countFeatures: function(features) {
		if (this.featureDocumentFrequency) {
			// this.tfidf.addDocument(datum.input);
...
```

#### <a name="apidoc.element.limdu.features.FeatureLookupTable.prototype.hashesToArrays"></a>[function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>hashesToArrays (hashes)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.hashesToArrays)
- description and source-code
```javascript
hashesToArrays = function (hashes) {
		this.addFeaturess(hashes);
	
		var arrays = [];
		for (var i=0; i<hashes.length; ++i) {
			arrays[i] = [];
			for (var feature in this.featureNameToFeatureIndex)
				arrays[i][this.featureNameToFeatureIndex[feature]] = hashes[i][feature] || 0;
		}
		return arrays;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.features.FeatureLookupTable.prototype.numberToFeature"></a>[function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>numberToFeature (number)](#apidoc.element.limdu.features.FeatureLookupTable.prototype.numberToFeature)
- description and source-code
```javascript
numberToFeature = function (number) {
		return this.featureIndexToFeatureName[number];
	}
```
- example usage
```shell
...
			}
		}

		if (this.labelLookupTable) {
			if (Array.isArray(classes)) {
				classes = classes.map(function(label) {
						if (_.isArray(label))
							label[0] = this.labelLookupTable.numberToFeature(label[0]);
						else
							label = this.labelLookupTable.numberToFeature(label);
						return label;
					}, this);
			} else {
				classes = this.labelLookupTable.numberToFeature(classes);
			}
...
```

#### <a name="apidoc.element.limdu.features.FeatureLookupTable.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.features.FeatureLookupTable.prototype.</span>toJSON ()](#apidoc.element.limdu.features.FeatureLookupTable.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
		return {
			featureIndexToFeatureName: this.featureIndexToFeatureName,
			featureNameToFeatureIndex: this.featureNameToFeatureIndex,
		}
	}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```



# <a name="apidoc.module.limdu.hamming"></a>[module limdu.hamming](#apidoc.module.limdu.hamming)

#### <a name="apidoc.element.limdu.hamming.hammingDistance"></a>[function <span class="apidocSignatureSpan">limdu.hamming.</span>hammingDistance (a, b)](#apidoc.element.limdu.hamming.hammingDistance)
- description and source-code
```javascript
hammingDistance = function (a, b) {
	var d = 0;
	for (var i=0; i<a.length; ++i) {
		if (b.indexOf(a[i])<0)
			d++;
	}
	for (var i=0; i<b.length; ++i) {
		if (a.indexOf(b[i])<0)
			d++;
	}
	return d;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.json"></a>[module limdu.json](#apidoc.module.limdu.json)

#### <a name="apidoc.element.limdu.json.toJSON"></a>[function <span class="apidocSignatureSpan">limdu.json.</span>toJSON (dataset)](#apidoc.element.limdu.json.toJSON)
- description and source-code
```javascript
toJSON = function (dataset) {
	json = "[";
	for (var i=0; i<dataset.length; ++i) {
		json += (
			(i>0? "\n, ": "\n  ")+
			JSON.stringify(dataset[i]));
	}	
	json += "\n]\n";
	return json;
}
```
- example usage
```shell
...
				samples.push(datum.input);
		});
		return samples;
	},

	toJSON : function(callback) {
		return {
			classifier: this.classifier.toJSON(callback),
			featureLookupTable: (this.featureLookupTable? this.featureLookupTable.toJSON(): undefined),
			labelLookupTable: (this.labelLookupTable? this.labelLookupTable.toJSON(): undefined),
			spellChecker:  (this.spellChecker? this.spellChecker/*.toJSON()*/: undefined),
			pastTrainingSamples: (this.pastTrainingSamples? this.pastTrainingSamples: undefined),
			featureDocumentFrequency: this.featureDocumentFrequency,
			documentCount: this.documentCount,
			/* Note: the feature extractors are functions - they should be created at initialization - they are not serializable! */
...
```



# <a name="apidoc.module.limdu.list"></a>[module limdu.list](#apidoc.module.limdu.list)

#### <a name="apidoc.element.limdu.list.average"></a>[function <span class="apidocSignatureSpan">limdu.list.</span>average (list)](#apidoc.element.limdu.list.average)
- description and source-code
```javascript
average = function (list)
	{
		sum = _.reduce(list, function(memo, num){ return memo + num; }, 0);
		return sum/list.length
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.list.clonedataset"></a>[function <span class="apidocSignatureSpan">limdu.list.</span>clonedataset (set)](#apidoc.element.limdu.list.clonedataset)
- description and source-code
```javascript
clonedataset = function (set)
	{
	set1 = []
	_.each(set, function(value, key, list){
		set1.push(_.clone(value))
		})
	return set1
	}
```
- example usage
```shell
...
			// else
				// classification.explanation['SpellCorrectedFeatures']=JSON.stringify(features);
		// }
		return classification;
	},

	outputToFormat: function(data) {
		dataset = util.clonedataset(data)
		dataset = dataset.map(function(datum) {
		var normalizedLabels = multilabelutils.normalizeOutputLabels(datum.output);
		return {
			input: datum.input,
			output: this.TestSplitLabel(normalizedLabels)
		}
		}, this);
...
```

#### <a name="apidoc.element.limdu.list.listembed"></a>[function <span class="apidocSignatureSpan">limdu.list.</span>listembed (label)](#apidoc.element.limdu.list.listembed)
- description and source-code
```javascript
listembed = function (label)
	{
		if ((label === null) || (label == undefined) || (typeof label == 'undefined'))
			return [[]]
		// if (typeof label != 'undefined')
		// else
		// {
		if ((_.isObject(label))&&!(_.isArray(label)))
		// if ('classes' in JSON.parse(label))
		if ('classes' in label)
			label = label.classes

		if (!(label[0] instanceof Array))
			return [label]
		else
			return label
		// }
		// else
		// {
			// return [label]
		// }
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.list.median"></a>[function <span class="apidocSignatureSpan">limdu.list.</span>median (values)](#apidoc.element.limdu.list.median)
- description and source-code
```javascript
median = function (values) {
 	    values.sort(function(a,b) {return a - b;} );
	    var half = Math.floor(values.length/2);
	    if(values.length % 2)
	        return values[half];
	    else
	        return (values[half-1] + values[half]) / 2.0;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.list.variance"></a>[function <span class="apidocSignatureSpan">limdu.list.</span>variance (list)](#apidoc.element.limdu.list.variance)
- description and source-code
```javascript
variance = function (list)
	{
		sum = _.reduce(list, function(memo, num){ return memo + num; }, 0);
		exp = sum/list.length
		sum2 = _.reduce(list, function(memo, num){ return memo + num*num; }, 0);
		exp2 = sum2/list.length
		return exp2-exp*exp
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.svmlight"></a>[module limdu.svmlight](#apidoc.module.limdu.svmlight)

#### <a name="apidoc.element.limdu.svmlight.toSvmLight"></a>[function <span class="apidocSignatureSpan">limdu.svmlight.</span>toSvmLight (dataset, bias, binarize, firstFeatureNumber)](#apidoc.element.limdu.svmlight.toSvmLight)
- description and source-code
```javascript
toSvmLight = function (dataset, bias, binarize, firstFeatureNumber) {
	var lines = "";
	for (var i=0; i<dataset.length; ++i) {
		var line = (i>0? "\n": "") +
			(binarize? (dataset[i].output>0? "1": "-1"): dataset[i].output) +  // in svm-light, the output comes first:
			featureArrayToFeatureString(dataset[i].input, bias, firstFeatureNumber)
			;
		lines += line;
	};
	lines += "\n";
	return lines;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.tsv"></a>[module limdu.tsv](#apidoc.module.limdu.tsv)

#### <a name="apidoc.element.limdu.tsv.toTSV"></a>[function <span class="apidocSignatureSpan">limdu.tsv.</span>toTSV (dataset, separator)](#apidoc.element.limdu.tsv.toTSV)
- description and source-code
```javascript
toTSV = function (dataset, separator) {
	if (!separator) separator="\t";
	dataset.forEach(function(sample) {
		console.log(JSON.stringify(sample.input)+separator+"["+sample.output+"]");
	});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.utils"></a>[module limdu.utils](#apidoc.module.limdu.utils)

#### <a name="apidoc.element.limdu.utils.PrecisionRecall"></a>[function <span class="apidocSignatureSpan">limdu.utils.</span>PrecisionRecall ()](#apidoc.element.limdu.utils.PrecisionRecall)
- description and source-code
```javascript
PrecisionRecall = function () {
	this.labels = {}
	this.confusion = {} // only in single label case
	
	this.count = 0;
	this.TRUE = 0;
	this.startTime = new Date();
}
```
- example usage
```shell
...
var IntentClassifier = limdu.classifiers.EnhancedClassifier.bind(0, {
	classifierType: limdu.classifiers.multilabel.BinaryRelevance.bind(0, {
		binaryClassifierType: limdu.classifiers.Winnow.bind(0, {retrain_count: 10})
	}),
	featureExtractor: limdu.features.NGramsOfWords(1),
});

var microAverage = new limdu.utils.PrecisionRecall();
var macroAverage = new limdu.utils.PrecisionRecall();

limdu.utils.partitions.partitions(dataset, numOfFolds, function(trainSet, testSet) {
	console.log("Training on "+trainSet.length+" samples, testing on "+testSet.length+" samples");
	var classifier = new IntentClassifier();
	classifier.trainBatch(trainSet);
	limdu.utils.test(classifier, testSet, /* verbosity = */0,
...
```

#### <a name="apidoc.element.limdu.utils.hammingDistance"></a>[function <span class="apidocSignatureSpan">limdu.utils.</span>hammingDistance (a, b)](#apidoc.element.limdu.utils.hammingDistance)
- description and source-code
```javascript
hammingDistance = function (a, b) {
	var d = 0;
	for (var i=0; i<a.length; ++i) {
		if (b.indexOf(a[i])<0)
			d++;
	}
	for (var i=0; i<b.length; ++i) {
		if (a.indexOf(b[i])<0)
			d++;
	}
	return d;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.utils.PrecisionRecall"></a>[module limdu.utils.PrecisionRecall](#apidoc.module.limdu.utils.PrecisionRecall)

#### <a name="apidoc.element.limdu.utils.PrecisionRecall.PrecisionRecall"></a>[function <span class="apidocSignatureSpan">limdu.utils.</span>PrecisionRecall ()](#apidoc.element.limdu.utils.PrecisionRecall.PrecisionRecall)
- description and source-code
```javascript
PrecisionRecall = function () {
	this.labels = {}
	this.confusion = {} // only in single label case
	
	this.count = 0;
	this.TRUE = 0;
	this.startTime = new Date();
}
```
- example usage
```shell
...
var IntentClassifier = limdu.classifiers.EnhancedClassifier.bind(0, {
	classifierType: limdu.classifiers.multilabel.BinaryRelevance.bind(0, {
		binaryClassifierType: limdu.classifiers.Winnow.bind(0, {retrain_count: 10})
	}),
	featureExtractor: limdu.features.NGramsOfWords(1),
});

var microAverage = new limdu.utils.PrecisionRecall();
var macroAverage = new limdu.utils.PrecisionRecall();

limdu.utils.partitions.partitions(dataset, numOfFolds, function(trainSet, testSet) {
	console.log("Training on "+trainSet.length+" samples, testing on "+testSet.length+" samples");
	var classifier = new IntentClassifier();
	classifier.trainBatch(trainSet);
	limdu.utils.test(classifier, testSet, /* verbosity = */0,
...
```



# <a name="apidoc.module.limdu.utils.PrecisionRecall.prototype"></a>[module limdu.utils.PrecisionRecall.prototype](#apidoc.module.limdu.utils.PrecisionRecall.prototype)

#### <a name="apidoc.element.limdu.utils.PrecisionRecall.prototype.addCase"></a>[function <span class="apidocSignatureSpan">limdu.utils.PrecisionRecall.prototype.</span>addCase (expected, actual)](#apidoc.element.limdu.utils.PrecisionRecall.prototype.addCase)
- description and source-code
```javascript
addCase = function (expected, actual) {
		this.count++;
		if (expected && actual) this.TP++;
		if (!expected && actual) this.FP++;
		if (expected && !actual) this.FN++;
		if (!expected && !actual) this.TN++;
		if (expected==actual) this.TRUE++;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.PrecisionRecall.prototype.addCases"></a>[function <span class="apidocSignatureSpan">limdu.utils.PrecisionRecall.prototype.</span>addCases (expectedClasses, actualClasses, logTruePositives)](#apidoc.element.limdu.utils.PrecisionRecall.prototype.addCases)
- description and source-code
```javascript
addCases = function (expectedClasses, actualClasses, logTruePositives) {
		var explanations = [];
		actualClasses = hash.normalized(actualClasses);
		expectedClasses = hash.normalized(expectedClasses);

		var allTrue = true;
		for (var actualClass in actualClasses) {
			if (actualClass in expectedClasses) {
				if (logTruePositives) explanations.push("\t\t+++ TRUE POSITIVE: "+actualClass);
				this.TP++;
			} else {
				explanations.push("\t\t--- FALSE POSITIVE: "+actualClass);
				this.FP++;
				allTrue = false;
			}
		}
		for (var expectedClass in expectedClasses) {
			if (!(expectedClass in actualClasses)) {
				explanations.push("\t\t--- FALSE NEGATIVE: "+expectedClass);
				this.FN++;
				allTrue = false;
			}
		}
		if (allTrue) {
			if (logTruePositives) explanations.push("\t\t*** ALL TRUE!");
			this.TRUE++;
		}
		this.count++;
		return explanations;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.PrecisionRecall.prototype.addCasesHash"></a>[function <span class="apidocSignatureSpan">limdu.utils.PrecisionRecall.prototype.</span>addCasesHash (expectedClasses, actualClasses, logTruePositives )](#apidoc.element.limdu.utils.PrecisionRecall.prototype.addCasesHash)
- description and source-code
```javascript
addCasesHash = function (expectedClasses, actualClasses, logTruePositives ) {
		var explanations = {};
		explanations['TP'] = []; explanations['FP'] = []; explanations['FN'] = [];

		if (expectedClasses.length == 1)
		{
			var expected = expectedClasses[0]
			if (!(expected in this.confusion))
					this.confusion[expected] = {}
			_.each(actualClasses, function(actualClass, key, list){
				if (!(actualClass in this.confusion[expected]))
					this.confusion[expected][actualClass] = 0
				this.confusion[expected][actualClass] +=1
			}, this)
		}

		actualClasses = hash.normalized(actualClasses);
		expectedClasses = hash.normalized(expectedClasses);

		var allTrue = true;
		for (var actualClass in actualClasses) {

			if (!(actualClass in this.labels)) {
				this.labels[actualClass]={}
				this.labels[actualClass]['TP']=0
				this.labels[actualClass]['FP']=0
				this.labels[actualClass]['FN']=0
				}

			if (actualClass in expectedClasses) {
				if (logTruePositives) explanations['TP'].push(actualClass);
				this.labels[actualClass]['TP'] += 1
				// this.TP++;
			} else {
				explanations['FP'].push(actualClass);
				this.labels[actualClass]['FP'] += 1
				// this.FP++;
				allTrue = false;
			}
		}
		for (var expectedClass in expectedClasses) {

			if (!(expectedClass in this.labels)) {
				this.labels[expectedClass]={}
				this.labels[expectedClass]['TP']=0
				this.labels[expectedClass]['FP']=0
				this.labels[expectedClass]['FN']=0
				}

			if (!(expectedClass in actualClasses)) {
				explanations['FN'].push(expectedClass);
				this.labels[expectedClass]['FN'] += 1
				// this.FN++;
				allTrue = false;
			}
		}
		if (allTrue) {
			// if ((logTruePositives)&& (!only_false_cases)) explanations.push("\t\t*** ALL TRUE!");
			this.TRUE++;
		}
		this.count++;

		_.each(explanations, function(value, key, list){
			// explanations[key] = _.sortBy(explanations[key], function(num){ num });
			explanations[key].sort()
		}, this)

		if (explanations['FP'].length == 0)
			delete explanations['FP']

		if (explanations['FN'].length == 0)
			delete explanations['FN']

		return explanations;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.PrecisionRecall.prototype.calculateStats"></a>[function <span class="apidocSignatureSpan">limdu.utils.PrecisionRecall.prototype.</span>calculateStats ()](#apidoc.element.limdu.utils.PrecisionRecall.prototype.calculateStats)
- description and source-code
```javascript
calculateStats = function ()
	{
		var stats = {}
		var temp_stats = {}
		
		this.retrieveLabels()

		var labelsstats = _.values(this.labels)

		_.each(['Precision', 'Recall', 'F1'], function(param, key, list){
			temp_stats[param] = _.pluck(labelsstats, param)
			// temp_stats[param] = _.filter(temp_stats[param], function(elem){ return (!_.isNaN(elem) && !_.isNull(elem) && elem>-1)  })
			temp_stats[param] = _.reduce(temp_stats[param], function(memo, num){ if (!_.isNaN(num) && !_.isNull(num) && num>-1) {return (
memo + num)} else return memo }) / temp_stats[param].length
		})

		_.each(['TP', 'FP', 'FN'], function(param, key, list){
			stats[param] = _.pluck(labelsstats, param)
			stats[param] = _.reduce(stats[param], function(memo, num){ return memo + num })
		})

		this.endTime = new Date();
		this.timeMillis = this.endTime-this.startTime;
		this.timePerSampleMillis = this.timeMillis / this.count;
		this.TP = stats.TP
		this.FP = stats.FP
		this.FN = stats.FN
		this.Accuracy = (this.TRUE) / (this.count);
		this.macroPrecision = temp_stats['Precision']
		this.macroRecall = temp_stats['Recall']
		this.macroF1 = temp_stats['F1']
		this.microPrecision = stats.TP / (stats.TP+stats.FP);
		this.microRecall = stats.TP / (stats.TP+stats.FN);
		this.microF1 = 2 / (1/this.microRecall + 1/this.microPrecision);
		this.HammingLoss = (stats.FN+stats.FP) / (stats.FN+stats.TP); // "the percentage of the wrong labels to the total number of labels
"
		this.HammingGain = 1-this.HammingLoss;
		
		// this.shortStatsString = sprintf("Accuracy=%d/%d=%1.0f%% HammingGain=1-%d/%d=%1.0f%% Precision=%1.0f%% Recall=%1.0f%% F1=%1.
0f%% timePerSample=%1.0f[ms]",
				// this.TRUE, this.count, this.Accuracy*100, (this.FN+this.FP), (this.FN+this.TP), this.HammingGain*100, this.Precision*100,
this.Recall*100, this.F1*100, this.timePerSampleMillis);
		
		// _.each(this.labels, function(st, lab, list){
		// 	_.each(st, function(val, par, list){
		// 		stats[lab+"_"+par] = val
		// 	}, this)
		// }, this)

		// return stats
	}
```
- example usage
```shell
...
	limdu.utils.test(classifier, testSet, /* verbosity = */0,
		microAverage, macroAverage);
});

macroAverage.calculateMacroAverageStats(numOfFolds);
console.log("\n\nMACRO AVERAGE:"); console.dir(macroAverage.fullStats());

microAverage.calculateStats();
console.log("\n\nMICRO AVERAGE:"); console.dir(microAverage.fullStats());
'''

## Back-classification (aka Generation)

Use this option to get the list of all samples with a given class.
...
```

#### <a name="apidoc.element.limdu.utils.PrecisionRecall.prototype.retrieveLabels"></a>[function <span class="apidocSignatureSpan">limdu.utils.PrecisionRecall.prototype.</span>retrieveLabels ()](#apidoc.element.limdu.utils.PrecisionRecall.prototype.retrieveLabels)
- description and source-code
```javascript
retrieveLabels = function ()
	{
		_.each(Object.keys(this.labels), function(label, key, list){
			
			this.labels[label]['Recall'] = this.labels[label]['TP'] / (this.labels[label]['TP'] + this.labels[label]['FN']);
			this.labels[label]['Precision'] = this.labels[label]['TP'] / (this.labels[label]['TP'] + this.labels[label]['FP']);
			this.labels[label]['F1'] = 2 / (1/this.labels[label]['Recall'] + 1/this.labels[label]['Precision'])

			if (!this.labels[label]['F1']) this.labels[label]['F1'] = -1
		}, this)

		var arlabels = _.pairs(this.labels)
		arlabels = _.sortBy(arlabels, function(num){ return arlabels[0] })
		this.labels = _.object(arlabels)

		return this.labels
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.utils.hash"></a>[module limdu.utils.hash](#apidoc.module.limdu.utils.hash)

#### <a name="apidoc.element.limdu.utils.hash.add"></a>[function <span class="apidocSignatureSpan">limdu.utils.hash.</span>add (target, source)](#apidoc.element.limdu.utils.hash.add)
- description and source-code
```javascript
add = function (target, source) {
	for (var feature in source) {
		if (!(feature in target))
			target[feature]=0;
		if (toString.call(target[feature]) != '[object Number]') continue;
		target[feature] += source[feature];
	}
	return target;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.hash.addtimes"></a>[function <span class="apidocSignatureSpan">limdu.utils.hash.</span>addtimes (target, scalar, source)](#apidoc.element.limdu.utils.hash.addtimes)
- description and source-code
```javascript
addtimes = function (target, scalar, source) {
	for (var feature in source) {
		if (!(feature in target))
			target[feature]=0;
		if (toString.call(target[feature]) != '[object Number]') continue;
		target[feature] += scalar*source[feature];
	}
	return target;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.hash.fromString"></a>[function <span class="apidocSignatureSpan">limdu.utils.hash.</span>fromString (string)](#apidoc.element.limdu.utils.hash.fromString)
- description and source-code
```javascript
fromString = function (string) {
	var lines = string.split(/[\n\r]/g);
	var hash = {};
	for (var i=0; i<lines.length; ++i) {
		var line = lines[i].trim();
		line = line.replace(/\s*#.*?$/, "");  // remove comments
		if (line.length<1) continue; // skip empty lines

		var parts = line.split(/\s*\/\s*/);
		if (parts.length<2 || !parts[0] || !parts[1]) {
			console.dir(parts);
			throw new Error("empty key or value");
		}
		var key = parts[0];
		var value = parts[1];
		if (key in hash) {
			console.warn("key "+key+" already exists. Old value="+hash[key]+", new value="+value);
		}
		hash[key]=value;
	}
	return hash;
}
```
- example usage
```shell
...
'''

On the remote server, do the following:

'''js
// retrieve the string from a file and then:

var intentClassifierCopy = serialize.fromString(intentClassifierString, __dirname);

console.log("Deserialized classifier:");
intentClassifierCopy.classifyAndLog("I want an apple and a banana");  // ['apl','bnn']
intentClassifierCopy.classifyAndLog("I want chips and a doughnut");  // ['cps','dnt']
intentClassifierCopy.trainOnline("I want an elm tree", "elm");
intentClassifierCopy.classifyAndLog("I want doughnut and elm tree");  // ['dnt','elm']
'''
...
```

#### <a name="apidoc.element.limdu.utils.hash.inner_product"></a>[function <span class="apidocSignatureSpan">limdu.utils.hash.</span>inner_product (features, weights)](#apidoc.element.limdu.utils.hash.inner_product)
- description and source-code
```javascript
inner_product = function (features, weights) {
	var result = 0;
	for (var feature in features) {
			if (feature in weights) {
				result += features[feature] * weights[feature];
			} else {
					/* the sample contains a feature that was never seen in training - ignore it for now */
			}
	}
	return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.hash.inner_product_matrix"></a>[function <span class="apidocSignatureSpan">limdu.utils.hash.</span>inner_product_matrix (features, weights)](#apidoc.element.limdu.utils.hash.inner_product_matrix)
- description and source-code
```javascript
inner_product_matrix = function (features, weights) {
	var result = {};
	for (category in weights) {
		result[category] = exports.inner_product(features, weights[category]);
	}
	return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.hash.multiply"></a>[function <span class="apidocSignatureSpan">limdu.utils.hash.</span>multiply (target, source)](#apidoc.element.limdu.utils.hash.multiply)
- description and source-code
```javascript
multiply = function (target, source) {
	for (var feature in source) {
		if (!(feature in target))
			target[feature]=1;
		if (toString.call(target[feature]) != '[object Number]') continue;
		target[feature] *= source[feature];
	}
	return target;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.hash.multiply_scalar"></a>[function <span class="apidocSignatureSpan">limdu.utils.hash.</span>multiply_scalar (target, source)](#apidoc.element.limdu.utils.hash.multiply_scalar)
- description and source-code
```javascript
multiply_scalar = function (target, source) {
	for (var feature in target) {
		if (toString.call(target[feature]) != '[object Number]') continue;
		target[feature] *= source;
	}
	return target;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.hash.normalize_sum_of_squares_to_1"></a>[function <span class="apidocSignatureSpan">limdu.utils.hash.</span>normalize_sum_of_squares_to_1 (features)](#apidoc.element.limdu.utils.hash.normalize_sum_of_squares_to_1)
- description and source-code
```javascript
normalize_sum_of_squares_to_1 = function (features) {
	var sum = exports.sum_of_square_values(features);
	if (sum!=0)
		exports.multiply_scalar(features, 1/Math.sqrt(sum));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.hash.normalize_sum_of_values_to_1"></a>[function <span class="apidocSignatureSpan">limdu.utils.hash.</span>normalize_sum_of_values_to_1 (features)](#apidoc.element.limdu.utils.hash.normalize_sum_of_values_to_1)
- description and source-code
```javascript
normalize_sum_of_values_to_1 = function (features) {
	var sum = exports.sum_of_absolute_values(features);
	if (sum!=0)
		exports.multiply_scalar(features, 1/sum);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.hash.normalized"></a>[function <span class="apidocSignatureSpan">limdu.utils.hash.</span>normalized (object)](#apidoc.element.limdu.utils.hash.normalized)
- description and source-code
```javascript
normalized = function (object) {
	if (Array.isArray(object)) {
		var result = {};
		for (var i=0; i<object.length; ++i)
			result[stringifyIfNeeded(object[i])]=true;
		return result;
	} else if (object instanceof Object) {
		return object;
	} else {
		var result = {};
		result[stringifyIfNeeded(object)]=true;
		return result;
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.hash.stringify_sorted"></a>[function <span class="apidocSignatureSpan">limdu.utils.hash.</span>stringify_sorted (weights, separator)](#apidoc.element.limdu.utils.hash.stringify_sorted)
- description and source-code
```javascript
stringify_sorted = function (weights, separator) {
	var result = "{" + separator;
	var keys = Object.keys(weights);
	keys.sort();
	var last = keys.length-1;
	for (var i=0; i <= last; i++) {
		var key = keys[i];
		var weight = weights[key];
		result += '"'+key+'": '+weight;
		if (i<last) result+=",";
		result += separator;
	}
	result += "}";
	return result;	
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.hash.sum_of_absolute_values"></a>[function <span class="apidocSignatureSpan">limdu.utils.hash.</span>sum_of_absolute_values (weights)](#apidoc.element.limdu.utils.hash.sum_of_absolute_values)
- description and source-code
```javascript
sum_of_absolute_values = function (weights) {
	var result = 0;
	for (var feature in weights)
		result += Math.abs(weights[feature]);
	return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.hash.sum_of_square_values"></a>[function <span class="apidocSignatureSpan">limdu.utils.hash.</span>sum_of_square_values (weights)](#apidoc.element.limdu.utils.hash.sum_of_square_values)
- description and source-code
```javascript
sum_of_square_values = function (weights) {
	var result = 0;
	for (var feature in weights)
		result += Math.pow(weights[feature],2);
	return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.hash.sum_of_values"></a>[function <span class="apidocSignatureSpan">limdu.utils.hash.</span>sum_of_values (weights)](#apidoc.element.limdu.utils.hash.sum_of_values)
- description and source-code
```javascript
sum_of_values = function (weights) {
	var result = 0;
	for (var feature in weights)
		result += weights[feature];
	return result;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.limdu.utils.partitions"></a>[module limdu.utils.partitions](#apidoc.module.limdu.utils.partitions)

#### <a name="apidoc.element.limdu.utils.partitions.partitions"></a>[function <span class="apidocSignatureSpan">limdu.utils.</span>partitions (dataset, numOfPartitions, callback)](#apidoc.element.limdu.utils.partitions.partitions)
- description and source-code
```javascript
partitions = function (dataset, numOfPartitions, callback) {
	var shuffledDataset = _.shuffle(dataset);
	var testSetCount = dataset.length / numOfPartitions;
	
	for (var iPartition=0; iPartition<numOfPartitions; ++iPartition) {
		var testSetStart = iPartition*testSetCount;
		var partition = exports.partition(dataset, testSetStart, testSetCount);
		callback(partition.train, partition.test, iPartition);
	}
}
```
- example usage
```shell
...
	}),
	featureExtractor: limdu.features.NGramsOfWords(1),
});

var microAverage = new limdu.utils.PrecisionRecall();
var macroAverage = new limdu.utils.PrecisionRecall();

limdu.utils.partitions.partitions(dataset, numOfFolds, function(trainSet, testSet) {
	console.log("Training on "+trainSet.length+" samples, testing on "+testSet.length+" samples");
	var classifier = new IntentClassifier();
	classifier.trainBatch(trainSet);
	limdu.utils.test(classifier, testSet, /* verbosity = */0,
		microAverage, macroAverage);
});
...
```

#### <a name="apidoc.element.limdu.utils.partitions.partition"></a>[function <span class="apidocSignatureSpan">limdu.utils.partitions.</span>partition (dataset, testSetStart, testSetCount)](#apidoc.element.limdu.utils.partitions.partition)
- description and source-code
```javascript
partition = function (dataset, testSetStart, testSetCount) {
		var datasetclone = JSON.parse(JSON.stringify(dataset));
		var testSet = datasetclone.splice(testSetStart, testSetCount);
		var trainSet = datasetclone; // without the test-set
		return {train: trainSet, test: testSet};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.partitions.partitions_consistent"></a>[function <span class="apidocSignatureSpan">limdu.utils.partitions.</span>partitions_consistent (dataset, numOfPartitions, callback)](#apidoc.element.limdu.utils.partitions.partitions_consistent)
- description and source-code
```javascript
partitions_consistent = function (dataset, numOfPartitions, callback) {
	var testSetCount = dataset.length / numOfPartitions;
	
	for (var iPartition=0; iPartition<numOfPartitions; ++iPartition) {
		var testSetStart = iPartition*testSetCount;
		var partition = exports.partition(dataset, testSetStart, testSetCount);
		callback(partition.train, partition.test, iPartition);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.partitions.partitions_consistent_by_fold"></a>[function <span class="apidocSignatureSpan">limdu.utils.partitions.</span>partitions_consistent_by_fold (dataset, numOfPartitions, partitionIndex)](#apidoc.element.limdu.utils.partitions.partitions_consistent_by_fold)
- description and source-code
```javascript
partitions_consistent_by_fold = function (dataset, numOfPartitions, partitionIndex) {

	if (!_.isArray(dataset))
		throw new Error("dataset is not an array")

	if (_.isUndefined(numOfPartitions))
		throw new Error("numOfPartitions "+ numOfPartitions)

	if (_.isUndefined(partitionIndex))
		throw new Error("partitionIndex "+ partitionIndex)

	var testSetCount = dataset.length / numOfPartitions;

	var result = {'train': [], 'test': []}
	
	for (var iPartition=0; iPartition<numOfPartitions; ++iPartition) {
		var testSetStart = iPartition*testSetCount;
		var partition = exports.partition(dataset, testSetStart, testSetCount);

		if (iPartition == partitionIndex)
			{
				result['train'] = partition.train
				result['test'] = partition.test
			}
	}
	return result
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.partitions.partitions_hash"></a>[function <span class="apidocSignatureSpan">limdu.utils.partitions.</span>partitions_hash (datasetor, numOfPartitions, callback)](#apidoc.element.limdu.utils.partitions.partitions_hash)
- description and source-code
```javascript
partitions_hash = function (datasetor, numOfPartitions, callback) {

	var count = datasetor[Object.keys(datasetor)[0]].length
	var testSetCount = Math.floor(count / numOfPartitions)

	for (var iPartition=0; iPartition<numOfPartitions; ++iPartition) {
		var testSetStart = iPartition*testSetCount;

		var dataset = JSON.parse(JSON.stringify(datasetor))

		var test = []
		var train = []

		_(count - testSetCount).times(function(n){ train.push([]) })
		
		_.each(dataset, function(value, key, list){
			test = test.concat(value.splice(testSetStart, testSetCount))
			_.each(value, function(elem, key1, list1){
				train[key1].push(elem)
			}, this)
		}, this)
	

		callback(train, test, iPartition);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.partitions.partitions_hash_fold"></a>[function <span class="apidocSignatureSpan">limdu.utils.partitions.</span>partitions_hash_fold (datasetor, numOfPartitions, fold )](#apidoc.element.limdu.utils.partitions.partitions_hash_fold)
- description and source-code
```javascript
partitions_hash_fold = function (datasetor, numOfPartitions, fold ) {

	var count = datasetor[Object.keys(datasetor)[0]].length
	var testSetCount = Math.floor(count / numOfPartitions)

	var testSetStart = fold*testSetCount;
	// var dataset = JSON.parse(JSON.stringify(datasetor))

	var test = []
	var train = []

	_(count - testSetCount).times(function(n){ train.push([]) })
		
	_.each(datasetor, function(value, key, list){
		test = test.concat(value.splice(testSetStart, testSetCount))
		_.each(value, function(elem, key1, list1){
			train[key1].push(elem)
		}, this)
	}, this)
	
	return {"train": train, "test": test}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.limdu.utils.partitions.partitions_reverese"></a>[function <span class="apidocSignatureSpan">limdu.utils.partitions.</span>partitions_reverese (dataset, numOfPartitions, callback)](#apidoc.element.limdu.utils.partitions.partitions_reverese)
- description and source-code
```javascript
partitions_reverese = function (dataset, numOfPartitions, callback) {
	var testSetCount = dataset.length / numOfPartitions;
	
	for (var iPartition=0; iPartition<numOfPartitions; ++iPartition) {
		var testSetStart = iPartition*testSetCount;
		var partition = exports.partition(dataset, testSetStart, testSetCount);
		callback(partition.test, partition.train, iPartition);
	}
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
