---
title: Тип ресурса numberRange
description: Определение номер диапазона.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5b428320fd66263149b6d443a15c6a0e1eee744a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845705"
---
# <a name="numberrange-resource-type"></a>Тип ресурса numberRange

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Определение номер диапазона.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
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





