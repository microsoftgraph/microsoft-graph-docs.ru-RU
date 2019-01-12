---
title: Тип ресурса iosHomeScreenItem
description: Представляет элемент на начальном экране iOS
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 477be5c509ab4d062a695c4b8df7eb00af6f51fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962606"
---
# <a name="ioshomescreenitem-resource-type"></a>Тип ресурса iosHomeScreenItem

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Представляет элемент на начальном экране iOS
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя приложения|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```





