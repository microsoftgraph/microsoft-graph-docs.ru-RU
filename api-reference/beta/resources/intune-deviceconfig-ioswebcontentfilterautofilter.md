---
title: тип ресурса iosWebContentFilterAutoFilter
description: Представляет тип параметра фильтра веб-контента iOS, который включает функцию автоматического фильтра iOS и позволяет дополнительно управлять доступом к URL-адресу. При построении без значений свойств устройство iOS включит автоматический фильтр независимо.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4c88850a9cb9cfab27da02231a908ed9466b6389
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127236"
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
|allowedUrls|Коллекция объектов string|Дополнительные URL-адреса, разрешенные для доступа|
|blockedUrls|Коллекция объектов string|Дополнительные URL-адреса, заблокированные для доступа|

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



