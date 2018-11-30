---
title: Тип ресурса teamsAppDefinition
description: Подробные сведения о одной версии teamsApp.
ms.openlocfilehash: b2a5b86de67fa1a4ecf673434b13d09c64ebe678
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081355"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="a5deb-103">Тип ресурса teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a5deb-103">teamsAppDefinition resource type</span></span>

> <span data-ttu-id="a5deb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a5deb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5deb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5deb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5deb-106">Подробные сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="a5deb-106">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a5deb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5deb-107">Properties</span></span>

| <span data-ttu-id="a5deb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5deb-108">Property</span></span>            | <span data-ttu-id="a5deb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a5deb-109">Type</span></span>     | <span data-ttu-id="a5deb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a5deb-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="a5deb-111">id</span><span class="sxs-lookup"><span data-stu-id="a5deb-111">id</span></span>                  | <span data-ttu-id="a5deb-112">строка</span><span class="sxs-lookup"><span data-stu-id="a5deb-112">string</span></span>   | <span data-ttu-id="a5deb-113">Уникальный идентификатор (не appid команды).</span><span class="sxs-lookup"><span data-stu-id="a5deb-113">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="a5deb-114">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="a5deb-114">teamsAppId</span></span>          | <span data-ttu-id="a5deb-115">string</span><span class="sxs-lookup"><span data-stu-id="a5deb-115">string</span></span>   | <span data-ttu-id="a5deb-116">Идентификатор в манифесте приложения группы.</span><span class="sxs-lookup"><span data-stu-id="a5deb-116">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="a5deb-117">displayName</span><span class="sxs-lookup"><span data-stu-id="a5deb-117">displayName</span></span>         | <span data-ttu-id="a5deb-118">строка</span><span class="sxs-lookup"><span data-stu-id="a5deb-118">string</span></span>   | <span data-ttu-id="a5deb-119">Имя приложения, предоставляемый разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="a5deb-119">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="a5deb-120">version</span><span class="sxs-lookup"><span data-stu-id="a5deb-120">version</span></span>             | <span data-ttu-id="a5deb-121">string</span><span class="sxs-lookup"><span data-stu-id="a5deb-121">string</span></span>   | <span data-ttu-id="a5deb-122">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="a5deb-122">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a5deb-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5deb-123">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="a5deb-124">См. также</span><span class="sxs-lookup"><span data-stu-id="a5deb-124">See also</span></span>

- [<span data-ttu-id="a5deb-125">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a5deb-125">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="a5deb-126">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a5deb-126">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="a5deb-127">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a5deb-127">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

