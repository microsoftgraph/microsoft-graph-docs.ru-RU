---
title: Тип ресурса Говернанцепермиссион
description: 'Представляет разрешение на доступ к определенному governanceResource в Говернанцесубжект.  '
localization_priority: Normal
ms.openlocfilehash: 2f6be4bdc502f829b1dcfd991d1c2ae6130dea8a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340184"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="89cfa-103">Тип ресурса Говернанцепермиссион</span><span class="sxs-lookup"><span data-stu-id="89cfa-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89cfa-104">Представляет разрешение на доступ к определенному [governanceResource](../resources/governanceresource.md)в [говернанцесубжект](../resources/governancesubject.md) .</span><span class="sxs-lookup"><span data-stu-id="89cfa-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="89cfa-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="89cfa-105">Properties</span></span>
| <span data-ttu-id="89cfa-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="89cfa-106">Property</span></span>     | <span data-ttu-id="89cfa-107">Тип</span><span class="sxs-lookup"><span data-stu-id="89cfa-107">Type</span></span>   |<span data-ttu-id="89cfa-108">Описание</span><span class="sxs-lookup"><span data-stu-id="89cfa-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89cfa-109">accessLevel</span><span class="sxs-lookup"><span data-stu-id="89cfa-109">accessLevel</span></span>|<span data-ttu-id="89cfa-110">String</span><span class="sxs-lookup"><span data-stu-id="89cfa-110">String</span></span>|<span data-ttu-id="89cfa-111">Уровень доступа.</span><span class="sxs-lookup"><span data-stu-id="89cfa-111">The access level.</span></span> <span data-ttu-id="89cfa-112">Допустимые значения ``None``: ``UserRead``, ``AdminRead``, и ``AdminReadWrite``.</span><span class="sxs-lookup"><span data-stu-id="89cfa-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="89cfa-113">isActive</span><span class="sxs-lookup"><span data-stu-id="89cfa-113">isActive</span></span>|<span data-ttu-id="89cfa-114">Логический</span><span class="sxs-lookup"><span data-stu-id="89cfa-114">Boolean</span></span>|<span data-ttu-id="89cfa-115">Указывает, имеет ли запрашивающая сторона какое – либо активное назначение ролей для этого уровня доступа.</span><span class="sxs-lookup"><span data-stu-id="89cfa-115">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="89cfa-116">Действительный</span><span class="sxs-lookup"><span data-stu-id="89cfa-116">isEligible</span></span>|<span data-ttu-id="89cfa-117">Логический</span><span class="sxs-lookup"><span data-stu-id="89cfa-117">Boolean</span></span>|<span data-ttu-id="89cfa-118">Указывает, имеет ли запрашивающее назначение роли для уровня доступа.</span><span class="sxs-lookup"><span data-stu-id="89cfa-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89cfa-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89cfa-119">JSON representation</span></span>

<span data-ttu-id="89cfa-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89cfa-120">Here is a JSON representation of the resource.</span></span>
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
