---
title: 'Использование тегов div API OneNote для извлечения данных из записанного содержимого '
description: " Корпоративные записные книжки в Microsoft 365"
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 41678fff4a84a20a49c4be94962a4381cf270e6a785a32568963dfed7a745184
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54216332"
---
# <a name="use-onenote-api-div-tags-to-extract-data-from-captures"></a>Использование тегов div API OneNote для извлечения данных из записанного содержимого 

**Область применения:** Пользовательские записные книжки в OneDrive | Корпоративные записные книжки в Microsoft 365.

Используйте API OneNote, чтобы извлекать данные визитных карточек с изображения или данные из рецептов и описаний товаров по URL-адресу.

<a name="attributes"></a>

## <a name="extraction-attributes"></a>Атрибуты извлечения

Чтобы извлекать и преобразовывать данные, просто включите элемент div, указывающий исходный контент, метод извлечения и резервное действие в запрос [create-page](onenote-create-page.md) или [update-page](onenote-update-page.md). API отображает извлеченные данные на странице в простом для чтения формате. 

```html
<div
  data-render-src="image-or-url"
  data-render-method="extraction-method"
  data-render-fallback="fallback-action">
</div>
```

### <a name="data-render-src"></a>data-render-src

Источник контента. Это может быть изображение визитной карточки либо абсолютный URL-адрес страницы с рецептом или описанием товара. Обязательный.

Для наилучших результатов используйте канонический URL-адрес, указанный в HTML-коде исходной веб-страницы (если он указан). Например, канонический URL-адрес может быть задан в исходной веб-странице следующим образом:

`<link rel="canonical" href="www.domainname.com/page/123/size12/type987" />` 


### <a name="data-render-method"></a>data-render-method

Метод извлечения, который необходимо запустить. Обязательный.

| Значение | Описание |
|:------|:------|
| extract.businesscard | Извлечение данных визитной карточки. |
| extract.recipe | Извлечение рецепта. |
| extract.product | Извлечение описания товара. |
| extract | Неизвестный тип извлечения. |

Для наилучших результатов укажите тип контента (`extract.businesscard`, `extract.recipe` или `extract.product`), если вы его знаете. Если тип контента неизвестен, используйте метод `extract`, и API OneNote попытается автоматически его определить.

### <a name="data-render-fallback"></a>data-render-fallback

Резервное действие при неудачном извлечении. Если атрибут не указан, по умолчанию используется значение **render**. 

| Значение | Описание |
|:------|:------|
| render | Отображает исходное изображение или снимок веб-страницы с рецептом или товаром. |
| Нет | Не выполняет никаких действий.<br /><br />Этот параметр удобно использовать, если вы хотите всегда размещать снимок визитной карточки или веб-страницы на странице (в дополнение к извлеченному контенту). Обязательно отправляйте отдельный элемент `img` в запросе, как показано в примерах. |

<a name="biz-card"></a>

## <a name="business-card-extractions"></a>Извлечение данных визитной карточки

API OneNote пытается найти и отобразить следующую контактную информацию на основе изображения визитной карточки человека или компании.

- Имя
- Название
- Организация
- Номер телефона/факса
- Почтовый и фактический адрес
- Адреса электронной почты
- Веб-сайты



<img alt="An example business card extraction" src="images/biz-card-extraction.png" width="200">

Извлеченная контактная информация в формате vCard (файл с расширением VCF) также внедряется в страницу. vCard — это удобный способ получить контактную информацию при извлечении HTML-контента страницы.

### <a name="common-scenarios-for-business-card-extractions"></a>Стандартные сценарии извлечения элементов визитных карточек

#### <a name="extract-business-card-information-and-also-render-the-business-card-image"></a>Извлечение данных визитной карточки и отрисовка ее изображения

Укажите метод `extract.businesscard` и резервное действие `none`. Кроме того, отправьте элемент `img` с атрибутом `src`, который также ссылается на изображение. Если API не может извлечь какой-либо контент, он отрисовывает только изображение визитной карточки.

```html 
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard"
    data-render-fallback="none">
</div>
<img src="name:scanned-card-image" />
```


#### <a name="extract-business-card-information-and-render-the-business-card-image-only-if-the-extraction-fails"></a>Извлечение данных визитной карточки и отрисовка ее изображения только при неудачном извлечении

Укажите метод `extract.businesscard` и используйте резервное действие по умолчанию `render`. Если API не может извлечь какой-либо контент, он отрисовывает изображение визитной карточки.

