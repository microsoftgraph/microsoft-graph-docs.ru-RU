---
title: Тип ресурса searchHit
description: Описание сущности searchHit
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 708945d9f6f28fe1ce83b40f276c5e8d7700112f
ms.sourcegitcommit: 84db9d70672e7a36a1130ff4f4b9baf3554d287f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2022
ms.locfileid: "66810279"
---
# <a name="searchhit-resource-type"></a>Тип ресурса searchHit

Пространство имен: microsoft.graph

Представляет один результат в списке результатов поиска.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|contentSource|Строка|Имя источника контента, **частью которого является externalItem** .|
|hitId|String|Внутренний идентификатор элемента. Формат идентификатора зависит от типа сущности. Дополнительные сведения см. в [формате hitId](#hitid-format).|
|rank|Int32|Ранг или порядок результата.|
|resultTemplateId|Строка|Идентификатор шаблона результата, используемого для отображения результата поиска. Этот идентификатор должен сопоставляться с макетом дисплея в словаре **resultTemplates** , который также включен в [searchResponse](searchresponse.md).|
|resource|[entity](entity.md)|Базовое представление результата поиска в Microsoft Graph.|
|summary|Строка|Сводка результата, если сводка доступна.|

### <a name="hitid-format"></a>Формат hitId

| Тип сущности     | Формат идентификатора        | Пример |
|:-------------|:------------|:------------|
|message|RestId|`AAMkAGIwMDA5MmY0LWY5ZTgtNGY5YS04NzczLWNhNjc0ZGIyZDBjYgBGAAAAAADm35sgHbzESapJ8_BjBlhEBwDAYtphe7dsRbDrOT-HAHoKAACmqNsoAADAYtphe7dsRbDrOT-HAHoKAAFsBhyEAAA=`|
|event|EwsId|`AAMkAGIwMDA5MmY0LWY5ZTgtNGY5YS04NzczLWNhNjc0ZGIyZDBjYgFRAAgI232z8Q+AAEYAAAAA5t+bIB28xEmqSfPgYwZYRAcAwGLaYXu3bEWw6zk/xwB6CgAAAAABDQAAwGLaYXu3bEWw6zk/xwB6CgABGnD/jwAAEA==`|
|список|GUID|`6249f5a0-c9fd-4103-8da5-8362fe911151`|
|listItem|GUID|`89b4aeff-de77-4b0e-bec9-a20cd4f6c32d` |
|site|Host, GUID, GUID|`microsoft.sharepoint.com,a5eb6988-c9ad-44be-b3b4-d334d01066c0,4c5ce7de-dbe6-4807-9909-3018f0b83266`|
|drive|Закодированная строка|`b!kf7AlbfRu0SMqtfcmhLTwf7MGLd-Z0BEqfzvkoqsr21iQFpfPV09TIVf1sa8xOJ0` |
|driveItem|Закодированная строка|`01ALOVTAX7V22IS566BZF35SNCBTKPNQZN`|
|externalItem|Закодированная строка|`AAMkADRiYWU5MDRkLWE1NGEtNDg5OS1hZWM2LWIxOWZmNzQzMTdiYQBGAAAAAAAvZTGE+1bNQp4lDRL1ctayBwCQNOp97HTbQK/QVOV30iomAAAAEF6yAACQNOp97HTbQK/QVOV30iomAAAAG/DWAAA=` |
|person|GUID@GUID|`497b7a2a-9e1a-48d7-80e8-2965d2fc3a81@72f988bf-86f1-41af-91ab-2d7cd011db47`|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHit",
  "baseType": null
}-->

```json
{
  "contentSource": "String",
  "hitId": "String",
  "rank": "Int32",
  "resultTemplateId": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" },
  "summary": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

