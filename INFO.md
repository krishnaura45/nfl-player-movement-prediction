# NFL - Big Data Bowl 2026 - Prediction

## Overview

You are tasked to predict NFL player movement during the video frames after the ball is thrown.

---

## Description

> Note: This Big Data Bowl 2026 has two competitions. This competition is the Prediction competition. Learn more about the [Analytics competition here](https://www.kaggle.com/competitions/nfl-big-data-bowl-2026-analytics).

The downfield pass is the crown jewel of American sports. When the ball is in the air, anything can happen, like a touchdown, an interception, or a contested catch. The uncertainty and the importance of the outcome of these plays is what helps keep audiences on the edge of its seat.

The 2026 Big Data Bowl is designed to help the National Football League better understand player movement during the pass play, starting with when the ball is thrown and ending when the ball is either caught or ruled incomplete. For the offensive team, this means focusing on the targeted receiver, whose job is to move towards the ball landing location in order to complete a catch. For the defensive team, who could have several players moving towards the ball, their jobs are to both prevent the offensive player from making a catch, while also going for the ball themselves. This year's Big Data Bowl asks our fans to help track the movement of these players.

In the Prediction Competition of the Big Data Bowl, participants are tasked with predicting player movement with the ball in the air. Specifically, the NFL is sharing data before the ball is thrown (including the Next Gen Stats tracking data), and stopping the play the moment the quarterback releases the ball. In addition to the pre-pass tracking data, we are providing participants with which offensive player was targeted (e.g, the targeted receiver) and the landing location of the pass.

Using the information above, participants should generate prediction models for player movement during the frames when the ball is in the air. The most accurate algorithms will be those whose output most closely matches the eventual player movement of each player.

### Competition specifics

In the NFL's tracking data, there are 10 frames per second. As a result, if a ball is in the air for 2.5 seconds, there will be 25 frames of location data to predict.
Quick passes (less than half a second), deflected passes, and throwaway passes are dropped from the competition.
Evaluation for the training data is based on historical data. Evaluation for the leaderboard is based on data that hasn't happened yet. Specifically, we will be doing a live leaderboard covering the last five weeks of the 2025 NFL season.

---

## Evaluation

Submissions are evaluated using the Root Mean Squared Error between the predicted and the observed target. The evaluation metric for this contest can be found here.

### Submission File

You must submit to this competition using the provided evaluation API, which ensures that models perform inference on a single play at a time. For each row in the test dataframe you must predict the corresponding x and y values.

---

## Timeline

This is a forecasting competition with an active training phase and a separate forecasting phase where models will be run against player data from future NFL games.

### Training Timeline

September 25, 2025 - Competition Start

November 26, 2025 - Team Merger deadline. This is the last day participants may join or merge teams.

November 26, 2025 - Entry deadline. You must accept the competition rules before this date in order to compete.

December 3, 2025 - Final submission deadline.

All deadlines are at 11:59 PM UTC on the corresponding day unless otherwise noted. The competition organizers reserve the right to update the contest timeline if they deem it necessary.

### Forecasting Timeline

December 4, 2025 - January 5, 2026 - Watch your results play out! The Kaggle Team will refresh the leaderboard throughout the competition at the conclusion of the prior week's NFL games (NFL games are typically played on Thursdays, Sundays, and Mondays). The first week of games scored begins with those played on December 4, December 7, and December 8. The final scheduled NFL game of the 2025-2026 regular season is Sunday, January 4, 2026.

January 6, 2026  - Competition end, results published

All deadlines are at 11:59 PM UTC on the corresponding day unless otherwise noted. The competition organizers reserve the right to update the contest timeline if they deem it necessary.

---

## Code Requirements

Submissions to this competition must be made through Notebooks. In order for the "Submit" button to be active after a commit, the following conditions must be met:

CPU Notebook <= 9 hours run-time
GPU Notebook <= 9 hours run-time
Internet access disabled
Freely & publicly available external data is allowed, including pre-trained models
Please see the Code Competition FAQ for more information on how to submit. And review the code debugging doc if you are encountering submission errors.

---

## Citation

Michael Lopez, Tom Bliss, Ally Blake, Yao Yan, Martyna Plomecka, and Addison Howard. [NFL Big Data Bowl 2026 - Prediction](https://kaggle.com/competitions/nfl-big-data-bowl-2026-prediction), 2025. Kaggle.
