---
title: Тип ресурса Теамкласссеттингс
description: Представляет параметры, характерные для Teams типа Class.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca8d345cd229c4a6c003c87865b5aaddf01096b4
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998618"
---
# <a name="teamclasssettings-resource-type"></a><span data-ttu-id="051c3-103">Тип ресурса Теамкласссеттингс</span><span class="sxs-lookup"><span data-stu-id="051c3-103">teamClassSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="051c3-104">Представляет свойства [команды](team.md), зависящие от класса.</span><span class="sxs-lookup"><span data-stu-id="051c3-104">Represents class-specific properties of a [team](team.md).</span></span> <span data-ttu-id="051c3-105">Доступно только в том случае, если команда представляет класс.</span><span class="sxs-lookup"><span data-stu-id="051c3-105">Available only when the team represents a class.</span></span>

## <a name="properties"></a><span data-ttu-id="051c3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="051c3-106">Properties</span></span>
| <span data-ttu-id="051c3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="051c3-107">Property</span></span>     | <span data-ttu-id="051c3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="051c3-108">Type</span></span>   |<span data-ttu-id="051c3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="051c3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="051c3-110">нотифигуардиансабаутассигнментс</span><span class="sxs-lookup"><span data-stu-id="051c3-110">notifyGuardiansAboutAssignments</span></span>|<span data-ttu-id="051c3-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="051c3-111">Boolean</span></span>|<span data-ttu-id="051c3-112">Если задано `true`значение, разрешает отправку сообщений сводки по неделям в родительские и опекуны, если администратор клиента включил параметр глобально.</span><span class="sxs-lookup"><span data-stu-id="051c3-112">If set to `true`, enables sending of weekly assignments digest emails to parents/guardians, provided the tenant admin has enabled the setting globally.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="051c3-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="051c3-113">JSON representation</span></span>

<span data-ttu-id="051c3-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="051c3-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamClassSettings"
}-->

```json
{
  "notifyGuardiansAboutAssignments": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's classSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
