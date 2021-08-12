---
title: тип ресурса verifiedPublisher
description: Представляет проверенного издателя приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: jesakowi
ms.openlocfilehash: f53559da47f61de645661c1acc8e0a94e4a6e6e6e9cf3c55e6faa8e2149452a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129906"
---
# <a name="verifiedpublisher-resource-type"></a>тип ресурса verifiedPublisher

Пространство имен: microsoft.graph

Представляет проверенного издателя [приложения](application.md). Дополнительные сведения см. [в Publisher проверки.](/azure/active-directory/develop/publisher-verification-overview) Проверенные издатели устанавливаются с помощью [setVerifiedPublisher](../api/application-setverifiedpublisher.md) и могут быть удалены только с помощью [unsetVerifiedPublisher.](../api/application-unsetverifiedpublisher.md)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|displayName|String|Проверенное имя издателя из учетной записи Центра партнеров издателя приложения.|
|verifiedPublisherId|String| ID проверенного издателя из учетной записи Центра партнеров издателя приложений. |
|addedDateTime|DateTimeOffSet| Время, когда проверенный издатель был добавлен или обновлен совсем недавно. |


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
