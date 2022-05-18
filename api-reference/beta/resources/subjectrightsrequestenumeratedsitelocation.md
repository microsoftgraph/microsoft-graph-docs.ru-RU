---
title: Тип ресурса subjectRightsRequestEnumeratedSiteLocation
description: Представляет свойства запроса прав субъекта, который определяет определенные сайты (сайты SharePoint, OneDrive для бизнеса сайты и Microsoft Teams каналы) в качестве расположения поиска.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: b7b8752fb51da3eaaa9762de7b38cf080559a5e4
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461806"
---
# <a name="subjectrightsrequestenumeratedsitelocation-resource-type"></a>Тип ресурса subjectRightsRequestEnumeratedSiteLocation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет свойства запроса прав субъекта, который определяет определенные сайты (сайты SharePoint, OneDrive для бизнеса сайты и Microsoft Teams каналы) в качестве расположения поиска.

Наследуется [от subjectRightsRequestSiteLocation](../resources/subjectrightsrequestsitelocation.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Url|Коллекция String|Коллекция URL-адресов сайтов, которые должны быть включены. Включает, например, URL-адрес каждого сайта `https://www.contoso.com/site1`.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectRightsRequestEnumeratedSiteLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectRightsRequestEnumeratedSiteLocation",
  "urls": [
    "String"
  ]
}
```

