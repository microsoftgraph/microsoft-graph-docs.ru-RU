---
title: Тип ресурса numberRange
description: Определение номер диапазона.
ms.openlocfilehash: ef4b24e3034414221365d81c40b453e7ca66a94b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075148"
---
# <a name="numberrange-resource-type"></a>Тип ресурса numberRange

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Определение номер диапазона.
## <a name="properties"></a>Свойства
|Свойство|Тип|Description|
|:---|:---|:---|
|lowerNumber|Int32|Меньшее число.|
|upperNumber|Int32|Верхний номер.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```





