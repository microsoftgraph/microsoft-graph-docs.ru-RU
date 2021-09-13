---
title: тип ресурса managedDeviceSummarizedAppState
description: Событие, представляющее устройства пользователя с сбойными или ожидающих приложениями.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 092dfef55500ec023c2cf0d79f63c5161c27c7c0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057203"
---
# <a name="manageddevicesummarizedappstate-resource-type"></a>тип ресурса managedDeviceSummarizedAppState

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Событие, представляющее устройства пользователя с сбойными или ожидающих приложениями.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|summarizedAppState|[runState](../resources/intune-troubleshooting-runstate.md)|runState для объекта. Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|deviceId|String|DeviceId устройства, представленного этим объектом|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceSummarizedAppState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceSummarizedAppState",
  "summarizedAppState": "String",
  "deviceId": "String"
}
```




