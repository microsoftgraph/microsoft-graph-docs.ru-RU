---
title: тип ресурса teamworkTagIdentity
description: Представляет тег в Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b9ea11746a98fba8bb209112c1cb6b1ed63fc954
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211136"
---
# <a name="teamworktagidentity-resource-type"></a><span data-ttu-id="fe63f-103">тип ресурса teamworkTagIdentity</span><span class="sxs-lookup"><span data-stu-id="fe63f-103">teamworkTagIdentity resource type</span></span>

<span data-ttu-id="fe63f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe63f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe63f-105">Представляет тег **в** Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="fe63f-105">Represents a **tag** in Microsoft Teams.</span></span> <span data-ttu-id="fe63f-106">Теги позволяют пользователям быстро подключаться к подмножество пользователей в команде.</span><span class="sxs-lookup"><span data-stu-id="fe63f-106">Tags allow users to quickly connect to subset of users in a team.</span></span> <span data-ttu-id="fe63f-107">Сведения об управлении тегами в Microsoft Teams см. в материале Управление тегами [в Microsoft Teams.](/microsoftteams/manage-tags)</span><span class="sxs-lookup"><span data-stu-id="fe63f-107">For details about tag management in Microsoft Teams, see [Manage tags in Microsoft Teams](/microsoftteams/manage-tags).</span></span>


<span data-ttu-id="fe63f-108">Наследует от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="fe63f-108">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fe63f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe63f-109">Properties</span></span>
|<span data-ttu-id="fe63f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe63f-110">Property</span></span>|<span data-ttu-id="fe63f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fe63f-111">Type</span></span>|<span data-ttu-id="fe63f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fe63f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe63f-113">displayName</span><span class="sxs-lookup"><span data-stu-id="fe63f-113">displayName</span></span>|<span data-ttu-id="fe63f-114">String</span><span class="sxs-lookup"><span data-stu-id="fe63f-114">String</span></span>|<span data-ttu-id="fe63f-115">Унаследованный от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="fe63f-115">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="fe63f-116">Отображение имени тега.</span><span class="sxs-lookup"><span data-stu-id="fe63f-116">Display name of the tag.</span></span>|
|<span data-ttu-id="fe63f-117">id</span><span class="sxs-lookup"><span data-stu-id="fe63f-117">id</span></span>|<span data-ttu-id="fe63f-118">String</span><span class="sxs-lookup"><span data-stu-id="fe63f-118">String</span></span>|<span data-ttu-id="fe63f-119">Унаследованный от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="fe63f-119">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="fe63f-120">ID тега.</span><span class="sxs-lookup"><span data-stu-id="fe63f-120">ID of the tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe63f-121">Связи</span><span class="sxs-lookup"><span data-stu-id="fe63f-121">Relationships</span></span>
<span data-ttu-id="fe63f-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fe63f-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe63f-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fe63f-123">JSON representation</span></span>
<span data-ttu-id="fe63f-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe63f-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkTagIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTagIdentity",
  "id": "String (identifier)",
  "displayName": "String"
}
```

