---
title: Тип ресурса learningContent
description: Представляет сущность, содержащую сведения о содержимом обучения.
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: resourcePageType
ms.openlocfilehash: 865070a402c68327a1fef41b6c793e5672f878c3
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883371"
---
# <a name="learningcontent-resource-type"></a>Тип ресурса learningContent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет метаданные содержимого для обучения сотрудников.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление learningContents](../api/learningprovider-list-learningcontents.md)|[Коллекция learningContent](../resources/learningcontent.md)|Получение списка ресурсов [learningContent](../resources/learningcontent.md) и их свойств. Этот список представляет метаданные содержимого указанного поставщика в Viva Обучение.|
|[Получение learningContent](../api/learningcontent-get.md)|[learningContent](../resources/learningcontent.md)|Возвращает указанный ресурс learningContent, который представляет метаданные принимаемых содержимого указанного поставщика.|
|[Обновление learningContent](../api/learningcontent-update.md)|[learningContent](../resources/learningcontent.md)|Обновите [указанный ресурс learningContent](../resources/learningcontent.md) . Используется поставщиком [обучения для](learningprovider.md) приема или обновления метаданных для своего содержимого в Viva Обучение.|
|[Удаление learningContent](../api/learningprovider-delete-learningcontents.md)|Нет|Удалите указанный ресурс learningContent, представляющий метаданные принимаемых содержимого указанного поставщика.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|additionalTags|Коллекция строк|Ключевые слова, разделы и другие теги, связанные с содержимым обучения. Необязательный элемент.|
|contentWebUrl|String|URL-адрес веб-сайта для обучающего содержимого. Обязательный.|
|Вклад|Строка|Автор, создатель или участник обучающего содержимого. Необязательный элемент.|
|createdDateTime|DateTimeOffset|Дата создания обучающего содержимого. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Необязательный элемент.|
|description|Строка|Описание или сводка для обучающего содержимого. Необязательный элемент.|
|duration|Длительность|Длительность обучающего содержимого в секундах. Необязательный элемент.|
|externalId|String|Уникальный идентификатор внешнего содержимого для обучающего содержимого. Обязательный.|
|format|Строка|Формат обучающего содержимого. Например, `Course`, `Video`, `Book`, `Book Summary`. `Audiobook Summary` Необязательный элемент.|
|isActive|Логический|Указывает, является ли содержимое активным. Неактивное содержимое не будет отображаться в пользовательском интерфейсе. Значение по умолчанию — `true`. Необязательный элемент.|
|isPremium|Логический|Указывает, требуется ли пользователю входить в систему на платформе поставщика обучения. Значение по умолчанию — `false`. Необязательный элемент.|
|isSearchable|Логический|Указывает, поддерживается ли поиск в обучающем содержимом. Значение по умолчанию — `true`. Необязательный элемент.|
|languageTag|String|Язык обучающего содержимого, например , `en-us` или `fr-fr`. Обязательный атрибут.|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения обучающего содержимого. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Необязательный элемент.|
|numberOfPages|Int32|Число страниц обучающего содержимого, например 9. Необязательный элемент.|
|SkillTags|Коллекция строк|Теги навыков, связанные с содержимым обучения. Необязательный элемент.|
|sourceName|String|Исходное имя обучающего содержимого, например или `LinkedIn Learning` `Coursera`. Необязательный элемент.|
|thumbnailWebUrl|Строка|URL-адрес эскиза содержимого обучения. Необязательный элемент.|
|title|Строка|Заголовок обучающего содержимого. Обязательный.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.learningContent",
  "openType": false
}
-->
``` json
{
    "@odata.type": "#microsoft.graph.learningContent",
    "additionalTags": [
        "String"
    ],
    "contentWebUrl": "String",
    "contributor": "String",
    "createdDateTime": "String (timestamp)",
    "description": "String",
    "duration": "String (duration)",
    "externalId": "String",
    "format": "String",
    "isActive": "Boolean",
    "isPremium": "Boolean",
    "isSearchable": "Boolean",
    "languageTag": "String",
    "lastModifiedDateTime": "String (timestamp)",
    "numberOfPages": "Integer",
    "skillTags": [
        "String"
    ],
    "sourceName": "String",
    "thumbnailWebUrl": "String",
    "title": "String"
}
```

