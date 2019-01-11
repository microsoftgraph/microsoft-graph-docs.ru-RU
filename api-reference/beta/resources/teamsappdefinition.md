---
title: Тип ресурса teamsAppDefinition
description: Подробные сведения о одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 8a13f6ffd4ca5385b9e264f8b8a5b8bddfe0a1fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851298"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="5f6c4-103">Тип ресурса teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="5f6c4-103">teamsAppDefinition resource type</span></span>

> <span data-ttu-id="5f6c4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5f6c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f6c4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f6c4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f6c4-106">Подробные сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="5f6c4-106">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5f6c4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f6c4-107">Properties</span></span>

| <span data-ttu-id="5f6c4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f6c4-108">Property</span></span>            | <span data-ttu-id="5f6c4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5f6c4-109">Type</span></span>     | <span data-ttu-id="5f6c4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5f6c4-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="5f6c4-111">id</span><span class="sxs-lookup"><span data-stu-id="5f6c4-111">id</span></span>                  | <span data-ttu-id="5f6c4-112">строка</span><span class="sxs-lookup"><span data-stu-id="5f6c4-112">string</span></span>   | <span data-ttu-id="5f6c4-113">Уникальный идентификатор (не appid команды).</span><span class="sxs-lookup"><span data-stu-id="5f6c4-113">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="5f6c4-114">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="5f6c4-114">teamsAppId</span></span>          | <span data-ttu-id="5f6c4-115">string</span><span class="sxs-lookup"><span data-stu-id="5f6c4-115">string</span></span>   | <span data-ttu-id="5f6c4-116">Идентификатор в манифесте приложения группы.</span><span class="sxs-lookup"><span data-stu-id="5f6c4-116">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="5f6c4-117">displayName</span><span class="sxs-lookup"><span data-stu-id="5f6c4-117">displayName</span></span>         | <span data-ttu-id="5f6c4-118">строка</span><span class="sxs-lookup"><span data-stu-id="5f6c4-118">string</span></span>   | <span data-ttu-id="5f6c4-119">Имя приложения, предоставляемый разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="5f6c4-119">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="5f6c4-120">version</span><span class="sxs-lookup"><span data-stu-id="5f6c4-120">version</span></span>             | <span data-ttu-id="5f6c4-121">string</span><span class="sxs-lookup"><span data-stu-id="5f6c4-121">string</span></span>   | <span data-ttu-id="5f6c4-122">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="5f6c4-122">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5f6c4-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f6c4-123">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "Test App",
  "version": "1.0.0",
}
```

# <a name="see-also"></a><span data-ttu-id="5f6c4-124">См. также</span><span class="sxs-lookup"><span data-stu-id="5f6c4-124">See also</span></span>

- [<span data-ttu-id="5f6c4-125">teamsApp</span><span class="sxs-lookup"><span data-stu-id="5f6c4-125">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="5f6c4-126">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="5f6c4-126">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="5f6c4-127">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5f6c4-127">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

