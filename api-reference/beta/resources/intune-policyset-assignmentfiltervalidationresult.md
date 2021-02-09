---
title: Тип ресурса assignmentFilterValidationResult
description: Представляет результат проверки API.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a540bdec4265c544f565e560b6858755d0076178
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160956"
---
# <a name="assignmentfiltervalidationresult-resource-type"></a>Тип ресурса assignmentFilterValidationResult

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет результат проверки API.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isValidRule|Boolean|Индикатор допустимым или недопустимым правилом.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterValidationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterValidationResult",
  "isValidRule": true
}
```




