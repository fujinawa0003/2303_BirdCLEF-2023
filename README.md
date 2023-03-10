# 2303_BirdCLEF-2023
BirdCLEF 2023_competition
<img width="1193" alt="image" src="https://user-images.githubusercontent.com/88224359/224439623-79448d49-49ed-457b-b360-3120efaaa487.png">


# Dataset Description
Your challenge in this competition is to identify which birds are calling in long recordings made in Kenya. This is an important task for scientists who monitor bird populations for conservation purposes. More accurate solutions could enable more comprehensive monitoring. This year, your notebook must also complete inference in a more constrained time frame. This will make it easier to deploy winning models for on the ground conservation efforts where efficiency is at a premium.   

This competition uses a hidden test. When your submitted notebook is scored, the actual test data (including a sample submission) will be made available to your notebook.   

Files.  
train_audio/ The training data consists of short recordings of individual bird calls generously uploaded by users of xenocanto.org. These files have been downsampled to 32 kHz where applicable to match the test set audio and converted to the ogg format. The training data should have nearly all relevant files; we expect there is no benefit to looking for more on xenocanto.org.

test_soundscapes/ When you submit a notebook, the test_soundscapes directory will be populated with approximately 200 recordings to be used for scoring. They are 10 minutes long and in ogg audio format. The file names are randomized. It should take your submission notebook approximately five minutes to load all of the test soundscapes.

train_metadata.csv A wide range of metadata is provided for the training data. The most directly relevant fields are:

- primary_label - a code for the bird species. You can review detailed information about the bird codes by appending the code to https://ebird.org/species/, such as https://ebird.org/species/amecro for the American Crow.
- latitude & longitude: coordinates for where the recording was taken. Some bird species may have local call 'dialects,' so you may want to seek geographic diversity in your training data.
- author - The user who provided the recording.
- filename: the name of the associated audio file.
- sample_submission.csv A valid sample submission.

row_id: A slug of [soundscape_id]_[end_time] for the prediction.
- [bird_id]: There are 264 bird ID columns. You will need to predict the probability of the presence of each bird for each row.
- eBird_Taxonomy_v2021.csv - Data on the relationships between different species.

# データセットの説明
このコンペティションの課題は、ケニアで録音された長時間の録音から、どの鳥が鳴いているのかを特定することです。これは、保全のために鳥の個体数を監視する科学者にとって、重要な課題です。より正確な解答が得られれば、より包括的なモニタリングが可能になります。今年は、より制約の多い時間枠の中で推論を完了させることも求められます。これにより、効率性が重視される現場での保全活動において、受賞モデルの展開がより容易になります。  

このコンペティションでは、隠しテストが採用されています。提出されたノートブックが採点される際、実際のテストデータ（サンプル提出を含む）があなたのノートブックに公開されます。  

ファイルです。 
train_audio/ トレーニングデータは、xenocanto.orgのユーザーによって惜しみなくアップロードされた個々の鳥の鳴き声の短い録音で構成されています。これらのファイルは、テストセットの音声と一致するように、必要に応じて32kHzにダウンサンプリングされ、oggフォーマットに変換されています。学習データには、ほぼすべての関連ファイルが含まれているはずです。xenocanto.orgでこれ以上のファイルを探すメリットはないものと思われます。

test_soundscapes/ ノートブックを提出すると、test_soundscapesディレクトリに、採点に使用する約200の録音が格納されます。これらは10分で、oggオーディオフォーマットです。ファイル名はランダムです。テスト用サウンドスケープをすべて読み込むには、投稿ノートブックに5分程度かかります。

train_metadata.csv トレーニングデータには、さまざまなメタデータが用意されています。最も直接的に関連するフィールドは以下の通りです。

- primary_label - 鳥の種類を表すコード。アメリカカラスの場合は https://ebird.org/species/amecro のように、https://ebird.org/species/ にコードを付加することで、鳥のコードに関する詳細情報を確認できます。
- 緯度・経度：録音が行われた場所の座標。鳥の種類によっては、地元で鳴く「方言」がある場合があるので、トレーニングデータには地理的な多様性を求めるとよいでしょう。
- author - 録音を提供したユーザー。
- filename：関連するオーディオファイルの名前です。
- sample_submission.csv 有効なサンプル投稿です。

row_id: soundscape_id]_[end_time] のスラッグで、予測のためのものです。
- bird_id]です。鳥のIDカラムは264個あります。各行に対して各鳥の存在確率を予測する必要があります。
- eBird_Taxonomy_v2021.csv - 異なる種間の関係に関するデータです。

# Reference
| No | Status | Name | Detail | Url |
| --- | --- | --- | --- | --- |
| 01 | doing | Inferring Birds with Kaggle Models | kaggleからの前回のモデル | [url]([https://www.kaggle.com/code/dschettler8845/novo-esp-eli5-performant-approaches-lb-0-451)](https://www.kaggle.com/code/philculliton/inferring-birds-with-kaggle-models)|


# やってみたいことリスト
| No | Status | Name | Detail |
| --- | --- | --- | --- |
| 01| done | EDA | EDA|.  


# Log
## 230311
ついにエントリー。

