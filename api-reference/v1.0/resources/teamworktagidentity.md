---
title: тип ресурса teamworkTagIdentity
description: Представляет тег в Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2f507844751b92493eab2c4bb84f2da2f3a04c8afb310b682ac9beb2f025031f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129941"
---
# <a name="teamworktagidentity-resource-type"></a>тип ресурса teamworkTagIdentity

Пространство имен: microsoft.graph

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

