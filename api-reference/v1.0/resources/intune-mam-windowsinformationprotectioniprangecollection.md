---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: af96367c0cbe5d9b91e41eb9ff5be3babbe31669
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60454147"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a>Тип ресурса windowsInformationProtectionIPRangeCollection

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Коллекция диапазонов IP-адресов Windows Information Protection

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя|
|ranges|Коллекция объектов [ipRange](../resources/intune-mam-iprange.md)|Коллекция диапазонов IP-адресов|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.ipRange"
    }
  ]
}
```



