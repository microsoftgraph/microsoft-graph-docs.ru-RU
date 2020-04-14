---
title: Тип ресурса Девицеманажементенумвалуе
description: Сведения об определении значения перечисления
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 70b8bc8b0760c0879ab5384620839d717ac7a41d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455703"
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



