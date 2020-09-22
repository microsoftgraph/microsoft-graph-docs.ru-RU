---
title: Тип ресурса Говернанцепермиссион
description: 'Представляет разрешение на доступ к определенному governanceResource в Говернанцесубжект.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 14c8335cab401c246f95452dac699daa4f81ea93
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033848"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="57140-103">Тип ресурса Говернанцепермиссион</span><span class="sxs-lookup"><span data-stu-id="57140-103">governancePermission resource type</span></span>

<span data-ttu-id="57140-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57140-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57140-105">Представляет разрешение на доступ к определенному [governanceResource](../resources/governanceresource.md)в [говернанцесубжект](../resources/governancesubject.md) .</span><span class="sxs-lookup"><span data-stu-id="57140-105">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>


## <a name="properties"></a><span data-ttu-id="57140-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="57140-106">Properties</span></span>
| <span data-ttu-id="57140-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="57140-107">Property</span></span>     | <span data-ttu-id="57140-108">Тип</span><span class="sxs-lookup"><span data-stu-id="57140-108">Type</span></span>   |<span data-ttu-id="57140-109">Описание</span><span class="sxs-lookup"><span data-stu-id="57140-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57140-110">accessLevel</span><span class="sxs-lookup"><span data-stu-id="57140-110">accessLevel</span></span>|<span data-ttu-id="57140-111">String</span><span class="sxs-lookup"><span data-stu-id="57140-111">String</span></span>|<span data-ttu-id="57140-112">Уровень доступа.</span><span class="sxs-lookup"><span data-stu-id="57140-112">The access level.</span></span> <span data-ttu-id="57140-113">Допустимые значения: ``None`` ,, ``UserRead`` ``AdminRead`` и ``AdminReadWrite`` .</span><span class="sxs-lookup"><span data-stu-id="57140-113">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="57140-114">isActive</span><span class="sxs-lookup"><span data-stu-id="57140-114">isActive</span></span>|<span data-ttu-id="57140-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="57140-115">Boolean</span></span>|<span data-ttu-id="57140-116">Указывает, имеет ли запрашивающая сторона какие – либо активные назначения ролей для этого уровня доступа.</span><span class="sxs-lookup"><span data-stu-id="57140-116">Indicate if the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="57140-117">Действительный</span><span class="sxs-lookup"><span data-stu-id="57140-117">isEligible</span></span>|<span data-ttu-id="57140-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="57140-118">Boolean</span></span>|<span data-ttu-id="57140-119">Указывает, имеет ли запрашивающее назначение роли для уровня доступа.</span><span class="sxs-lookup"><span data-stu-id="57140-119">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57140-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57140-120">JSON representation</span></span>

<span data-ttu-id="57140-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57140-121">Here is a JSON representation of the resource.</span></span>
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


