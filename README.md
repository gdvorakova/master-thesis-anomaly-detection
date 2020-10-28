# Anomaly Detection and Automated Diagnostics Using Machine Learning Techniques

## Background/motivation (incl. key concepts & terminology)
For decades radio communication has been confined to the boundaries of network
coverage. In certain mission-critical communications for public safety
organisations, it is crucial to stay connected even beyond the boundaries of the
radio system. Motorola Solutions’ SmartConnect is a system optimised for
reliability and excellent coverage to ensure connection between teams no matter
where they are.
Land Mobile Radio (LMR) is the leading communication system for public safety,
voice-centric, “Push-To-Talk” (PTT) mobile radio communications. P25 (Project 25),
is a set of standards suited to public safety radio systems and first responders to
address interoperability issues related to LMR radio communications. Long-Term
Evolution (LTE) is a widely deployed broadband technology offering high-data-rate
applications currently not supported in LMR. Both LMR and LTE provide value for
public safety users, however, the greatest benefit is when both technologies are
leveraged simultaneously. When LMR is unavailable, SmartConnect is
automatically switching the P25 channel to the broadband LTE system without
intervention.
The production system consists of infrastructure and directly connected radios.
There are two kinds of data available. Both infrastructure and radios are being
monitored and produce logs and metrics. In addition, there is a recorded history of
customer documented issues of the production system, that can be correlated
against the logs and metrics.

## A problem statement
The goal of the thesis is to apply and evaluate various machine learning techniques
to automate analysis of the ever-growing amount of logs and metrics produced by
a production system consisting of two main actors - infrastructure and Push-ToTalk devices connected to the infrastructure.
The target is to try to correlate the reported issues against the logs and metrics
(e.g. caused by end-user loaded wrong certificate, system-admin applied a wrong
configuration, dependency broke down) in order to automatically detect and
possibly self-heal or help the end-user to overcome some of the production
system problems.

Prior to applying machine learning to the problem, it is needed to preprocess the
raw logged data from both the PTT devices and the infrastructure. The first
problem our research tries to address is whether it is possible to use machine
learning techniques at all to detect anomalies on the provided data.
Another part of the research is to try to analyse the current state of the logging to
determine whether there are properties of the system that should be recorded
further in order to improve the performance of our machine learning models or,
conversely, there are data properties that could be omitted from the trace as they
do not provide any valuable information and unnecessarily take up storage space.
Exploratory analysis will be performed on the datasets in order to identify
anomalous patterns and identify hypotheses to be further tested.
If there are informative patterns yielded by the exploratory analysis, we will
propose different machine learning approaches to detect them and we will
evaluate their performance in a series of experiments.
Possible extensions
After achieving the thesis statement, there are possibilities of extending the
project. One such extensions is applying machine learning techniques in order to
characterise audio streams and classify different kinds of poor audio connection.
Another possible research question is to determine how much data is required to
log to predict an anomaly to effect the data size.

## A list of 4-6 project-specific learning objectives

- Understand and analyse the structure of a real-world dataset.
- Apply data preprocessing techniques on raw log data from live production
systems to prepare inputs for machine learning models.
- Build further on the grounding of principles acquired in the Machine Learning
course, and to determine if those principles can be applied to achieve anomaly
detection.
- Investigate the data quality requirements that would allow for anomaly
detection.
- Ability to discuss the methodologies and theory of anomaly detection
techniques in general as well as at an academic level.
