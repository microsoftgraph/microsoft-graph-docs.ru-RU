---
title: Обновление learningContent
description: Обновление свойств объекта learningContent.
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: apiPageType
ms.openlocfilehash: 80e9caa91d973e90e0f7b8d9f4ccb07708dbdb4f
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883403"
---
# <a name="update-learningcontent"></a>Обновление learningContent
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновите [указанный ресурс learningContent](../resources/learningcontent.md) . 

Используется поставщиком [обучения для](../resources/learningprovider.md) приема или обновления метаданных для своего содержимого в Viva Обучение. Если указанное обучающее содержимое еще не существует для указанного поставщика, эта операция создает метаданные для нового содержимого. В противном случае эта операция заменяет метаданные существующего содержимого.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|LearningContent.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|LearningContent.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /employeeExperience/learningProviders/{registrationId}/learningContents(externalId='{externalId}') 
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Свойство|Тип|Описание|
|:---|:---|:---|
|additionalTags|Коллекция строк|Ключевые слова, разделы и другие теги, связанные с содержимым обучения. Необязательный элемент.|
|contentWebUrl|String|URL-адрес веб-сайта для обучающего содержимого. Обязательный.|
|Вклад|String|Автор, создатель или участник обучающего содержимого. Необязательный элемент.|
|createdDateTime|DateTimeOffset|Дата создания обучающего содержимого. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Необязательный элемент.|
|description|Строка|Описание или сводка для обучающего содержимого. Необязательный элемент.|
|duration|Длительность|Длительность обучающего содержимого в секундах. Необязательный элемент.|
|externalId|String|Уникальный идентификатор внешнего содержимого для обучающего содержимого. Обязательный.|
|format|String|Формат обучающего содержимого. Например, `Course`, `Video`, `Book`, `Book Summary`. `Audiobook Summary` Необязательный элемент.|
|isActive|Логический|Указывает, является ли содержимое активным. Неактивное содержимое не будет отображаться в пользовательском интерфейсе. Значение по умолчанию — `true`. Необязательный элемент.|
|isPremium|Логический|Указывает, требуется ли пользователю входить в систему на платформе поставщика обучения. Значение по умолчанию — `false`. Необязательный элемент.|
|isSearchable|Логический|Указывает, поддерживается ли поиск в обучающем содержимом. Значение по умолчанию — `true`. Необязательный элемент.|
|languageTag|Строка|Язык обучающего содержимого, например , `en-us` или `fr-fr`. Обязательный атрибут.|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения обучающего содержимого. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Необязательный элемент.|
|numberOfPages|Int32|Число страниц обучающего содержимого, например 9. Необязательный элемент.|
|SkillTags|Коллекция строк|Теги навыков, связанные с содержимым обучения. Необязательный элемент.|
|sourceName|String|Исходное имя обучающего содержимого, например или `LinkedIn Learning` `Coursera`. Необязательный элемент.|
|thumbnailWebUrl|Строка|URL-адрес эскиза содержимого обучения. Необязательный элемент.|
|title|Строка|Заголовок обучающего содержимого. Обязательный.|



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `202 Accepted` отклика и обновленный объект [learningContent](../resources/learningcontent.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_learningcontent"
}
-->
``` http
PATCH /employeeExperience/learningProviders/13727311-e7bb-470d-8b20-6a23d9030d70/learningContents(externalId='LP4471') 
Content-Type: application/json

{
    "title": "Manage classes, resources, assessment, and planning in Microsoft Teams with Beedle",
    "description": "A module to guide users through the various teaching and learning enhancements that Beedle provides within Microsoft Teams, with many examples of everyday application.",
    "contentWebUrl": "https://docs.microsoft.com/en-us/learn/modules/manage-classes-resources-assessment-planning-beedle/",
    "sourceName": "MsLearn",
    "thumbnailWebUrl": "https://syndetics.com/index.aspx?isbn=9783319672175/LC.GIF",
    "languageTag": "en-us",
    "numberOfPages": 9,
    "duration": "PT20M",
    "format": "Book",
    "createdDateTime": "2018-01-01T00:00:00",
    "lastModifiedDateTime": "2021-04-01T04:26:06.1995367Z",
    "contributor": "Scott Simpson",
    "additionalTags": [
        "Create private or public teams",
        "Add members to teams"
    ],
    "skillTags": [
        "Create teams",
        "Teams channels",
        "Teams members"
    ],
    "isActive": true,
    "isPremium": false,
    "isSearchable": true
}
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.learningContent"
}
-->
``` http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#learningProviders('13727311-e7bb-470d-8b20-6a23d9030d70')/learningContents/$entity",
    "externalId": "LP4471",
    "title": "Manage classes, resources, assessment, and planning in Microsoft Teams with Beedle",
    "description": "A module to guide users through the various teaching and learning enhancements that Beedle provides within Microsoft Teams, with many examples of everyday application.",
    "contentWebUrl": "https://docs.microsoft.com/en-us/learn/modules/manage-classes-resources-assessment-planning-beedle/",
    "sourceName": "MsLearn",
    "thumbnailWebUrl": "https://syndetics.com/index.aspx?isbn=9783319672175/LC.GIF",
    "languageTag": "en-us",
    "numberOfPages": 9,
    "duration": "PT20M",
    "format": "Book",
    "createdDateTime": "2018-01-01T00:00:00",
    "lastModifiedDateTime": "2021-04-01T04:26:06.1995367Z",
    "contributor": "Scott Simpson",
    "additionalTags": [
        "Create private or public teams",
        "Add members to teams"
    ],
    "skillTags": [
        "Create teams",
        "Teams channels",
        "Teams members"
    ],
    "isActive": true,
    "isPremium": false,
    "isSearchable": true
}
```