```html
<div
    data-render-src="name:scanned-card-image"
    data-render-method="extract.businesscard">
</div>
```
 
При извлечении данных визитной карточки изображение отправляется в виде именованной части в составном запросе. Примеры отправки изображения в запросе см. в статье [Добавление изображений и файлов](onenote-images-files.md).


<a name="recipe"></a>

## <a name="recipe-extractions"></a>Извлечение рецептов

На основе URL-адреса рецепта API OneNote пытается найти и отобразить указанные ниже сведения.

- Изображение главного имиджевого баннера
- Оценка
- ингредиенты;
- Инструкции
- время подготовки, приготовления и общее;
- Сервировка


<img alt="An example recipe extraction" src="images/recipe-extraction.png" width="200">

API оптимизирован для работы с рецептами со многих популярных сайтов, например *Allrecipes.com*, *FoodNetwork.com* и *SeriousEats.com*.

### <a name="common-scenarios-for-recipe-extractions"></a>Стандартные сценарии извлечения рецептов

#### <a name="extract-recipe-information-and-also-render-a-snapshot-of-the-recipe-webpage"></a>Извлечение рецепта и отображение снимка веб-страницы с рецептом

Укажите метод `extract.recipe` и резервное действие `none`. Кроме того, отправьте элемент `img` с атрибутом `data-render-src`, в качестве значения которого используется URL-адрес рецепта. Если API не может извлечь какой-либо контент, он отображает только снимок веб-страницы с рецептом.

Потенциально этот сценарий дает максимальное количество сведений, так как на веб-странице может быть дополнительная информация, например отзывы и предложения клиентов.

```html 
<div
    data-render-src="https://allrecipes.com/recipe/guacamole/"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<img data-render-src="https://allrecipes.com/recipe/guacamole/" />
```
 

#### <a name="extract-recipe-information-and-render-a-snapshot-of-the-recipe-webpage-only-if-the-extraction-fails"></a>Извлечение рецепта и отображение снимка веб-страницы с рецептом только в случае неудачного извлечения

Укажите метод `extract.recipe` и используйте резервное действие по умолчанию. Если API не может извлечь какой-либо контент, он отображает снимок веб-страницы с рецептом.

```html  
<div
    data-render-src="https://www.foodnetwork.com/recipes/alton-brown/creme-brulee-recipe.html"
    data-render-method="extract.recipe">
</div>
```


#### <a name="extract-recipe-information-and-also-render-a-link-to-the-recipe"></a>Извлечение рецепта и отображение ссылки на рецепт

Укажите метод `extract.recipe` и резервное действие `none`. Кроме того, отправьте элемент `a` с атрибутом `src`, в качестве значения которого задан URL-адрес рецепта (вы также можете отправить любую информацию, которую необходимо добавить на страницу). Если API не может извлечь какой-либо контент, отображается только ссылка на рецепт.

```html  
<div
    data-render-src="https://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html"
    data-render-method="extract.recipe"
    data-render-fallback="none">
</div>
<a href="https://www.seriouseats.com/recipes/2014/09/diy-spicy-kimchi-beef-instant-noodles-recipe.html">Recipe URL</a>
``` 


<a name="product"></a>

## <a name="product-listing-extractions"></a>Извлечение описания товара

- Название
- Оценка
- первичное изображение;
- Описание
- Возможности
- Спецификации



<img alt="An example product listing extraction" src="images/product-extraction.png" width="200">

API оптимизирован для работы с товарами со многих популярных сайтов, например *Amazon.com* и *HomeDepot.com*.

### <a name="common-scenarios-for-recipe-extractions"></a>Стандартные сценарии извлечения рецептов

#### <a name="extract-product-information-and-also-render-a-snapshot-of-the-product-webpage"></a>Извлечение информации о товаре и отображение снимка веб-страницы товара

Укажите метод `extract.product` и резервное действие `none`. Кроме того, отправьте элемент `img` с атрибутом `data-render-src`, в качестве значения которого используется URL-адрес страницы товара. Если API не может извлечь какой-либо контент, он отображает только снимок веб-страницы товара.

Потенциально этот сценарий дает максимальное количество сведений, так как на веб-странице может быть дополнительная информация, например отзывы и предложения клиентов.

```html 
<div
    data-render-src="https://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<img data-render-src="https://www.amazon.com/Microsoft-Band-Small/dp/B00P2T2WVO" />
```


