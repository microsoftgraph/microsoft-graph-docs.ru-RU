---
title: Тип ресурса windowsInformationProtectionStoreApp
description: Защита данных приложений для Windows из Microsoft Store
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fa2059f7e85c180d4ff091a4596267471d772e3d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986616"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a>Тип ресурса windowsInformationProtectionStoreApp

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Защита данных приложений для Windows из Microsoft Store

Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя приложения. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|описание|String|Описание приложения. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|publisherName|String|Имя издателя. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|productName|String|Название продукта. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|denied|Boolean|Если задано значение true, то приложению отказано в защите или исключении. Наследуется от [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|

## <a name="relationships"></a>Связи
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





