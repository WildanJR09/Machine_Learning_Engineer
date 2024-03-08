# Quiz 4

---

## True or False: A ParDo acts on all items at once (like a Map in MapReduce).

`False`

---

## Your development team is about to execute this code block. What is your team about to do?

```cmd
mvn compile -e exec:java \
    -Dexec.mainClass=$MAIN \
    -Dexec.args="--project=$PROJECT" \
    --stagingLocation=gs://$BUCKET/staging/ \
    --tempLocation=gs://$BUCKET/staging/ \
    --runner=DataflowRunner \
```

`We are compiling our Cloud Dataflow pipeline written in Java and are submitting it to the cloud for execution.Notice that we are calling mvn compile and passing in --runner=DataflowRunner.`

---

## What is one key advantage of preprocessing your features using Apache Beam?

`The same code you use to preprocess features in training and evaluation can also be used in serving.`

---

## Which of these accurately describes the relationship between Apache Beam and Dataflow?

`Apache Beam is the API for data pipeline building in Java or Python and Dataflow is the implementation and execution framework.`

---

## To run a pipeline you need something called a **\_\_\_\_**.

`runner`

---

## What is the purpose of a Cloud Dataflow connector?

.apply(TextIO.write().to(“gs://…”));

`Connectors allow you to output the results of a pipeline to a specific data sink like Bigtable, Google Cloud Storage, flat file, BigQuery, and more.`

---

## True or False: The Filter method can be carried out in parallel and autoscaled by the execution framework:

![](https://cdn.qwiklabs.com/tdbwGpro8kEkyktN5xcKaRAuBLvobRVzfXMbD2Eurrc%3D)

`True: Anything in Map or FlatMap can be parallelized by the Beam execution framework.`

---
