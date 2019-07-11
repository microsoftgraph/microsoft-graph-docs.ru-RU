---
title: Тип ресурса Говернанцепермиссион
description: 'Представляет разрешение на доступ к определенному governanceResource в Говернанцесубжект.  '
localization_priority: Normal
ms.openlocfilehash: cd5b15a85dee7a193962a6072bcdf34b1d4f131a
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621307"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="fe175-103">Тип ресурса Говернанцепермиссион</span><span class="sxs-lookup"><span data-stu-id="fe175-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe175-104">Представляет разрешение на доступ к определенному [governanceResource](../resources/governanceresource.md)в [говернанцесубжект](../resources/governancesubject.md) .</span><span class="sxs-lookup"><span data-stu-id="fe175-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="fe175-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe175-105">Properties</span></span>
| <span data-ttu-id="fe175-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe175-106">Property</span></span>     | <span data-ttu-id="fe175-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fe175-107">Type</span></span>   |<span data-ttu-id="fe175-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fe175-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe175-109">accessLevel</span><span class="sxs-lookup"><span data-stu-id="fe175-109">accessLevel</span></span>|<span data-ttu-id="fe175-110">String</span><span class="sxs-lookup"><span data-stu-id="fe175-110">String</span></span>|<span data-ttu-id="fe175-111">Уровень доступа.</span><span class="sxs-lookup"><span data-stu-id="fe175-111">The access level.</span></span> <span data-ttu-id="fe175-112">Допустимые значения ``None``: ``UserRead``, ``AdminRead``, и ``AdminReadWrite``.</span><span class="sxs-lookup"><span data-stu-id="fe175-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="fe175-113">isActive</span><span class="sxs-lookup"><span data-stu-id="fe175-113">isActive</span></span>|<span data-ttu-id="fe175-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe175-114">Boolean</span></span>|<span data-ttu-id="fe175-115">Указывает, имеет ли запрашивающая сторона какие – либо активные назначения ролей для этого уровня доступа.</span><span class="sxs-lookup"><span data-stu-id="fe175-115">Indicate if the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="fe175-116">Действительный</span><span class="sxs-lookup"><span data-stu-id="fe175-116">isEligible</span></span>|<span data-ttu-id="fe175-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe175-117">Boolean</span></span>|<span data-ttu-id="fe175-118">Указывает, имеет ли запрашивающее назначение роли для уровня доступа.</span><span class="sxs-lookup"><span data-stu-id="fe175-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe175-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe175-119">JSON representation</span></span>

<span data-ttu-id="fe175-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe175-120">Here is a JSON representation of the resource.</span></span>
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
