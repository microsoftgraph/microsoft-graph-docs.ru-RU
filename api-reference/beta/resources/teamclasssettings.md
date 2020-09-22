---
title: Тип ресурса Теамкласссеттингс
description: Представляет параметры, характерные для Teams типа Class.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 97a20a312f899db5334003edb1b739bdc3b9e346
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046673"
---
# <a name="teamclasssettings-resource-type"></a><span data-ttu-id="078d0-103">Тип ресурса Теамкласссеттингс</span><span class="sxs-lookup"><span data-stu-id="078d0-103">teamClassSettings resource type</span></span>

<span data-ttu-id="078d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="078d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="078d0-105">Представляет свойства [команды](team.md), зависящие от класса.</span><span class="sxs-lookup"><span data-stu-id="078d0-105">Represents class-specific properties of a [team](team.md).</span></span> <span data-ttu-id="078d0-106">Доступна только в том случае, если команда представляет класс.</span><span class="sxs-lookup"><span data-stu-id="078d0-106">Available only when the team represents a class.</span></span>

## <a name="properties"></a><span data-ttu-id="078d0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="078d0-107">Properties</span></span>
| <span data-ttu-id="078d0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="078d0-108">Property</span></span>     | <span data-ttu-id="078d0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="078d0-109">Type</span></span>   |<span data-ttu-id="078d0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="078d0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="078d0-111">нотифигуардиансабаутассигнментс</span><span class="sxs-lookup"><span data-stu-id="078d0-111">notifyGuardiansAboutAssignments</span></span>|<span data-ttu-id="078d0-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="078d0-112">Boolean</span></span>|<span data-ttu-id="078d0-113">Если задано значение `true` , разрешает отправку сообщений сводки по неделям в родительские и опекуны, если администратор клиента включил параметр глобально.</span><span class="sxs-lookup"><span data-stu-id="078d0-113">If set to `true`, enables sending of weekly assignments digest emails to parents/guardians, provided the tenant admin has enabled the setting globally.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="078d0-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="078d0-114">JSON representation</span></span>

<span data-ttu-id="078d0-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="078d0-115">The following is a JSON representation of the resource.</span></span>

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


