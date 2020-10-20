---
title: Тип ресурса Сервицеусеражент
description: Тип Сервицеусеражент
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b3d939042c4688ee3512ad380e0f3f75e0badffa
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601463"
---
# <a name="serviceuseragent-resource-type"></a>Тип ресурса Сервицеусеражент

Пространство имен: microsoft.graph.callRecords

Представляет агент пользователя службы конечной точки в вызове. Наследуется от типа [UserAgent](callrecords-useragent.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|applicationVersion|String|Определяет версию программного обеспечения приложения, используемого конечной точкой.|
|headerValue|String|Значение заголовка User — Agent, указанное конечной точкой.|
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
