---
title: Тип ресурса Сервицеусеражент
description: Тип Сервицеусеражент
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9cf6b0483ebda33068824f0a3345c12894fd2d7e
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353122"
---
# <a name="serviceuseragent-resource-type"></a>Тип ресурса Сервицеусеражент

Пространство имен: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет агент пользователя службы конечной точки в вызове. Наследуется от типа [UserAgent](callrecords-useragent.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|applicationVersion|String|Определяет версию программного обеспечения приложения, используемого конечной точкой.|
|headerValue|String|Значение заголовка User — Agent, указанное конечной точкой.|
|role|Microsoft. Graph. Каллрекордс. Сервицероле|Определяет роль службы, используемой этой конечной точкой. Возможные значения: `unknown`, `customBot`, `skypeForBusinessMicrosoftTeamsGateway`, `skypeForBusinessAudioVideoMcu`, `skypeForBusinessApplicationSharingMcu`, `skypeForBusinessCallQueues`, `skypeForBusinessAutoAttendant`, `mediationServer`, `mediationServerCloudConnectorEdition`, `exchangeUnifiedMessagingService`, `mediaController`, `conferencingAnnouncementService`, `conferencingAttendant`, `audioTeleconferencerController`, `skypeForBusinessUnifiedCommunicationApplicationPlatform`, `responseGroupServiceAnnouncementService`, `gateway`, `skypeTranslator`, `skypeForBusinessAttendant`, `responseGroupService`, `unknownFutureValue`.|

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