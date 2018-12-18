---
title: Тип ресурса teamsAppDefinition
description: Подробные сведения о одной версии teamsApp.
author: nkramer
ms.openlocfilehash: 71a1783131661aed120f375f7cc58d55fb0ca0d2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336836"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="42354-103">Тип ресурса teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="42354-103">teamsAppDefinition resource type</span></span>

> <span data-ttu-id="42354-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="42354-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42354-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42354-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42354-106">Подробные сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="42354-106">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="42354-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="42354-107">Properties</span></span>

| <span data-ttu-id="42354-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="42354-108">Property</span></span>            | <span data-ttu-id="42354-109">Тип</span><span class="sxs-lookup"><span data-stu-id="42354-109">Type</span></span>     | <span data-ttu-id="42354-110">Описание</span><span class="sxs-lookup"><span data-stu-id="42354-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="42354-111">id</span><span class="sxs-lookup"><span data-stu-id="42354-111">id</span></span>                  | <span data-ttu-id="42354-112">строка</span><span class="sxs-lookup"><span data-stu-id="42354-112">string</span></span>   | <span data-ttu-id="42354-113">Уникальный идентификатор (не appid команды).</span><span class="sxs-lookup"><span data-stu-id="42354-113">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="42354-114">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="42354-114">teamsAppId</span></span>          | <span data-ttu-id="42354-115">string</span><span class="sxs-lookup"><span data-stu-id="42354-115">string</span></span>   | <span data-ttu-id="42354-116">Идентификатор в манифесте приложения группы.</span><span class="sxs-lookup"><span data-stu-id="42354-116">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="42354-117">displayName</span><span class="sxs-lookup"><span data-stu-id="42354-117">displayName</span></span>         | <span data-ttu-id="42354-118">строка</span><span class="sxs-lookup"><span data-stu-id="42354-118">string</span></span>   | <span data-ttu-id="42354-119">Имя приложения, предоставляемый разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="42354-119">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="42354-120">version</span><span class="sxs-lookup"><span data-stu-id="42354-120">version</span></span>             | <span data-ttu-id="42354-121">string</span><span class="sxs-lookup"><span data-stu-id="42354-121">string</span></span>   | <span data-ttu-id="42354-122">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="42354-122">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="42354-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42354-123">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="42354-124">См. также</span><span class="sxs-lookup"><span data-stu-id="42354-124">See also</span></span>

- [<span data-ttu-id="42354-125">teamsApp</span><span class="sxs-lookup"><span data-stu-id="42354-125">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="42354-126">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="42354-126">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="42354-127">teamsTab</span><span class="sxs-lookup"><span data-stu-id="42354-127">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

