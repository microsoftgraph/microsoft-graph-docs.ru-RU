---
title: тип ресурса teamworkUserIdentity
description: Представляет пользователя в Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7ae7655a5b2c84cc01d354d32d25eb724d5f4a6c
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211131"
---
# <a name="teamworkuseridentity-resource-type"></a><span data-ttu-id="c7b16-103">тип ресурса teamworkUserIdentity</span><span class="sxs-lookup"><span data-stu-id="c7b16-103">teamworkUserIdentity resource type</span></span>

<span data-ttu-id="c7b16-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7b16-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7b16-105">Представляет пользователя **в** Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c7b16-105">Represents a **user** in Microsoft Teams.</span></span>


<span data-ttu-id="c7b16-106">Наследует от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="c7b16-106">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c7b16-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7b16-107">Properties</span></span>
|<span data-ttu-id="c7b16-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7b16-108">Property</span></span>|<span data-ttu-id="c7b16-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c7b16-109">Type</span></span>|<span data-ttu-id="c7b16-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c7b16-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7b16-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c7b16-111">displayName</span></span>|<span data-ttu-id="c7b16-112">String</span><span class="sxs-lookup"><span data-stu-id="c7b16-112">String</span></span>|<span data-ttu-id="c7b16-113">Унаследованный от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="c7b16-113">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="c7b16-114">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="c7b16-114">Display name of the user.</span></span> <span data-ttu-id="c7b16-115">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c7b16-115">Optional.</span></span>|
|<span data-ttu-id="c7b16-116">id</span><span class="sxs-lookup"><span data-stu-id="c7b16-116">id</span></span>|<span data-ttu-id="c7b16-117">String</span><span class="sxs-lookup"><span data-stu-id="c7b16-117">String</span></span>|<span data-ttu-id="c7b16-118">Унаследованный от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="c7b16-118">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="c7b16-119">ID пользователя.</span><span class="sxs-lookup"><span data-stu-id="c7b16-119">ID of the user.</span></span> |
|<span data-ttu-id="c7b16-120">userIdentityType</span><span class="sxs-lookup"><span data-stu-id="c7b16-120">userIdentityType</span></span>|<span data-ttu-id="c7b16-121">teamworkUserIdentityType</span><span class="sxs-lookup"><span data-stu-id="c7b16-121">teamworkUserIdentityType</span></span>| <span data-ttu-id="c7b16-122">Тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="c7b16-122">Type of user.</span></span> <span data-ttu-id="c7b16-123">Возможные значения: `aadUser` `onPremiseAadUser` , , , , , `anonymousGuest` , `federatedUser` и `personalMicrosoftAccountUser` `skypeUser` `phoneUser` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="c7b16-123">Possible values are: `aadUser`, `onPremiseAadUser`, `anonymousGuest`, `federatedUser`, `personalMicrosoftAccountUser`, `skypeUser`, `phoneUser`, and `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7b16-124">Связи</span><span class="sxs-lookup"><span data-stu-id="c7b16-124">Relationships</span></span>
<span data-ttu-id="c7b16-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c7b16-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7b16-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c7b16-126">JSON representation</span></span>
<span data-ttu-id="c7b16-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7b16-127">The following is a JSON representation of the resource.</span></span>
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

