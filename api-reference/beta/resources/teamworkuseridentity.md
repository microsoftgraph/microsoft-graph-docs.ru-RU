---
title: тип ресурса teamworkUserIdentity
description: Представляет пользователя в Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b0c50856a2b7051a631cd14ab3985cd8724bfe4c
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211433"
---
# <a name="teamworkuseridentity-resource-type"></a><span data-ttu-id="b615b-103">тип ресурса teamworkUserIdentity</span><span class="sxs-lookup"><span data-stu-id="b615b-103">teamworkUserIdentity resource type</span></span>

<span data-ttu-id="b615b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b615b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b615b-105">Представляет пользователя **в** Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b615b-105">Represents a **user** in Microsoft Teams.</span></span>


<span data-ttu-id="b615b-106">Наследует от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="b615b-106">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b615b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b615b-107">Properties</span></span>
|<span data-ttu-id="b615b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b615b-108">Property</span></span>|<span data-ttu-id="b615b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b615b-109">Type</span></span>|<span data-ttu-id="b615b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b615b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b615b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b615b-111">displayName</span></span>|<span data-ttu-id="b615b-112">String</span><span class="sxs-lookup"><span data-stu-id="b615b-112">String</span></span>|<span data-ttu-id="b615b-113">Унаследованный от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="b615b-113">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="b615b-114">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="b615b-114">Display name of the user.</span></span> <span data-ttu-id="b615b-115">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="b615b-115">Optional.</span></span>|
|<span data-ttu-id="b615b-116">id</span><span class="sxs-lookup"><span data-stu-id="b615b-116">id</span></span>|<span data-ttu-id="b615b-117">String</span><span class="sxs-lookup"><span data-stu-id="b615b-117">String</span></span>|<span data-ttu-id="b615b-118">Унаследованный от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="b615b-118">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="b615b-119">ID пользователя.</span><span class="sxs-lookup"><span data-stu-id="b615b-119">ID of the user.</span></span> |
|<span data-ttu-id="b615b-120">userIdentityType</span><span class="sxs-lookup"><span data-stu-id="b615b-120">userIdentityType</span></span>|<span data-ttu-id="b615b-121">teamworkUserIdentityType</span><span class="sxs-lookup"><span data-stu-id="b615b-121">teamworkUserIdentityType</span></span>| <span data-ttu-id="b615b-122">Тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="b615b-122">Type of user.</span></span> <span data-ttu-id="b615b-123">Возможные значения: `aadUser` `onPremiseAadUser` , , , , , `anonymousGuest` , `federatedUser` и `personalMicrosoftAccountUser` `skypeUser` `phoneUser` .</span><span class="sxs-lookup"><span data-stu-id="b615b-123">Possible values are: `aadUser`, `onPremiseAadUser`, `anonymousGuest`, `federatedUser`, `personalMicrosoftAccountUser`, `skypeUser`, and `phoneUser`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b615b-124">Связи</span><span class="sxs-lookup"><span data-stu-id="b615b-124">Relationships</span></span>
<span data-ttu-id="b615b-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b615b-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b615b-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b615b-126">JSON representation</span></span>
<span data-ttu-id="b615b-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b615b-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkUserIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkUserIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "userIdentityType": "String"
}
```

