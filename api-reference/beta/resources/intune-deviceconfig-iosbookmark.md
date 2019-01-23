---
title: Тип ресурса iosBookmark
description: URL-адрес закладку операций ввода-вывода
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e95f3bfd40bdf5ca5782aa9233a020623d32d6a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395911"
---
# <a name="iosbookmark-resource-type"></a>Тип ресурса iosBookmark

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

URL-адрес закладку операций ввода-вывода

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|url|String|Разрешен доступ к URL-адрес|
|bookmarkFolder|String|Папка, в которую будет добавлен закладки в Safari|
|displayName|String|Отображаемое имя закладки|

## <a name="relationships"></a>Отношения
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




