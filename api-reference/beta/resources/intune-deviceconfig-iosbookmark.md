---
title: Тип ресурса iosBookmark
description: Закладки URL-адресов iOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ee61f1b0b45d735c6c738db6220d84b3cc962b6b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788235"
---
# <a name="iosbookmark-resource-type"></a>Тип ресурса iosBookmark

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Закладки URL-адресов iOS

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|url|String|URL-адрес, разрешенный для доступа|
|bookmarkFolder|Строка|Папка, в которую должна быть добавлена закладка в Safari|
|displayName|Строка|Имя отображения закладки|

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



