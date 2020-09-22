---
title: Тип ресурса Телеконференцедевицекуалити
description: Представляет данные качества на уровне сеанса видеоконференций для видеоконференций.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 455a69257e880c71c28fa7968e5e8294075437e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086279"
---
# <a name="teleconferencedevicequality-resource-type"></a>Тип ресурса Телеконференцедевицекуалити

Пространство имен: microsoft.graph

Представляет данные качества на уровне сеанса видеоконференций для видеоконференций.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|callChainId|Guid|Уникальный идентификатор для всех вызовов участников в конференции или уникальный идентификатор для двух вызовов участников в вызове P2P. Необходимо скопировать из `Microsoft.Graph.Call.CallChainId`.|
|клаудсервицедеплойментенвиронмент|Строка|Географическая область, в которой развернута служба, например `ProdNoam` .|
|клаудсервицедеплойментид|Строка|Уникальный идентификатор развертывания, назначенный Azure.|
|клаудсервицеинстанценаме|Строка|Имя развернутого экземпляра облачной службы Azure, например `FrontEnd_IN_3` .|
|клаудсервиценаме|Строка|Имя развернутой облачной службы Azure, например `contoso.cloudapp.net` .|
|девицедескриптион|Строка|Любое дополнительное описание, например `VTC Bldg 30/21` .|
|deviceName|String|Имя агента мультимедиа пользователя, например `Cisco SX80` .|
|медиалегид|Guid|Уникальный идентификатор для конкретной точки носителя участника в Конференции.  Если происходит переопределение, у одного участника может быть несколько идентификаторов носителей. Партнер Кви назначает это значение.|
|медиакуалитилист|Коллекция [телеконференцедевицемедиакуалити](teleconferencedevicemediaquality.md)|Список качеств мультимедиа в сеансе мультимедиа (вызов), например качество звука, качество видео и/или общий доступ к экрану.|
|партиЦипантид|Guid|Уникальный идентификатор определенного участника в Конференции. Партнеру Кви необходимо скопировать значение `Call.MyParticipantId` этого свойства.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceQuality",
  "baseType": null
}-->

```json
{
  "callChainId": "Guid",
  "cloudServiceDeploymentEnvironment": "String",
  "cloudServiceDeploymentId": "String",
  "cloudServiceInstanceName": "String",
  "cloudServiceName": "String",
  "deviceDescription": "String",
  "deviceName": "String",
  "mediaLegId": "Guid",
  "mediaQualityList": [{"@odata.type": "microsoft.graph.teleconferenceDeviceMediaQuality"}],
  "participantId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teleconferenceDeviceQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

