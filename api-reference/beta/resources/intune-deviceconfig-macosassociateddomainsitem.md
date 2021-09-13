---
title: тип ресурса macOSAssociatedDomainsItem
description: Сопоставление идентификаторов приложений с связанными доменами.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e1229706d524cb16c9c66c1acf4c7fb86e65ede0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081327"
---
# <a name="macosassociateddomainsitem-resource-type"></a>тип ресурса macOSAssociatedDomainsItem

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сопоставление идентификаторов приложений с связанными доменами.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|applicationIdentifier|String|Идентификатор приложения для связывать домены с.|
|домены|Коллекция объектов string|Список доменов, которые можно связать.|
|directDownloadsEnabled|Boolean|Определяет, следует ли загружать данные напрямую или через CDN.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAssociatedDomainsItem",
  "applicationIdentifier": "String",
  "domains": [
    "String"
  ],
  "directDownloadsEnabled": true
}
```