#### <a name="extract-product-information-and-render-a-snapshot-of-the-product-webpage-only-if-the-extraction-fails"></a>Извлечение информации о товаре и отображение снимка веб-страницы с товаром только в случае неудачного извлечения

Укажите метод `extract.product` и используйте резервное действие по умолчанию. Если API не может извлечь какой-либо контент, он вместо этого отображает снимок веб-страницы товара.

```html 
<div
    data-render-src="https://www.sears.com/craftsman-19hp-42-8221-turn-tight-174-hydrostatic-yard-tractor/p-07120381000P"
    data-render-method="extract.product">
</div>
```
 

#### <a name="extract-product-information-and-also-render-a-link-to-the-product"></a>Извлечение информации о товаре и отображение ссылки на товар

Укажите метод `extract.product` и резервное действие `none`. Кроме того, отправьте элемент `a` с атрибутом `src`, в качестве значения которого задан URL-адрес страницы товара (вы также можете отправить любую информацию, которую необходимо добавить на страницу). Если API не может извлечь какой-либо контент, отображается только ссылка на страницу.

```html 
<div
    data-render-src="https://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001"
    data-render-method="extract.product"
    data-render-fallback="none">
</div>
<a href="https://www.homedepot.com/p/Active-Ventilation-5-Watt-Solar-Powered-Exhaust-Attic-Fan-RBSF-8-WT/204203001">Product URL</a>
```


<a name="unknown"></a> 

## <a name="unknown-content-type-extractions"></a>Извлечение содержимого неизвестного типа

Если вы не знаете тип контента (визитная карточка, рецепт или товар), который вы отправляете, вы можете использовать неполный метод `extract` и разрешить API OneNote автоматически определять тип контента. Вы можете сделать это, если ваше приложение отправляет изображения различных типов.

> **Примечание.** Если вы не знаете тип контента, который вы отправляете, используйте метод `extract.businesscard`, `extract.recipe` или `extract.product`. В некоторых случаях это позволяет оптимизировать результаты извлечения.
 
### <a name="common-scenarios-for-unknown-extractions"></a>Стандартные сценарии извлечения контента неизвестного типа

#### <a name="send-an-image-or-a-url-and-render-the-supplied-image-or-a-snapshot-of-the-webpage-if-the-extraction-fails"></a>Отправка изображения или URL-адреса и отображение предоставленного изображения или снимка веб-страницы при неудачном извлечении

Укажите метод `extract`, чтобы API автоматически определял тип контента, и используйте резервное действие по умолчанию. Если API не может извлечь какой-либо контент, он отображает предоставленное изображение или снимок веб-страницы.

```html 
<div
    data-render-src="some image or url"
    data-render-method="extract">
</div>
```


<a name="request-response-info"></a>

## <a name="response-information"></a>Информация в ответе

| Данные в ответе | Описание |  
|------|------|  
| Код успешного завершения действия | Код состояния HTTP 201 при успешном выполнении запроса POST и код состояния HTTP 204 при успешном выполнении запроса PATCH. |  
| Ошибки| Дополнительные сведения об ошибках OneNote, которые может возвращать Microsoft Graph, см. в статье [Коды ошибок для API OneNote в Microsoft Graph](onenote-error-codes.md). |  


<a name="permissions"></a>

## <a name="permissions"></a>Разрешения

Чтобы можно было создавать или изменять страницы OneNote, вам придется запросить соответствующие разрешения. Выберите минимальный уровень разрешений, необходимый для работы вашего приложения.

#### <a name="permissions-for-post-pages"></a>Разрешения для запросов POST со страницами

- Notes.Create
- Notes.ReadWrite
- Notes.ReadWrite.All  

#### <a name="permissions-for-patch-pages"></a>Разрешения в случае запросов PATCH для страниц

- Notes.ReadWrite
- Notes.ReadWrite.All

Дополнительные сведения об областях разрешений и принципе их использования см. в [справочнике по разрешениям Microsoft Graph](permissions-reference.md).


<a name="see-also"></a>

## <a name="see-also"></a>См. также

- [Создание страниц OneNote](onenote-create-page.md)
- [Обновление содержимого страницы OneNote](onenote-update-page.md)
- [Добавление изображений и файлов](onenote-images-files.md)
- [Интеграция с OneNote](integrate-with-onenote.md)
- [Блог разработчиков OneNote](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Вопросы разработки OneNote на сайте «Вопросы и ответы Майкрософт»](/answers/topics/microsoft-graph-notes.html)
- [Репозитории GitHub OneNote](https://go.microsoft.com/fwlink/?LinkID=390178)