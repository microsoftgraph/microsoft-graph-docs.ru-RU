---
title: тип ресурса teamworkDeviceActivity
description: Представляет сведения о действиях для Microsoft Teams устройства с включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 43e9e81eb8c2f921ce3657bf42c4a94f17c7c236
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262597"
---
# <a name="teamworkdeviceactivity-resource-type"></a>тип ресурса teamworkDeviceActivity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о действиях для устройства с [Microsoft Teams с](../resources/teamworkdevice.md) включенной поддержкой, включая активные периферийные устройства, присоединенные к устройству.

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получить teamworkDeviceActivity](../api/teamworkdeviceactivity-get.md)|[teamworkDeviceActivity](../resources/teamworkdeviceactivity.md)|Ознакомьтесь с свойствами и отношениями объекта [teamworkDeviceActivity](../resources/teamworkdeviceactivity.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|activePeripherals|[teamworkActivePeripherals](../resources/teamworkactiveperipherals.md)|Активные периферийные устройства, присоединенные к устройству.|
|createdBy|[identitySet](../resources/identityset.md)|Удостоверение пользователя, создавшего документ действий устройства.|
|createdDateTime|DateTimeOffset|Дата и время создания документа действий устройства.|
|id|String|Идентификатор документа. Наследуется [от сущности](../resources/entity.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Удостоверение пользователя, который в последний раз изменил сведения о действиях устройства.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения даты и времени действия устройства.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkDeviceActivity",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDeviceActivity",
  "activePeripherals": {
    "@odata.type": "microsoft.graph.teamworkActivePeripherals"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```

