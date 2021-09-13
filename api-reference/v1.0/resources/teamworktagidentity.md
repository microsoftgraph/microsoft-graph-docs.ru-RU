---
title: тип ресурса teamworkTagIdentity
description: Представляет тег в Microsoft Teams.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7cd605a42f0f0c7f697c7b291fe30645bdf4403b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128174"
---
# <a name="teamworktagidentity-resource-type"></a>тип ресурса teamworkTagIdentity

Пространство имен: microsoft.graph

Представляет тег **в** Microsoft Teams. Теги позволяют пользователям быстро подключаться к подмножество пользователей в команде. Сведения об управлении тегами в Microsoft Teams см. в материале Управление тегами [в Microsoft Teams.](/microsoftteams/manage-tags)


Наследует от [удостоверения](../resources/identity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Унаследованный от [удостоверения](../resources/identity.md). Отображение имени тега.|
|id|String|Унаследованный от [удостоверения](../resources/identity.md). ID тега.|

## <a name="relationships"></a>Отношения
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

