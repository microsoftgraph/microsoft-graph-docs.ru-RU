---
title: тип ресурса teleconferenceDeviceQuality
description: Представляет данные о качестве сеанса сеанса видеоконференции устройства.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 655ebbbc65f62ec3ace0640ed012b2d89bc0e6adb8242218ae223f57ab36d34f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218396"
---
# <a name="teleconferencedevicequality-resource-type"></a>тип ресурса teleconferenceDeviceQuality

Пространство имен: microsoft.graph

Представляет данные о качестве сеанса сеанса видеоконференции устройства.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|callChainId|Guid|Уникальный идентификатор для всех звонков участника конференции или уникальный идентификатор для двух вызовов участников в вызове P2P. Необходимо скопировать из `Microsoft.Graph.Call.CallChainId`.|
|cloudServiceDeploymentEnvironment|String|Гео-регион, в котором развернута служба, например `ProdNoam` .|
|cloudServiceDeploymentId|String|Уникальный идентификатор развертывания, присвоенный Azure.|
|cloudServiceInstanceName|String|Имя экземпляра развернутой облачной службы Azure, например `FrontEnd_IN_3` .|
|cloudServiceName|String|Имя развернутой облачной службы Azure, например `contoso.cloudapp.net` .|
|deviceDescription|String|Любое дополнительное описание, например `VTC Bldg 30/21` .|
|deviceName|String|Имя агента мультимедиа пользователя, например `Cisco SX80` .|
|mediaLegId|Guid|Уникальный идентификатор для определенной области мультимедиа участника конференции.  Один участник может иметь несколько идентификаторов ног мультимедиа, если происходит перенацеление. Партнер CVI назначает это значение.|
|mediaQualityList|[коллекция teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md)|Список качеств мультимедиа в сеансе мультимедиа (вызов), таких как качество звука, качество видео и/или качество обмена экранами.|
|participantId|Guid|Уникальный идентификатор для конкретного участника конференции. ПартнерУ CVI необходимо скопировать это `Call.MyParticipantId` свойство.|

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

