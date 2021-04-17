---
title: тип ресурса teamsAppIcon
description: Значок, связанный с приложением в Microsoft Teams.
author: jecha
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3e8a256dc0b9e92c414cd3d362bb36579708083f
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882713"
---
# <a name="teamsappicon-resource-type"></a><span data-ttu-id="88eab-103">тип ресурса teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="88eab-103">teamsAppIcon resource type</span></span>

<span data-ttu-id="88eab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88eab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88eab-105">Значок, связанный с [teamsApp.](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="88eab-105">An icon associated with a [teamsApp](teamsapp.md).</span></span>

## <a name="methods"></a><span data-ttu-id="88eab-106">Методы</span><span class="sxs-lookup"><span data-stu-id="88eab-106">Methods</span></span>

| <span data-ttu-id="88eab-107">Метод</span><span class="sxs-lookup"><span data-stu-id="88eab-107">Method</span></span>                                            | <span data-ttu-id="88eab-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="88eab-108">Return Type</span></span>                                       | <span data-ttu-id="88eab-109">Описание</span><span class="sxs-lookup"><span data-stu-id="88eab-109">Description</span></span>                                                    | 
| :------------------------------------------------ | :------------------------------------------------ | :------------------------------------------------------------- |
| [<span data-ttu-id="88eab-110">Получить значок</span><span class="sxs-lookup"><span data-stu-id="88eab-110">Get icon</span></span>](../api/teamsappicon-get.md)     | [<span data-ttu-id="88eab-111">teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="88eab-111">teamsAppIcon</span></span>](teamsappicon.md)                   | <span data-ttu-id="88eab-112">Получите значок, связанный с определенной версией приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="88eab-112">Get an icon associated with a specific version of a Teams app.</span></span> |
| [<span data-ttu-id="88eab-113">Получить контент с хост-контентом</span><span class="sxs-lookup"><span data-stu-id="88eab-113">Get hosted content</span></span>](../api/teamworkhostedcontent-get.md) | [<span data-ttu-id="88eab-114">teamworkHostedContent</span><span class="sxs-lookup"><span data-stu-id="88eab-114">teamworkHostedContent</span></span>](teamworkhostedcontent.md) | <span data-ttu-id="88eab-115">Получите у себя содержимое (и его bytes) для значка.</span><span class="sxs-lookup"><span data-stu-id="88eab-115">Get hosted content (and its bytes) for an icon.</span></span>                |

## <a name="properties"></a><span data-ttu-id="88eab-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="88eab-116">Properties</span></span>

| <span data-ttu-id="88eab-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="88eab-117">Property</span></span>      | <span data-ttu-id="88eab-118">Тип</span><span class="sxs-lookup"><span data-stu-id="88eab-118">Type</span></span>                        | <span data-ttu-id="88eab-119">Описание</span><span class="sxs-lookup"><span data-stu-id="88eab-119">Description</span></span>                                                                             |
| :------------ | :-------------------------- | :-------------------------------------------------------------------------------------- |
| <span data-ttu-id="88eab-120">id</span><span class="sxs-lookup"><span data-stu-id="88eab-120">id</span></span>            | <span data-ttu-id="88eab-121">string</span><span class="sxs-lookup"><span data-stu-id="88eab-121">string</span></span>                      | <span data-ttu-id="88eab-122">Уникальный ID значка приложения.</span><span class="sxs-lookup"><span data-stu-id="88eab-122">The unique ID of the app icon.</span></span>                                                          |
| <span data-ttu-id="88eab-123">webUrl</span><span class="sxs-lookup"><span data-stu-id="88eab-123">webUrl</span></span>        | <span data-ttu-id="88eab-124">string</span><span class="sxs-lookup"><span data-stu-id="88eab-124">string</span></span>                      | <span data-ttu-id="88eab-125">Веб-URL-адрес, который можно использовать для скачивания изображения.</span><span class="sxs-lookup"><span data-stu-id="88eab-125">The web URL that can be used for downloading the image.</span></span>                                 |

## <a name="relationships"></a><span data-ttu-id="88eab-126">Связи</span><span class="sxs-lookup"><span data-stu-id="88eab-126">Relationships</span></span>

| <span data-ttu-id="88eab-127">Связь</span><span class="sxs-lookup"><span data-stu-id="88eab-127">Relationship</span></span>  | <span data-ttu-id="88eab-128">Тип</span><span class="sxs-lookup"><span data-stu-id="88eab-128">Type</span></span>                                              | <span data-ttu-id="88eab-129">Описание</span><span class="sxs-lookup"><span data-stu-id="88eab-129">Description</span></span>                                                                         |
| :------------ | :------------------------------------------------ | :---------------------------------------------------------------------------------- |
| <span data-ttu-id="88eab-130">hostedContent</span><span class="sxs-lookup"><span data-stu-id="88eab-130">hostedContent</span></span> | [<span data-ttu-id="88eab-131">teamworkHostedContent</span><span class="sxs-lookup"><span data-stu-id="88eab-131">teamworkHostedContent</span></span>](teamworkhostedcontent.md) | <span data-ttu-id="88eab-132">Содержимое значка приложения, если значок находится в инфраструктуре Teams.</span><span class="sxs-lookup"><span data-stu-id="88eab-132">The contents of the app icon if the icon is hosted within the Teams infrastructure.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="88eab-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="88eab-133">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppIcon",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "webUrl": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="88eab-134">См. также</span><span class="sxs-lookup"><span data-stu-id="88eab-134">See also</span></span>

- [<span data-ttu-id="88eab-135">teamsApp</span><span class="sxs-lookup"><span data-stu-id="88eab-135">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="88eab-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="88eab-136">teamsAppDefinition</span></span>](teamsappdefinition.md)
