---
title: Тип ресурса teamsAppDefinition
description: Подробные сведения о одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 8fafb266b2bfc2c7ea6e0951ac2906f133817246
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860979"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="5e218-103">Тип ресурса teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="5e218-103">teamsAppDefinition resource type</span></span>



<span data-ttu-id="5e218-104">Подробные сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="5e218-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5e218-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e218-105">Properties</span></span>

| <span data-ttu-id="5e218-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e218-106">Property</span></span>            | <span data-ttu-id="5e218-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5e218-107">Type</span></span>     | <span data-ttu-id="5e218-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5e218-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="5e218-109">id</span><span class="sxs-lookup"><span data-stu-id="5e218-109">id</span></span>                  | <span data-ttu-id="5e218-110">строка</span><span class="sxs-lookup"><span data-stu-id="5e218-110">string</span></span>   | <span data-ttu-id="5e218-111">Уникальный идентификатор (не appid команды).</span><span class="sxs-lookup"><span data-stu-id="5e218-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="5e218-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="5e218-112">teamsAppId</span></span>          | <span data-ttu-id="5e218-113">string</span><span class="sxs-lookup"><span data-stu-id="5e218-113">string</span></span>   | <span data-ttu-id="5e218-114">Идентификатор в манифесте приложения группы.</span><span class="sxs-lookup"><span data-stu-id="5e218-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="5e218-115">displayName</span><span class="sxs-lookup"><span data-stu-id="5e218-115">displayName</span></span>         | <span data-ttu-id="5e218-116">строка</span><span class="sxs-lookup"><span data-stu-id="5e218-116">string</span></span>   | <span data-ttu-id="5e218-117">Имя приложения, предоставляемый разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="5e218-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="5e218-118">version</span><span class="sxs-lookup"><span data-stu-id="5e218-118">version</span></span>             | <span data-ttu-id="5e218-119">string</span><span class="sxs-lookup"><span data-stu-id="5e218-119">string</span></span>   | <span data-ttu-id="5e218-120">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="5e218-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5e218-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e218-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="5e218-122">См. также</span><span class="sxs-lookup"><span data-stu-id="5e218-122">See also</span></span>

- [<span data-ttu-id="5e218-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="5e218-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="5e218-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="5e218-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="5e218-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5e218-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

