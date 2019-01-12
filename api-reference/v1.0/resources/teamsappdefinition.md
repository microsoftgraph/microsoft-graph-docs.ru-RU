---
title: Тип ресурса teamsAppDefinition
description: Подробные сведения о одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3aed533ecca3bff48071b04adadcea6b52169f89
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951931"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="7914e-103">Тип ресурса teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="7914e-103">teamsAppDefinition resource type</span></span>



<span data-ttu-id="7914e-104">Подробные сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="7914e-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7914e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7914e-105">Properties</span></span>

| <span data-ttu-id="7914e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7914e-106">Property</span></span>            | <span data-ttu-id="7914e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7914e-107">Type</span></span>     | <span data-ttu-id="7914e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7914e-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="7914e-109">id</span><span class="sxs-lookup"><span data-stu-id="7914e-109">id</span></span>                  | <span data-ttu-id="7914e-110">строка</span><span class="sxs-lookup"><span data-stu-id="7914e-110">string</span></span>   | <span data-ttu-id="7914e-111">Уникальный идентификатор (не appid команды).</span><span class="sxs-lookup"><span data-stu-id="7914e-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="7914e-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="7914e-112">teamsAppId</span></span>          | <span data-ttu-id="7914e-113">string</span><span class="sxs-lookup"><span data-stu-id="7914e-113">string</span></span>   | <span data-ttu-id="7914e-114">Идентификатор в манифесте приложения группы.</span><span class="sxs-lookup"><span data-stu-id="7914e-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="7914e-115">displayName</span><span class="sxs-lookup"><span data-stu-id="7914e-115">displayName</span></span>         | <span data-ttu-id="7914e-116">строка</span><span class="sxs-lookup"><span data-stu-id="7914e-116">string</span></span>   | <span data-ttu-id="7914e-117">Имя приложения, предоставляемый разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="7914e-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="7914e-118">version</span><span class="sxs-lookup"><span data-stu-id="7914e-118">version</span></span>             | <span data-ttu-id="7914e-119">string</span><span class="sxs-lookup"><span data-stu-id="7914e-119">string</span></span>   | <span data-ttu-id="7914e-120">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="7914e-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7914e-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7914e-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="7914e-122">См. также</span><span class="sxs-lookup"><span data-stu-id="7914e-122">See also</span></span>

- [<span data-ttu-id="7914e-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="7914e-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="7914e-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="7914e-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="7914e-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="7914e-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

