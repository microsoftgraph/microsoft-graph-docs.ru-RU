---
title: тип ресурса iosWebContentFilterAutoFilter
description: Представляет тип параметра фильтра веб-контента iOS, который включает функцию автоматического фильтра iOS и позволяет дополнительно управлять доступом к URL-адресу. При построении без значений свойств устройство iOS включит автоматический фильтр независимо.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0cbd15f366397564b24f6c715eaf2ea9b6826d30
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58813007"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>тип ресурса iosWebContentFilterAutoFilter

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет тип параметра фильтра веб-контента iOS, который включает функцию автоматического фильтра iOS и позволяет дополнительно управлять доступом к URL-адресу. При построении без значений свойств устройство iOS включит автоматический фильтр независимо.


Наследует [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedUrls|Коллекция String|Дополнительные URL-адреса, разрешенные для доступа|
|blockedUrls|Коллекция String|Дополнительные URL-адреса, заблокированные для доступа|

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



