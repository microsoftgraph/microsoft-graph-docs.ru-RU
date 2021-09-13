---
title: Тип ресурса iosBookmark
description: Закладки URL-адресов iOS
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2df99ad3410864cc6bae922a6c8dafac4f022f2e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086850"
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
|bookmarkFolder|String|Папка, в которую должна быть добавлена закладка в Safari|
|displayName|String|Имя отображения закладки|

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



