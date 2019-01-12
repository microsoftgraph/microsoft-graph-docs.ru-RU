---
title: Тип ресурса iosBookmark
description: URL-адрес закладку операций ввода-вывода
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cbf39a2eee5064b7d3ddfa474b1f70758d4c7047
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938176"
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





