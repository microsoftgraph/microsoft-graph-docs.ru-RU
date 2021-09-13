---
title: тип ресурса verifiedPublisher
description: Представляет проверенного издателя приложения.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: jesakowi
ms.openlocfilehash: 4c63c0cdcfb6324077092923eeff91eed65e7b60
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134285"
---
# <a name="verifiedpublisher-resource-type"></a>тип ресурса verifiedPublisher

Пространство имен: microsoft.graph

Представляет проверенного издателя [приложения](application.md). Дополнительные сведения см. [в Publisher проверки.](/azure/active-directory/develop/publisher-verification-overview) Проверенные издатели устанавливаются с помощью [setVerifiedPublisher](../api/application-setverifiedpublisher.md) и могут быть удалены только с помощью [unsetVerifiedPublisher.](../api/application-unsetverifiedpublisher.md)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|displayName|Строка|Проверенное имя издателя из учетной записи Центра партнеров издателя приложения.|
|verifiedPublisherId|Строка| ID проверенного издателя из учетной записи Центра партнеров издателя приложений. |
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
