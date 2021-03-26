



      
  <div id="readme" class="Box-body readme blob js-code-block-container p-5 p-xl-6 gist-border-0">
    <article class="markdown-body entry-content container-lg" itemprop="text"><h1><a id="user-content-位相一貫性検証機能" class="anchor" aria-hidden="true" href="#位相一貫性検証機能"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>位相一貫性検証機能</h1>
<h2><a id="user-content-概要" class="anchor" aria-hidden="true" href="#概要"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>概要</h2>
<p>3D都市モデルの品質管理支援のための位相一貫性検証機能です。</p>
<p>本ソフトウェアは、国土交通省の<a href="https://www.mlit.go.jp/plateau/" rel="nofollow">Project PLATEAU</a>で開発した<a href="https://github.com/Project-PLATEAU/CityGML-evaluation-system">品質評価システム</a>で利用した、3D都市モデルの位相一貫性検証機能（FME Workspace）です。対応データ形式は<a href="https://www.ogc.org/standards/citygml" rel="nofollow">OGC CityGML 2.0</a>形式です。また、CityGMLの拡張仕様であるADE（Application Domain Extension）にも対応しており、内閣府地方創生推進事務局が定めた<a href="https://www.kantei.go.jp/jp/singi/tiiki/toshisaisei/itoshisaisei/iur/" rel="nofollow">i-都市再生技術仕様案 v1.4 (iｰUR 1.4)</a>などにも対応可能です。</p>
<p>本ソフトウェアの動作には前提ソフトウェア（商用ソフトウェア）が必要で、単独では利用できません。位相一貫性検証機能の実装例として参考にして下さい。</p>
<p>なお、本ソフトウェアはドイツ<a href="https://vc.systems/en/" rel="nofollow">virtualcitysystems社</a>が開発した製品機能を、オープンソースとして公開するためご提供を頂いたものです。virtualcitysystems社に感謝します。</p>
<p>機能一覧</p>
<ul>
<li>runner.fmw：複数CityGMLをZIP圧縮したファイルを検証します。パラメータMAX_PROCの指定に応じてマルチプロセスで実行できます。</li>
<li>CityGMLValidation.fmw：CityGMLファイルを検証します。パラメータで検証内容を指定し、また検証結果（JSON形式のログファイル）の出力先を設定できます。</li>
</ul>
<h2><a id="user-content-動作環境前提ソフトウェア" class="anchor" aria-hidden="true" href="#動作環境前提ソフトウェア"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>動作環境、前提ソフトウェア</h2>
<p>動作環境</p>
<ul>
<li>Windows (Windows Server 2016 Datacenterで動作確認)</li>
</ul>
<p>前提ソフトウェア</p>
<ul>
<li>商用ソフトウェア：<a href="https://www.safe.com/fme/fme-desktop/" rel="nofollow">FME Desktop</a></li>
</ul>
<h2><a id="user-content-利用方法" class="anchor" aria-hidden="true" href="#利用方法"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>利用方法</h2>
<ol>
<li>
<p>上記の前提ソフトウェアをインストールします。</p>
</li>
<li>
<p>本レポジトリの一式をダウンロードし、任意のディレクトリに置きます。</p>
</li>
<li>
<p>FME WorkbenchでCityGMLValidation.fmwを開いて実行するか、またはコマンドラインからパラメータを指定してFME.exeを実行して下さい。</p>
<p>fme.exe CityGMLValidation.fmw --INPUT "CityGML.gml" --ADE_XSD_DOC "" --SRS_AXIS "2&lt;comma&gt;1&lt;comma&gt;3" --COORD "EPSG:6677" --OVER_CHECK "LoD2" --OVERLAP "5" --TOLERANCE "0.001" --BOUNDEDBY "Yes" --PREC "3" --PLAN_ANG "20" --PLAN_DIST "0.03" --OUTPUT "report.json"</p>
<p>fme.exe runner.fmw --INPUT "CityGML.zip" --ADE_XSD_DOC "" --SRS_AXIS "2&lt;comma&gt;1&lt;comma&gt;3" --COORD "EPSG:6677" --OVER_CHECK "LoD2" --OVERLAP "5" --TOLERANCE "0.001" --BOUNDEDBY "Yes" --PREC "3" --PLAN_ANG "20" --PLAN_DIST "0.03" --OUTPUT "OutputFolder" --MAX_PROC "7" --WORKSPACE_FILE "CityGMLValidation.fmw" --LOG "logs"</p>
</li>
<li>
<p>パラメータの詳細は<a href="/Project-PLATEAU/CityGML-geometry-validator/blob/main/doc/documentation.pdf">ドキュメント</a>を参照して下さい。注意点は下記です</p>
<ol>
<li>COORD：緯経度から平面直角座標系に変換して検証するため、対象都市毎に適切な系のEPSGコードを指定。</li>
<li>OVER_CHECK：重複判定を実施する対象。通常は"LoD2"だが計算リソースを要するため、必須でなければ"No"としても良い。</li>
<li>TOLERANCE：0.001は「1mm以内の近接点をエラーと検出する」の意味。より詳細なモデルでは0.0001など適切に変更しても良い。</li>
<li>PREC：計算誤差を考慮し、近接点を同一点にSnap処理する単位。3は「1mm」の意味だが、モデルの有効桁数に応じて8など詳細化しても良い。</li>
</ol>
</li>
<li>
<p>ログファイルにエラーが出力された場合、<a href="/Project-PLATEAU/CityGML-geometry-validator/blob/main/doc/log.pdf">ログコード一覧</a>を参照し、エラーの原因を分析して下さい。</p>
</li>
</ol>
<h2><a id="user-content-ライセンス" class="anchor" aria-hidden="true" href="#ライセンス"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>ライセンス</h2>
<p>Copyright (C) 2021 virtualcitysystems, GmbH.</p>
<p>本ソフトウェアは<a href="/Project-PLATEAU/CityGML-geometry-validator/blob/main/LICENSE">Apache-2.0 License</a>を適用します。</p>
<h2><a id="user-content-注意事項" class="anchor" aria-hidden="true" href="#注意事項"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>注意事項</h2>
<ul>
<li>本レポジトリは参考資料として提供しているものです。動作保証は行っておりません。</li>
<li>予告なく変更・削除する可能性があります。</li>
<li>本レポジトリの利用により生じた損失及び損害等について、国土交通省及び著作権者はいかなる責任も負わないものとします。</li>
</ul>
   
