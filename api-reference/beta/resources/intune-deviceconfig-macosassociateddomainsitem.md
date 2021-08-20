---
title: тип ресурса macOSAssociatedDomainsItem
description: Сопоставление идентификаторов приложений с связанными доменами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff607e0eb88a53aa53500b278e7cbf90da49a34fa4033a3907f24818c3618ddc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54183129"
---
# <a name="macosassociateddomainsitem-resource-type"></a>тип ресурса macOSAssociatedDomainsItem

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сопоставление идентификаторов приложений с связанными доменами.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|applicationIdentifier|Строка|Идентификатор приложения для связывать домены с.|
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




