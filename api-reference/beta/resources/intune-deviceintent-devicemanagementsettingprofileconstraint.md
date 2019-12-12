---
title: Тип ресурса Девицеманажементсеттингпрофилеконстраинт
description: Ограничение на применение заданной метаданных профиля
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fdd9e308f332d446ad9032736e5f08e8e3545d9e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955689"
---
# <a name="devicemanagementsettingprofileconstraint-resource-type"></a>Тип ресурса Девицеманажементсеттингпрофилеконстраинт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничение на применение заданной метаданных профиля


Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|source|Строка|Источник объекта|
|types|Коллекция объектов string|Коллекция типов, которые несет данный объект|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingProfileConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingProfileConstraint",
  "source": "String",
  "types": [
    "String"
  ]
}
```



