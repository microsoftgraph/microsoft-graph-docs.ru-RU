---
title: Тип ресурса iosBookmark
description: URL-адрес закладку операций ввода-вывода
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 37cdcc1b886914b4b42e0a97e8947a565c75f5b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841001"
---
# <a name="iosbookmark-resource-type"></a>Тип ресурса iosBookmark

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

URL-адрес закладку операций ввода-вывода
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|url|String|Разрешен доступ к URL-адрес|
|bookmarkFolder|Строка|Папка, в которую будет добавлен закладки в Safari|
|displayName|Строка|Отображаемое имя закладки|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosBookmark"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosBookmark",
  "url": "String",
  "bookmarkFolder": "String",
  "displayName": "String"
}
```





