---
title: Тип ресурса Сервицеусеражент
description: Тип Сервицеусеражент
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 052c177e2cef4adf5a882408c3cdef3a211dea73
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069332"
---
# <a name="serviceuseragent-resource-type"></a>Тип ресурса Сервицеусеражент

Пространство имен: microsoft.graph.callRecords

Представляет агент пользователя службы конечной точки в вызове. Наследуется от типа [UserAgent](callrecords-useragent.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|applicationVersion|String|Определяет версию программного обеспечения приложения, используемого конечной точкой.|
|headerValue|Строка|Значение заголовка User — Agent, указанное конечной точкой.|
|role|Microsoft. Graph. Каллрекордс. Сервицероле|Определяет роль службы, используемой этой конечной точкой. Возможные значения: `unknown` ,,,,,,,,,,,,,,,,,,,,,,,,,,, `customBot` `skypeForBusinessMicrosoftTeamsGateway` `skypeForBusinessAudioVideoMcu` `skypeForBusinessApplicationSharingMcu` `skypeForBusinessCallQueues` `skypeForBusinessAutoAttendant` `mediationServer` `mediationServerCloudConnectorEdition` `exchangeUnifiedMessagingService` `mediaController` `conferencingAnnouncementService` `conferencingAttendant` `audioTeleconferencerController` `skypeForBusinessUnifiedCommunicationApplicationPlatform` `responseGroupServiceAnnouncementService` `gateway` `skypeTranslator` `skypeForBusinessAttendant` `responseGroupService` `voicemail` `unknownFutureValue` .|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.serviceUserAgent",
  "baseType": "microsoft.graph.callRecords.userAgent"
}-->

```json
{
  "applicationVersion": "String",
  "headerValue": "String",
  "role": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceUserAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
