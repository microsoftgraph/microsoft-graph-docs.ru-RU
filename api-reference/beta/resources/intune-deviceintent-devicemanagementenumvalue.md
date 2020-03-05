---
title: Тип ресурса Девицеманажементенумвалуе
description: Сведения об определении значения перечисления
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8400aa7228fbc04e52a66074380f302f02e66823
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528859"
---
# <a name="devicemanagementenumvalue-resource-type"></a>Тип ресурса Девицеманажементенумвалуе

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения об определении значения перечисления

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|значение|String|Необработанный текст значения перечисления|
|displayName|String|Отображаемое имя для этого значения перечисления|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementEnumValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementEnumValue",
  "value": "String",
  "displayName": "String"
}
```



