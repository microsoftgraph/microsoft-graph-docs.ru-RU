---
title: Тип ресурса Манажеддевицесуммаризедаппстате
description: Событие, представляющее устройства пользователя с невыполненными или ожидающими приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 566a2f4836f7f24143035b26336063d784e4b727
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023970"
---
# <a name="manageddevicesummarizedappstate-resource-type"></a>Тип ресурса Манажеддевицесуммаризедаппстате

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Событие, представляющее устройства пользователя с невыполненными или ожидающими приложениями.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|суммаризедаппстате|[рунстате](../resources/intune-shared-runstate.md)|Рунстате для объекта. Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|deviceId|String|DeviceId устройства, представленного этим объектом|

## <a name="relationships"></a>Отношения
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






