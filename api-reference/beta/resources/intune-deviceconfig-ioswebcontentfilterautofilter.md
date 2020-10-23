---
title: Тип ресурса Иосвебконтентфилтераутофилтер
description: Представляет тип параметра фильтра веб-содержимого iOS, который включает функцию автоматического фильтра iOS и предоставляет дополнительные возможности управления доступом по URL-адресу. При создании без значений свойств устройство iOS включит автоматический фильтр независимо.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4db3b5c04b4cbac46e04ce097ec12ed979ed9ee2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702497"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>Тип ресурса Иосвебконтентфилтераутофилтер

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет тип параметра фильтра веб-содержимого iOS, который включает функцию автоматического фильтра iOS и предоставляет дополнительные возможности управления доступом по URL-адресу. При создании без значений свойств устройство iOS включит автоматический фильтр независимо.


Наследуется от [иосвебконтентфилтербасе](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедурлс|Коллекция строк|Дополнительные URL-адреса, разрешенные для Access|
|блоккедурлс|Коллекция строк|Дополнительные URL-адреса, заблокированные для Access|

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





