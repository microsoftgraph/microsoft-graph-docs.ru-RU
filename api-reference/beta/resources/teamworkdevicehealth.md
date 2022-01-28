---
title: тип ресурса teamworkDeviceHealth
description: Представляет сведения о состоянии здоровья устройства с Microsoft Teams с включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0c26b784f42dedc87b02e3a616ff93b7f0c1b46b
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262561"
---
# <a name="teamworkdevicehealth-resource-type"></a>тип ресурса teamworkDeviceHealth

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о состоянии здоровья устройства с [Microsoft Teams с](../resources/teamworkdevice.md) включенной поддержкой. Состояние устройства рассчитывается на основе конфигурации устройства и других параметров устройства.

Наследуется [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get teamworkDeviceHealth](../api/teamworkdevicehealth-get.md)|[teamworkDeviceHealth](../resources/teamworkdevicehealth.md)|Ознакомьтесь с свойствами и отношениями объекта [teamworkDeviceHealth](../resources/teamworkdevicehealth.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|подключение|[teamworkConnection](../resources/teamworkconnection.md)|Сведения о состоянии подключения.|
|createdBy|[identitySet](../resources/identityset.md)|Удостоверение пользователя, создавшего документ о состоянии устройства.|
|createdDateTime|DateTimeOffset|Дата и время создания документа о состоянии устройства.|
|hardwareHealth|[teamworkHardwareHealth](../resources/teamworkhardwarehealth.md)|Сведения о состоянии здоровья оборудования устройства.|
|id|String|Идентификатор Doucument. Наследуется [от сущности](../resources/entity.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Удостоверение пользователя, который в последний раз изменил сведения о состоянии устройства.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения состояния устройства.|
|loginStatus|[teamworkLoginStatus](../resources/teamworkloginstatus.md)|Состояние входа в Microsoft Teams, Skype для бизнеса и Exchange.|
|peripheralsHealth|[teamworkPeripheralsHealth](../resources/teamworkperipheralshealth.md)|Сведения о состоянии здоровья всех периферийных устройств (например, динамика и микрофона), присоединенных к устройству.|
|softwareUpdateHealth|[teamworkSoftwareUpdateHealth](../resources/teamworksoftwareupdatehealth.md)|Обновления программного обеспечения, доступные для устройства.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkDeviceHealth",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDeviceHealth",
  "connection": {
    "@odata.type": "microsoft.graph.teamworkConnection"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "hardwareHealth": {
    "@odata.type": "microsoft.graph.teamworkHardwareHealth"
  },
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "loginStatus": {
    "@odata.type": "microsoft.graph.teamworkLoginStatus"
  },
  "peripheralsHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralsHealth"
  },
  "softwareUpdateHealth": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateHealth"
  }
}
```

