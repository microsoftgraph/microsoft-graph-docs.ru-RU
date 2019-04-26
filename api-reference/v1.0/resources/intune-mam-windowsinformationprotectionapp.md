---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00d329baea829fa8fb7664895382a377f53461ab
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561204"
---
# <a name="windowsinformationprotectionapp-resource-type"></a>Тип ресурса windowsInformationProtectionApp

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Защита данных приложений для Windows

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя приложения.|
|description|String|Описание приложения.|
|publisherName|String|Имя издателя|
|productName|String|Название продукта.|
|denied|Boolean|Если задано значение true, то приложению отказано в защите или исключении.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



