---
title: тип ресурса macOSAssociatedDomainsItem
description: Сопоставление идентификаторов приложений с связанными доменами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2658a02a4881e793879a68bc6d1822d9a9b2a0a5
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819145"
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
|домены|Коллекция String|Список доменов, которые можно связать.|
|directDownloadsEnabled|Логический|Определяет, следует ли загружать данные напрямую или через CDN.|

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



