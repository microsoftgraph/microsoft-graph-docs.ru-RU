---
title: Тип ресурса Телеконференцедевицекуалити
description: Представляет данные качества на уровне сеанса видеоконференций для видеоконференций.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4d76114a35a9ac7d0c9901437b672697c295ebbf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42763272"
---
# <a name="teleconferencedevicequality-resource-type"></a>Тип ресурса Телеконференцедевицекуалити

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет данные качества на уровне сеанса видеоконференций для видеоконференций.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|callChainId|GUID|Уникальный идентификатор для всех вызовов участников в конференции или уникальный идентификатор для двух вызовов участников в вызове P2P. Необходимо скопировать из `Microsoft.Graph.Call.CallChainId`.|
|клаудсервицедеплойментенвиронмент|String|Географическая область, в которой развернута служба, `ProdNoam`например.|
|клаудсервицедеплойментид|String|Уникальный идентификатор развертывания, назначенный Azure.|
|клаудсервицеинстанценаме|String|Имя развернутого экземпляра облачной службы Azure, `FrontEnd_IN_3`например.|
|клаудсервиценаме|String|Имя развернутой облачной службы Azure, `contoso.cloudapp.net`например.|
|девицедескриптион|String|Любое дополнительное описание, например `VTC Bldg 30/21`.|
|deviceName|String|Имя агента мультимедиа пользователя, например `Cisco SX80`.|
|медиалегид|GUID|Уникальный идентификатор для конкретной точки носителя участника в Конференции.  Если происходит переопределение, у одного участника может быть несколько идентификаторов носителей. Партнер Кви назначает это значение.|
|медиакуалитилист|Коллекция [телеконференцедевицемедиакуалити](teleconferencedevicemediaquality.md)|Список качеств мультимедиа в сеансе мультимедиа (вызов), например качество звука, качество видео и/или общий доступ к экрану.|
|партиЦипантид|GUID|Уникальный идентификатор определенного участника в Конференции. Партнеру Кви необходимо скопировать `Call.MyParticipantId` значение этого свойства.|

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
