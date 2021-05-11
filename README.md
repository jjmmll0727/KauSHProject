# KauSHProject

listening user's talk and analyzing it and recommend music list related user's emotion

my task>>

android studio를 기반으로 google cloud platform에서 SPEECH TO TEXT api를 사용해 사용자의 음성데이터를 텍스트 데이터로 전환하는 작업을 하였다. 
초기에 aws transcribe service를 시도했지만, 한국어를 인식하는데 있어서 google speech to text api가 더 좋은 효과를 발휘하여 바꾸게 되었다. 

또한 음성텍스트를 aws sagemaker를 사용하는 자연어처리 팀에게 넘겨주기 위해 aws s3에 저장하고 event-driven 방식을 구현하기 위해 lamba service와 s3연동하였다.

인간의 감정을 크게 기쁨 슬픔 무념무상(?) 으로 나누어 자연어처리 팀에서 사용자의 말을 분석하여 넘겨주면 그에 해당하는 음악을 재생해주는 기능을 구현하였다. 

음악 리스트는 firebase에 수작업으로 추가하였다. 

-------------------------------------------------------

처음으로 기획부터 디자인 개발 까지 진행한 프로젝트였다. 
android studio는 다른 팀원이 전담하여 진행하였지만, AWS를 처음으로 사용하는 좋은 경험이었다고 생각한다. 추후에 serverless service를 구축할때 AWS service들을 자주 사용하면 좋을 것 같다. 


[음성데이터 감정 분석.pdf](https://github.com/jjmmll0727/KauSHProject/files/6455834/default.pdf)


