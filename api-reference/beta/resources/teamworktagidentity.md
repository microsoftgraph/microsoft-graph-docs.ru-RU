---
title: тип ресурса teamworkTagIdentity
description: Представляет тег в Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c0f6a8876533b2add5b63615095113f5485bfbca
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211427"
---
# <a name="teamworktagidentity-resource-type"></a>тип ресурса teamworkTagIdentity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тег **в** Microsoft Teams. Теги позволяют пользователям быстро подключаться к подмножество пользователей в команде. Сведения об управлении тегами в Microsoft Teams см. в материале Управление тегами [в Microsoft Teams.](/microsoftteams/manage-tags)


Наследует от [удостоверения](../resources/identity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Унаследованный от [удостоверения](../resources/identity.md). Отображение имени тега.|
|id|String|Унаследованный от [удостоверения](../resources/identity.md). ID тега.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkTagIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTagIdentity",
  "id": "String (identifier)",
  "displayName": "String"
}
```

