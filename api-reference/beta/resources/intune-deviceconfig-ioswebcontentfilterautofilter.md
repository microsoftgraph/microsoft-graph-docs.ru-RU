---
title: Тип ресурса iosWebContentFilterAutoFilter
description: Представляет операций ввода-вывода тип параметра фильтра веб-содержимого, который позволяет функция автоматического фильтра операций ввода-вывода и для управления доступом к дополнительные URL-адреса. При создании без значения свойства устройства iOS позволит автоматического фильтра вне зависимости от.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d5be275b74e2675881b9d36b047e2017ef95adb2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401231"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>Тип ресурса iosWebContentFilterAutoFilter

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет операций ввода-вывода тип параметра фильтра веб-содержимого, который позволяет функция автоматического фильтра операций ввода-вывода и для управления доступом к дополнительные URL-адреса. При создании без значения свойства устройства iOS позволит автоматического фильтра вне зависимости от.


Наследуется от [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedUrls|Коллекция String|Дополнительные URL-адреса, разрешенных для access|
|blockedUrls|Коллекция String|Дополнительные URL-адреса, заблокированные для access|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterAutoFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterAutoFilter",
  "allowedUrls": [
    "String"
  ],
  "blockedUrls": [
    "String"
  ]
}
```




