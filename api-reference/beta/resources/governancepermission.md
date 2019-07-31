---
title: Тип ресурса Говернанцепермиссион
description: 'Представляет разрешение на доступ к определенному governanceResource в Говернанцесубжект.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8bf32b855ed77ccdf712b1a739ef913d0a3dade0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971946"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="6db9e-103">Тип ресурса Говернанцепермиссион</span><span class="sxs-lookup"><span data-stu-id="6db9e-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6db9e-104">Представляет разрешение на доступ к определенному [governanceResource](../resources/governanceresource.md)в [говернанцесубжект](../resources/governancesubject.md) .</span><span class="sxs-lookup"><span data-stu-id="6db9e-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="6db9e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6db9e-105">Properties</span></span>
| <span data-ttu-id="6db9e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6db9e-106">Property</span></span>     | <span data-ttu-id="6db9e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6db9e-107">Type</span></span>   |<span data-ttu-id="6db9e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6db9e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6db9e-109">accessLevel</span><span class="sxs-lookup"><span data-stu-id="6db9e-109">accessLevel</span></span>|<span data-ttu-id="6db9e-110">String</span><span class="sxs-lookup"><span data-stu-id="6db9e-110">String</span></span>|<span data-ttu-id="6db9e-111">Уровень доступа.</span><span class="sxs-lookup"><span data-stu-id="6db9e-111">The access level.</span></span> <span data-ttu-id="6db9e-112">Допустимые значения ``None``: ``UserRead``, ``AdminRead``, и ``AdminReadWrite``.</span><span class="sxs-lookup"><span data-stu-id="6db9e-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="6db9e-113">isActive</span><span class="sxs-lookup"><span data-stu-id="6db9e-113">isActive</span></span>|<span data-ttu-id="6db9e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="6db9e-114">Boolean</span></span>|<span data-ttu-id="6db9e-115">Указывает, имеет ли запрашивающая сторона какие – либо активные назначения ролей для этого уровня доступа.</span><span class="sxs-lookup"><span data-stu-id="6db9e-115">Indicate if the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="6db9e-116">Действительный</span><span class="sxs-lookup"><span data-stu-id="6db9e-116">isEligible</span></span>|<span data-ttu-id="6db9e-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="6db9e-117">Boolean</span></span>|<span data-ttu-id="6db9e-118">Указывает, имеет ли запрашивающее назначение роли для уровня доступа.</span><span class="sxs-lookup"><span data-stu-id="6db9e-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6db9e-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6db9e-119">JSON representation</span></span>

<span data-ttu-id="6db9e-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6db9e-120">Here is a JSON representation of the resource.</span></span>
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
