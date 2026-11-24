// ==UserScript==
// @name        Creat Install LinkCard 🔵
// @namespace        http://tampermonkey.net/
// @version        0.1
// @description        GitHubのリポジトリで起動用リンクカードを生成　ショートカット「F6」
// @author        personwritep
// @match        https://github.com/*
// @icon        https://www.google.com/s2/favicons?sz=64&domain=github.com
// @grant        none

// ==/UserScript==


let listen=Symbol();


let target=document.querySelector('head');
let monitor0=new MutationObserver(main);
monitor0.observe(target, { childList: true });

main();

function main(){
    if(!window[listen]){
        window.addEventListener('keydown', check_key);
        window[listen]=true; }


    function check_key(event){
        if(isRepoRoot()){ // リポジトリトップの場合
            if(event.keyCode==117){ // ショートカット「F6」
                event.preventDefault();
                event.stopImmediatePropagation();
                let owner;
                let repo;
                let paths=window.location.pathname.split('/').filter(Boolean);
                owner=paths[0];
                repo=paths[1];
                make_card(owner, repo); }}}


    function isRepoRoot(){ // リポジトリのルート画面
        let pathParts=window.location.pathname.split('/').filter(Boolean);
        return pathParts.length===2 || (pathParts.length>=4 && pathParts[2]==='tree'); }

} // main();



function make_card(owner, repo){
    let card_url; // 生成するインストール用のURL
    card_url='https://github.com/'+ owner +'/'+ repo +'/raw/main/'+ repo +'.user.js';


    let card_html=
        '<div class="ogpCard_root" style="text-align: center;">'+
        '<article class="ogpCard_wrap" contenteditable="false" '+
        'style="display:inline-block; max-width:100%">'+
        '<a class="ogpCard_link" data-ogp-card-log="" href="'+ card_url +'" '+
        'rel="noopener noreferrer" style="display: flex; justify-content: space-between; '+
        'overflow: hidden; width: 500px; max-width: 100%; height: 108px; '+
        'border: 1px solid rgb(0, 128, 186); border-radius: 4px; background-color: #fff; '+
        'color: #000; text-decoration: none; margin: 0 auto;" target="_blank">'+
        '<span class="ogpCard_content" style="display: flex; flex-direction: column; '+
        'overflow: hidden; width: 100%; padding: 8px 25px 4px 15px; justify-content: inherit;">'+
        '<span class="ogpCard_title" style="-webkit-box-orient: vertical; display: -webkit-box; '+
        '-webkit-line-clamp: 2; max-height: 44px; font: bold 16px/1.25 Meiryo; text-align: left; '+
        'overflow: hidden; flex-shrink: 0;">'+ repo +'<br>　　/ at main・'+ owner +
        '</span><span class="ogpCard_description" style="overflow: hidden; '+
        'font: 13px/1.4 Meiryo; text-align: left;">'+
        'Contribute to '+ owner +'/'+ repo +' development by creating an account on GitHub.</span>'+
        '<span class="ogpCard_url" style="display: flex; align-items: center; margin: auto 0 0 20px;">'+
        '<span class="ogpCard_iconWrap" style="font: bold 14px/17px Meiryo;">'+
        '<img alt="" src="https://t1.gstatic.com/faviconV2?client=SOCIAL&amp;type=FAVICON'+
        '&amp;fallback_opts=TYPE,SIZE,URL&amp;url=https://github.com&amp;size=16" '+
        'style="vertical-align: -3px; margin-right: 2px; min-width: 16px;"></span>'+
        '<span class="ogpCard_urlText" style="overflow: hidden; text-overflow: ellipsis; '+
        'white-space: nowrap; font-size: 13px; text-align: left; font-weight: bold;">github.com'+
        '</span></span></span>'+
        '<span class="ogpCard_imageWrap" style="position: relative; width: 100px; height: 100px; '+
        'flex-shrink: 0; margin: auto 0; right: 15px; background: #4abaff; overflow: hidden;">'+
        '<i class="fa-brands fa-github" style="font-size: 54px; margin-top: 15%;"> </i>'+
        '<span style="font: bold 24px/27px Meiryo; background: transparent">GitHub</span>'+
        '</span></a></article></div>';


    if(navigator.clipboard){ // copyToClipboardを実行
        navigator.clipboard.writeText(card_html);

        alert(
            "🟦　インストール用リンクカードを生成して\n"+
            "　　 クリップボードにコピーしました"); }

} // make_card()
