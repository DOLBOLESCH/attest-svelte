<div style="display: grid;">
    <article class="main_article">
        <h2 id="article_title">CSS</h2>
        <hr id="hr1">
        <!-- svelte-ignore a11y-img-redundant-alt -->
        <img src="#" alt="main-image" id="main_img">
        <hr id="hr2">
        <p id="article_text">
          <strong>CSS -&nbsp; Cascading Style Sheets «каскадные таблицы стилей».</strong>  формальный язык описания внешнего вида документа (веб-страницы), написанного с использованием языка разметки (чаще всего HTML или XHTML). Также может применяться к любым XML-документам, например, к SVG или XUL.
        </p>
        <p id="article_text">
            <strong>CSS используется создателями веб-страниц для задания цветов, шрифтов, стилей, расположения отдельных блоков и других аспектов представления внешнего вида этих веб-страниц.</strong> Основной целью разработки CSS является ограждение и отделение описания логической структуры веб-страницы (которое производится с помощью HTML или других языков разметки) от описания внешнего вида этой веб-страницы (которое теперь производится с помощью формального языка CSS). Такое разделение может увеличить доступность документа, предоставить большую гибкость и возможность управления его представлением, а также уменьшить сложность и повторяемость в структурном содержимом.
        </p>
        <p id="article_text">
            <strong>Кроме того, CSS позволяет представлять один и тот же документ в различных стилях или методах вывода,</strong> таких как экранное представление, печатное представление, чтение голосом (специальным голосовым браузером или программой чтения с экрана) или при выводе устройствами, использующими шрифт Брайля.
        </p>
        <p id="article_text">
            <strong>Правила CSS могут располагаться как в самом веб-документе, внешний вид которого они описывают, так и во внешних файлах, имеющих расширение .css.</strong> Формат CSS — это текстовый файл, в котором содержится перечень правил CSS и комментариев к ним.
            Стили CSS могут быть подключены или внедрены в описываемый ими веб-документ четырьмя способами.
        </p>
    </article>
    <hr id="final_hr">
</div>

<style>
div {
    margin: 0;
    padding: 0;
}
hr {
    height: 2px;
    background-color: black;
    border: none;
}
#final_hr {
    margin-top: 60px;
    margin-bottom: 120px;
    width: 100%;
}

#article_title,
#article_text  {
    font-family: sans-serif;
}

.main_article {
    position: relative;
    min-width: 1010px;
    width: 79vw;
    background-color: #E0E0E0;
    border-radius: 15px;
}
#article_title {
    position: absolute;
    top: 0;
    margin: 0 0 26px 4%;
    font-weight: 600;
    font-size: 40px;
}
#article_text {
    position: relative;
    max-width: 63%;
    margin-left: 4%;
    bottom: 120px;
    font-weight: 500;
    font-size: 22px;
}
.main_article {
    margin-top: 100px;
    justify-self: center;
    background-color: white;
}
#article_title {
    position: static;
    margin: 0 0 60px 0;
}
#article_text {
    position: static;
    margin: 0 0 40px 0;
    max-width: unset;
}
#hr1 {
    margin: 0px 0 38px;
}
#hr2 {
    margin: 60px 0 25px;
}
</style>