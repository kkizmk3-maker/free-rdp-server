name: Deploy Free RDP Server

on:
  workflow_dispatch: # يمكنك تشغيله يدوياً
  schedule:
    - cron: '0 0 * * *' # إعادة التشغيل يومياً

jobs:
  deploy-rdp:
    runs-on: ubuntu-latest
    timeout-minutes: 30

    steps:
    - name: Start Ubuntu RDP
