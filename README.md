# Openshift(minishift)でtiida(JBoss Data Virtualization)を試してみるプロジェクト

## Tiida(JBoss Data Virtualization)とは

## [OpenShift](https://www.openshift.com) とは

[Red Hat社](https://www.redhat.com/ja)が提供するコンテナ環境で、[Docker](https://www.docker.com)および[Kubernetes](https://kubernetes.io/)をベースに、専用のコマンドとwebコンソール画面が追加されています。

商用版のOpenShift Container Platform(旧Enterprise)と、オープンソース版のOKD（旧OpenShift origin)があり、さらに開発環境用としてOKDをローカルのVM上で動かす[Minishift](https://github.com/minishift/minishift)が提供されています。

## 環境の構築

無償使用可能なのはDockerおよび各種依存コマンドをインストールした上でOKDをインストールするか、またはMinishiftをインストールするかのどちらかとなりますが、既存のdocker環境を利用するOKDではdocker環境の状況や既存のコマンド群との干渉が煩雑になってしまいます。  
今回は、仮想マシン上に独立した環境を立ち上げてくれるMinishiftを使用する事にします。

setupフォルダの中に各OS別のセットアップスクリプトを用意しました。
MacOS Xの場合はmac.shを、...(他順次用意)実行してください。

ルート権限は不用ですが、各OSでの管理者権限での実行が必要となります。
