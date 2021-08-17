---
title: тип ресурса iosWebContentFilterAutoFilter
description: Представляет тип параметра фильтра веб-контента iOS, который включает функцию автоматического фильтра iOS и позволяет дополнительно управлять доступом к URL-адресу. При построении без значений свойств устройство iOS включит автоматический фильтр независимо.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9d09b964b02b5bc329fca67662d9a46a69c67740732d068c7bd918e4b37aff3a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206657"
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




