---
title: Тип ресурса Иосбукмарк
description: Закладка URL-адреса iOS
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c8a4ff93674f9fedbed0597fb8e418a59b9ea70
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946562"
---
# <a name="iosbookmark-resource-type"></a>Тип ресурса Иосбукмарк

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Закладка URL-адреса iOS

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|url|String|URL-адрес, разрешенный для доступа|
|Букмаркфолдер|Строка|Папка, в которую следует добавить закладку в Safari|
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




