---
title: Тип ресурса windowsInformationProtectionResourceCollection
description: Коллекция ресурсов Windows Information Protection
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b7e706e83753a49e7eece3d2efef95b7113a8cf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342091"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a>Тип ресурса windowsInformationProtectionResourceCollection

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Коллекция ресурсов Windows Information Protection

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя|
|resources|Коллекция строк|Коллекция ресурсов|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```



