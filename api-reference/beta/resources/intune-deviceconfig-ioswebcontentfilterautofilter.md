---
title: Тип ресурса Иосвебконтентфилтераутофилтер
description: Представляет тип параметра фильтра веб-содержимого iOS, который включает функцию автоматического фильтра iOS и предоставляет дополнительные возможности управления доступом по URL-адресу. При создании без значений свойств устройство iOS включит автоматический фильтр независимо.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b3bcf8c66aff4220b7e2b394819beb35255bfba3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529821"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>Тип ресурса Иосвебконтентфилтераутофилтер

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет тип параметра фильтра веб-содержимого iOS, который включает функцию автоматического фильтра iOS и предоставляет дополнительные возможности управления доступом по URL-адресу. При создании без значений свойств устройство iOS включит автоматический фильтр независимо.


Наследуется от [иосвебконтентфилтербасе](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедурлс|Коллекция String|Дополнительные URL-адреса, разрешенные для Access|
|блоккедурлс|Коллекция String|Дополнительные URL-адреса, заблокированные для Access|

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



