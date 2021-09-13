---
title: тип ресурса teleconferenceDeviceQuality
description: Представляет данные о качестве сеанса сеанса видеоконференции устройства.
ms.localizationpriority: medium
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6e7b29330634b099974300c660b45923b31b9b66
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128090"
---
# <a name="teleconferencedevicequality-resource-type"></a>тип ресурса teleconferenceDeviceQuality

Пространство имен: microsoft.graph

Представляет данные о качестве сеанса сеанса видеоконференции устройства.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|callChainId|Guid|Уникальный идентификатор для всех звонков участника конференции или уникальный идентификатор для двух вызовов участников в вызове P2P. Необходимо скопировать из `Microsoft.Graph.Call.CallChainId`.|
|cloudServiceDeploymentEnvironment|Строка|Гео-регион, в котором развернута служба, например `ProdNoam` .|
|cloudServiceDeploymentId|Строка|Уникальный идентификатор развертывания, присвоенный Azure.|
|cloudServiceInstanceName|Строка|Имя экземпляра развернутой облачной службы Azure, например `FrontEnd_IN_3` .|
|cloudServiceName|String|Имя развернутой облачной службы Azure, например `contoso.cloudapp.net` .|
|deviceDescription|Строка|Любое дополнительное описание, например `VTC Bldg 30/21` .|
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

