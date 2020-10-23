---
title: Тип ресурса Девицеманажементенумвалуе
description: Сведения об определении значения перечисления
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 943a7c825dc1ee38ec74c6f50d866b6d550782c6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696120"
---
# <a name="devicemanagementenumvalue-resource-type"></a>Тип ресурса Девицеманажементенумвалуе

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения об определении значения перечисления

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|значение|String|Необработанный текст значения перечисления|
|displayName|Строка|Отображаемое имя для этого значения перечисления|

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





