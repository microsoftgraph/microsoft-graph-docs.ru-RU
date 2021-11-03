---
title: тип ресурса verifiedPublisher
description: Представляет проверенного издателя приложения.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: jesakowi
ms.openlocfilehash: c65456a7dbe9b1adcb57a19a75ebf6322e84a189
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60684065"
---
# <a name="verifiedpublisher-resource-type"></a>тип ресурса verifiedPublisher

Пространство имен: microsoft.graph

Представляет проверенного издателя [приложения](application.md). Дополнительные сведения см. [в Publisher проверки.](/azure/active-directory/develop/publisher-verification-overview) Проверенные издатели устанавливаются с помощью [setVerifiedPublisher](../api/application-setverifiedpublisher.md) и могут быть удалены только с помощью [unsetVerifiedPublisher.](../api/application-unsetverifiedpublisher.md)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|addedDateTime|DateTimeOffSet| Время, когда проверенный издатель был добавлен или обновлен совсем недавно. |
|displayName|String|Проверенное имя издателя из учетной записи Центра партнеров издателя приложения.|
|verifiedPublisherId|String| ID проверенного издателя из учетной записи Центра партнеров издателя приложений. |


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedPublisher"
}-->

```json
{
  "displayName": "String",
  "verifiedPublisherId": "String",
  "addedDateTime": "DateTimeOffSet"
}
```


<!-- uuid: 7a355221-34dd-4579-9bdd-4c3e1909e1bb
2020-09-09 20:45:56 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "verifiedPublisher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
