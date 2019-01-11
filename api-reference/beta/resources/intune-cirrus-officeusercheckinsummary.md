---
title: Тип ресурса officeUserCheckinSummary
description: Сущности, которая описывает клиента возврат stats.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c2470b1e531f1b268d6797fe2692baf0031728b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834024"
---
# <a name="officeusercheckinsummary-resource-type"></a>Тип ресурса officeUserCheckinSummary

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Сущности, которая описывает клиента возврат stats.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|succeededUserCount|Int32|Всего успешных пользователя проверьте ins за последние три месяца.|
|failedUserCount|Int32|Всего неудачных пользователя проверьте ins за последние три месяца.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeUserCheckinSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeUserCheckinSummary",
  "succeededUserCount": 1024,
  "failedUserCount": 1024
}
```



