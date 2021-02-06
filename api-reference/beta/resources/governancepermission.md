---
title: Тип ресурса governancePermission
description: 'Представляет разрешение на доступ, которое имеется у governanceSubject к определенному governanceResource.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: f316a863ecba9ed546b9ba4045e57ada87e97ab9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128847"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="b98c8-103">Тип ресурса governancePermission</span><span class="sxs-lookup"><span data-stu-id="b98c8-103">governancePermission resource type</span></span>

<span data-ttu-id="b98c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b98c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b98c8-105">Представляет разрешение на доступ, которое [имеется у governanceSubject](../resources/governancesubject.md) к определенному [governanceResource.](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="b98c8-105">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>


## <a name="properties"></a><span data-ttu-id="b98c8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b98c8-106">Properties</span></span>
| <span data-ttu-id="b98c8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b98c8-107">Property</span></span>     | <span data-ttu-id="b98c8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b98c8-108">Type</span></span>   |<span data-ttu-id="b98c8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b98c8-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b98c8-110">accessLevel</span><span class="sxs-lookup"><span data-stu-id="b98c8-110">accessLevel</span></span>|<span data-ttu-id="b98c8-111">Строка</span><span class="sxs-lookup"><span data-stu-id="b98c8-111">String</span></span>|<span data-ttu-id="b98c8-112">Уровень доступа.</span><span class="sxs-lookup"><span data-stu-id="b98c8-112">The access level.</span></span> <span data-ttu-id="b98c8-113">Допустимые значения: ``None`` , , , и ``UserRead`` ``AdminRead`` ``AdminReadWrite`` .</span><span class="sxs-lookup"><span data-stu-id="b98c8-113">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="b98c8-114">isActive</span><span class="sxs-lookup"><span data-stu-id="b98c8-114">isActive</span></span>|<span data-ttu-id="b98c8-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="b98c8-115">Boolean</span></span>|<span data-ttu-id="b98c8-116">Указать, есть ли у запрашивателя назначение активной роли для уровня доступа.</span><span class="sxs-lookup"><span data-stu-id="b98c8-116">Indicate if the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="b98c8-117">isEligible</span><span class="sxs-lookup"><span data-stu-id="b98c8-117">isEligible</span></span>|<span data-ttu-id="b98c8-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="b98c8-118">Boolean</span></span>|<span data-ttu-id="b98c8-119">Указать, есть ли у запрашивателя право на назначение роли для уровня доступа.</span><span class="sxs-lookup"><span data-stu-id="b98c8-119">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b98c8-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b98c8-120">JSON representation</span></span>

<span data-ttu-id="b98c8-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b98c8-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governancePermission"
}-->
```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```


