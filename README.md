# kubenetes-samples

kubenetes の samples プロジェクト

## 環境

- Windows10 Pro(22H2)
- Rancher Desktop： v1.9.1
- minikube version： v1.31.2

## 環境構築メモ
- 注意：「PowerShell」や「Rancher Desktop」は管理者権限で起動すること

- minukebeコマンド
```bash
・minikube起動
$ minikube start --driver=docker
・ダッシュボード表示
$ minikube dashboard
・ステータス確認
$ minikube status
・バージョン確認
$ minikube version version
・クラスラー停止
$ minikube stop
・クラスラー完全削除
$ minikube delete -all
```
- kubectlコマンド
```bash
・podの作成
$ kubectl apply -f [yamlファイル名]
・pod一覧の確認
$ kubectl get pod
・podの削除
$ kubectl delete pod [pod名]
・podのIP確認
$ kubectl get pod -o wide
```

## 参考

- [minikube Documentation](https://minikube.sigs.k8s.io/docs/)
- [サイボウズ新人研修の「Kubernetes を使った開発入門」を触ってみた備忘録](https://zenn.dev/ikuraikura/articles/86941a924fd86af4800d)
