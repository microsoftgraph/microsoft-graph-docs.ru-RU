---
title: Тип ресурса subjectRightsRequestEnumeratedMailboxLocation
description: Представляет свойства запроса прав субъекта, который определяет определенные почтовые ящики (Exchange почтовые ящики и отдельные или групповые Microsoft Teams чата) в качестве расположения поиска.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 1edae24833a7e003fa1a498ca3642508e38af6fa
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461767"
---
# <a name="subjectrightsrequestenumeratedmailboxlocation-resource-type"></a>Тип ресурса subjectRightsRequestEnumeratedMailboxLocation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет свойства запроса прав субъекта, который определяет определенные почтовые ящики (Exchange почтовые ящики и отдельные или групповые Microsoft Teams чата) в качестве расположения поиска.

Наследуется [от subjectRightsRequestMailboxLocation](../resources/subjectrightsrequestmailboxlocation.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|upns|Коллекция String|Коллекция почтовых ящиков, которые должны быть включены в поиск. Включает имя участника-пользователя (имя участника-пользователя) каждого почтового ящика, например `Monica.Thompson@contoso.com`.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectRightsRequestEnumeratedMailboxLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectRightsRequestEnumeratedMailboxLocation",
  "upns": [
    "String"
  ]
}
```

