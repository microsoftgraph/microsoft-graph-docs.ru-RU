---
title: Тип ресурса Теамкласссеттингс
description: Представляет параметры, характерные для Teams типа Class.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 312acf937fdb90940a640d35c6a19c88981e842c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533551"
---
# <a name="teamclasssettings-resource-type"></a><span data-ttu-id="a2df5-103">Тип ресурса Теамкласссеттингс</span><span class="sxs-lookup"><span data-stu-id="a2df5-103">teamClassSettings resource type</span></span>

<span data-ttu-id="a2df5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2df5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a2df5-105">Представляет свойства [команды](team.md), зависящие от класса.</span><span class="sxs-lookup"><span data-stu-id="a2df5-105">Represents class-specific properties of a [team](team.md).</span></span> <span data-ttu-id="a2df5-106">Доступна только в том случае, если команда представляет класс.</span><span class="sxs-lookup"><span data-stu-id="a2df5-106">Available only when the team represents a class.</span></span>

## <a name="properties"></a><span data-ttu-id="a2df5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2df5-107">Properties</span></span>
| <span data-ttu-id="a2df5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2df5-108">Property</span></span>     | <span data-ttu-id="a2df5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a2df5-109">Type</span></span>   |<span data-ttu-id="a2df5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a2df5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2df5-111">нотифигуардиансабаутассигнментс</span><span class="sxs-lookup"><span data-stu-id="a2df5-111">notifyGuardiansAboutAssignments</span></span>|<span data-ttu-id="a2df5-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2df5-112">Boolean</span></span>|<span data-ttu-id="a2df5-113">Если задано `true`значение, разрешает отправку сообщений сводки по неделям в родительские и опекуны, если администратор клиента включил параметр глобально.</span><span class="sxs-lookup"><span data-stu-id="a2df5-113">If set to `true`, enables sending of weekly assignments digest emails to parents/guardians, provided the tenant admin has enabled the setting globally.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2df5-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2df5-114">JSON representation</span></span>

<span data-ttu-id="a2df5-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2df5-115">The following is a JSON representation of the resource.</span></span>

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
