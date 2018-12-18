---
title: Тип ресурса teamsAppDefinition
description: Подробные сведения о одной версии teamsApp.
author: nkramer
ms.openlocfilehash: 43bd4262008a29668739e78d4b598da1e77e3d4b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351641"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="5fb36-103">Тип ресурса teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="5fb36-103">teamsAppDefinition resource type</span></span>



<span data-ttu-id="5fb36-104">Подробные сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="5fb36-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5fb36-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5fb36-105">Properties</span></span>

| <span data-ttu-id="5fb36-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5fb36-106">Property</span></span>            | <span data-ttu-id="5fb36-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5fb36-107">Type</span></span>     | <span data-ttu-id="5fb36-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5fb36-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="5fb36-109">id</span><span class="sxs-lookup"><span data-stu-id="5fb36-109">id</span></span>                  | <span data-ttu-id="5fb36-110">строка</span><span class="sxs-lookup"><span data-stu-id="5fb36-110">string</span></span>   | <span data-ttu-id="5fb36-111">Уникальный идентификатор (не appid команды).</span><span class="sxs-lookup"><span data-stu-id="5fb36-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="5fb36-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="5fb36-112">teamsAppId</span></span>          | <span data-ttu-id="5fb36-113">string</span><span class="sxs-lookup"><span data-stu-id="5fb36-113">string</span></span>   | <span data-ttu-id="5fb36-114">Идентификатор в манифесте приложения группы.</span><span class="sxs-lookup"><span data-stu-id="5fb36-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="5fb36-115">displayName</span><span class="sxs-lookup"><span data-stu-id="5fb36-115">displayName</span></span>         | <span data-ttu-id="5fb36-116">строка</span><span class="sxs-lookup"><span data-stu-id="5fb36-116">string</span></span>   | <span data-ttu-id="5fb36-117">Имя приложения, предоставляемый разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="5fb36-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="5fb36-118">version</span><span class="sxs-lookup"><span data-stu-id="5fb36-118">version</span></span>             | <span data-ttu-id="5fb36-119">string</span><span class="sxs-lookup"><span data-stu-id="5fb36-119">string</span></span>   | <span data-ttu-id="5fb36-120">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="5fb36-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5fb36-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5fb36-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="5fb36-122">См. также</span><span class="sxs-lookup"><span data-stu-id="5fb36-122">See also</span></span>

- [<span data-ttu-id="5fb36-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="5fb36-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="5fb36-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="5fb36-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="5fb36-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5fb36-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

