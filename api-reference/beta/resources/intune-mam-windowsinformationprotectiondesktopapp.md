---
title: Тип ресурса windowsInformationProtectionDesktopApp
description: Защита данных классических приложений для Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cbb67edbbe38687e06c5952399a6d5bf02b5f56
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994561"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a>Тип ресурса windowsInformationProtectionDesktopApp

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Защита данных классических приложений для Windows


Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя приложения. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|description|Строка|Описание приложения. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|publisherName|String|Имя издателя. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|productName|String|Название продукта. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|denied|Boolean|Если задано значение true, то приложению отказано в защите или исключении. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|binaryName|String|Двоичное имя.|
|binaryVersionLow|String|Нижняя двоичная версия.|
|binaryVersionHigh|String|Верхняя двоичная версия.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDesktopApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true,
  "binaryName": "String",
  "binaryVersionLow": "String",
  "binaryVersionHigh": "String"
}
```





