---
title: Тип ресурса windowsInformationProtectionStoreApp
description: Защита данных приложений для Windows из Microsoft Store
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 895267d331200939ffd86a5c811e8459db982f0a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994421"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a>Тип ресурса windowsInformationProtectionStoreApp

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Защита данных приложений для Windows из Microsoft Store


Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя приложения. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|description|Строка|Описание приложения. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|publisherName|String|Имя издателя. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|productName|String|Название продукта. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|denied|Boolean|Если задано значение true, то приложению отказано в защите или исключении. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionStoreApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```





