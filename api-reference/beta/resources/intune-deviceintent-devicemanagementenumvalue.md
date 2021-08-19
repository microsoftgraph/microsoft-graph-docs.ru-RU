---
title: тип ресурса deviceManagementEnumValue
description: Сведения об определении для значения enum
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e2492208bd2d0f85e5d8e548fde5af0f82ff01a84c9a68d9fc1db77c827e4473
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206433"
---
# <a name="devicemanagementenumvalue-resource-type"></a>тип ресурса deviceManagementEnumValue

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения об определении для значения enum

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|значение|String|Текст необработанных значений в переименовку|
|displayName|Строка|Отображение имени для этого значения в переуме|

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




