---
title: Тип ресурса Иосвебконтентфилтераутофилтер
description: Представляет тип параметра фильтра веб-содержимого iOS, который включает функцию автоматического фильтра iOS и предоставляет дополнительные возможности управления доступом по URL-АДРЕСу. При создании без значений свойств устройство iOS включит автоматический фильтр независимо.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb6bf2da4320c228123e24ae67bd21b13f2c21eb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946072"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>Тип ресурса Иосвебконтентфилтераутофилтер

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет тип параметра фильтра веб-содержимого iOS, который включает функцию автоматического фильтра iOS и предоставляет дополнительные возможности управления доступом по URL-АДРЕСу. При создании без значений свойств устройство iOS включит автоматический фильтр независимо.


Наследуется от [иосвебконтентфилтербасе](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Алловедурлс|Коллекция строк|Дополнительные URL-адреса, разрешенные для Access|
|Блоккедурлс|Коллекция строк|Дополнительные URL-адреса, заблокированные для Access|

## <a name="relationships"></a>Связи
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




