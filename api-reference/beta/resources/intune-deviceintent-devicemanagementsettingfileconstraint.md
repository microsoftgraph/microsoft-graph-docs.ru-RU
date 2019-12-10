---
title: Тип ресурса Девицеманажементсеттингфилеконстраинт
description: Ограничение, обеспечивающее расширение файла, приемлемо для данного параметра
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60ff6a00e30e328daf2330e39511956ec1ab1f18
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39924628"
---
# <a name="devicemanagementsettingfileconstraint-resource-type"></a>Тип ресурса Девицеманажементсеттингфилеконстраинт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничение, обеспечивающее расширение файла, приемлемо для данного параметра


Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|суппортедекстенсионс|Коллекция строк|Допустимые расширения файлов для отправки для этого параметра|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingFileConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingFileConstraint",
  "supportedExtensions": [
    "String"
  ]
}
```



