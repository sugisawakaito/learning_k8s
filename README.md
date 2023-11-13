https://www.udemy.com/course/web-application-with-docker-kubernetes/
を見ながら学習中

command:
  **apply**: "マニファクトファイルの記述をkubenerticeに反映するコマンド。ちなみに'-f'か'-k'がないとmust errorになる"
    **-f**: "どのファイルをしているか表す。 -f. --filename=[]"
  **get**: "反映されたPodsのstatusを確認するコマンド"
    **"-w"**: "Podsのstatusが変更するまでログが出続ける。-w, --watch"
    **"-o"**:
      **"wide"**: "IP情報まで見れる"
  **delete**: "反映されているPodsを削除するコマンド"
  **cp <src> <pod-name>:<dest>**: "指定されたファイルを指定された転送先に送る"
  **describe pod**: "反映されているkubeneticeの情報をgetより詳細にできる"
