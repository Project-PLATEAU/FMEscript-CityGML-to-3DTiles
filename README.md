



      
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
<h2><a id="user-content-参考資料" class="anchor" aria-hidden="true" href="#参考資料"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>参考資料</h2>
<ul>
<li>品質評価システム: <a href="https://github.com/Project-PLATEAU/CityGML-evaluation-system">https://github.com/Project-PLATEAU/CityGML-evaluation-system</a></li>
<li>モデル自動生成システム: <a href="https://github.com/Project-PLATEAU/CityGML-production-system">https://github.com/Project-PLATEAU/CityGML-production-system</a></li>
<li>書式・概念一貫性検証機能: <a href="https://github.com/Project-PLATEAU/CityGML-validation-function">https://github.com/Project-PLATEAU/CityGML-validation-function</a></li>
</ul>
</article>
  </div>

    </div>

  

  <details class="details-reset details-overlay details-overlay-dark" id="jumpto-line-details-dialog">
    <summary data-hotkey="l" aria-label="Jump to line"></summary>
    <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast linejump" aria-label="Jump to line">
      <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="js-jump-to-line-form Box-body d-flex" action="" accept-charset="UTF-8" method="get">
        <input class="form-control flex-auto mr-3 linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
        <button type="submit" class="btn" data-close-dialog>Go</button>
</form>    </details-dialog>
  </details>


</div>



  </div>
</div>

    </main>
  </div>


  </div>

          
<div class="footer container-xl width-full p-responsive" role="contentinfo">
  <div class="position-relative d-flex flex-row-reverse flex-lg-row flex-wrap flex-lg-nowrap flex-justify-center flex-lg-justify-between pt-6 pb-2 mt-6 f6 color-text-secondary border-top color-border-secondary ">
    <ul class="list-style-none d-flex flex-wrap col-12 col-lg-5 flex-justify-center flex-lg-justify-between mb-2 mb-lg-0">
      <li class="mr-3 mr-lg-0">&copy; 2021 GitHub, Inc.</li>
        <li class="mr-3 mr-lg-0"><a href="https://docs.github.com/en/github/site-policy/github-terms-of-service" data-ga-click="Footer, go to terms, text:terms">Terms</a></li>
        <li class="mr-3 mr-lg-0"><a href="https://docs.github.com/en/github/site-policy/github-privacy-statement" data-ga-click="Footer, go to privacy, text:privacy">Privacy</a></li>
        <li class="mr-3 mr-lg-0"><a data-ga-click="Footer, go to security, text:security" href="https://github.com/security">Security</a></li>
        <li class="mr-3 mr-lg-0"><a href="https://www.githubstatus.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
        <li><a data-ga-click="Footer, go to help, text:Docs" href="https://docs.github.com">Docs</a></li>
    </ul>

    <a aria-label="Homepage" title="GitHub" class="footer-octicon d-none d-lg-block mx-lg-4" href="https://github.com">
      <svg height="24" class="octicon octicon-mark-github" viewBox="0 0 16 16" version="1.1" width="24" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
</a>
    <ul class="list-style-none d-flex flex-wrap col-12 col-lg-5 flex-justify-center flex-lg-justify-between mb-2 mb-lg-0">
        <li class="mr-3 mr-lg-0"><a href="https://support.github.com" data-ga-click="Footer, go to contact, text:contact">Contact GitHub</a></li>
        <li class="mr-3 mr-lg-0"><a href="https://github.com/pricing" data-ga-click="Footer, go to Pricing, text:Pricing">Pricing</a></li>
      <li class="mr-3 mr-lg-0"><a href="https://docs.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li class="mr-3 mr-lg-0"><a href="https://services.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
        <li class="mr-3 mr-lg-0"><a href="https://github.blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a data-ga-click="Footer, go to about, text:about" href="https://github.com/about">About</a></li>
    </ul>
  </div>
  <div class="d-flex flex-justify-center pb-6">
    <span class="f6 color-text-tertiary"></span>
  </div>

  
</div>



  <div id="ajax-error-message" class="ajax-error-message flash flash-error" hidden>
    <svg class="octicon octicon-alert" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.22 1.754a.25.25 0 00-.44 0L1.698 13.132a.25.25 0 00.22.368h12.164a.25.25 0 00.22-.368L8.22 1.754zm-1.763-.707c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0114.082 15H1.918a1.75 1.75 0 01-1.543-2.575L6.457 1.047zM9 11a1 1 0 11-2 0 1 1 0 012 0zm-.25-5.25a.75.75 0 00-1.5 0v2.5a.75.75 0 001.5 0v-2.5z"></path></svg>
    <button type="button" class="flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
      <svg class="octicon octicon-x" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z"></path></svg>
    </button>
    You can’t perform that action at this time.
  </div>

  <div class="js-stale-session-flash flash flash-warn flash-banner" hidden
    >
    <svg class="octicon octicon-alert" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.22 1.754a.25.25 0 00-.44 0L1.698 13.132a.25.25 0 00.22.368h12.164a.25.25 0 00.22-.368L8.22 1.754zm-1.763-.707c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0114.082 15H1.918a1.75 1.75 0 01-1.543-2.575L6.457 1.047zM9 11a1 1 0 11-2 0 1 1 0 012 0zm-.25-5.25a.75.75 0 00-1.5 0v2.5a.75.75 0 001.5 0v-2.5z"></path></svg>
    <span class="js-stale-session-flash-signed-in" hidden>You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
    <span class="js-stale-session-flash-signed-out" hidden>You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
  </div>
    <template id="site-details-dialog">
  <details class="details-reset details-overlay details-overlay-dark lh-default color-text-primary hx_rsm" open>
    <summary role="button" aria-label="Close dialog"></summary>
    <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast hx_rsm-dialog hx_rsm-modal">
      <button class="Box-btn-octicon m-0 btn-octicon position-absolute right-0 top-0" type="button" aria-label="Close dialog" data-close-dialog>
        <svg class="octicon octicon-x" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z"></path></svg>
      </button>
      <div class="octocat-spinner my-6 js-details-dialog-spinner"></div>
    </details-dialog>
  </details>
</template>

    <div class="Popover js-hovercard-content position-absolute" style="display: none; outline: none;" tabindex="0">
  <div class="Popover-message Popover-message--bottom-left Popover-message--large Box color-shadow-large" style="width:360px;">
  </div>
</div>




  </body>
</html>

