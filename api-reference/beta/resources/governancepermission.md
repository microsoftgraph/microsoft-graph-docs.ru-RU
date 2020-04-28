---
title: Тип ресурса Говернанцепермиссион
description: 'Представляет разрешение на доступ к определенному governanceResource в Говернанцесубжект.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3efdebea07bb824b2314af516810ca36ad43adc9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497624"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="eb8b0-103">Тип ресурса Говернанцепермиссион</span><span class="sxs-lookup"><span data-stu-id="eb8b0-103">governancePermission resource type</span></span>

<span data-ttu-id="eb8b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb8b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb8b0-105">Представляет разрешение на доступ к определенному [governanceResource](../resources/governanceresource.md)в [говернанцесубжект](../resources/governancesubject.md) .</span><span class="sxs-lookup"><span data-stu-id="eb8b0-105">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="eb8b0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb8b0-106">Properties</span></span>
| <span data-ttu-id="eb8b0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb8b0-107">Property</span></span>     | <span data-ttu-id="eb8b0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="eb8b0-108">Type</span></span>   |<span data-ttu-id="eb8b0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="eb8b0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb8b0-110">accessLevel</span><span class="sxs-lookup"><span data-stu-id="eb8b0-110">accessLevel</span></span>|<span data-ttu-id="eb8b0-111">String</span><span class="sxs-lookup"><span data-stu-id="eb8b0-111">String</span></span>|<span data-ttu-id="eb8b0-112">Уровень доступа.</span><span class="sxs-lookup"><span data-stu-id="eb8b0-112">The access level.</span></span> <span data-ttu-id="eb8b0-113">Допустимые значения ``None``: ``UserRead``, ``AdminRead``, и ``AdminReadWrite``.</span><span class="sxs-lookup"><span data-stu-id="eb8b0-113">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="eb8b0-114">isActive</span><span class="sxs-lookup"><span data-stu-id="eb8b0-114">isActive</span></span>|<span data-ttu-id="eb8b0-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb8b0-115">Boolean</span></span>|<span data-ttu-id="eb8b0-116">Указывает, имеет ли запрашивающая сторона какие – либо активные назначения ролей для этого уровня доступа.</span><span class="sxs-lookup"><span data-stu-id="eb8b0-116">Indicate if the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="eb8b0-117">Действительный</span><span class="sxs-lookup"><span data-stu-id="eb8b0-117">isEligible</span></span>|<span data-ttu-id="eb8b0-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb8b0-118">Boolean</span></span>|<span data-ttu-id="eb8b0-119">Указывает, имеет ли запрашивающее назначение роли для уровня доступа.</span><span class="sxs-lookup"><span data-stu-id="eb8b0-119">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb8b0-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb8b0-120">JSON representation</span></span>

<span data-ttu-id="eb8b0-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb8b0-121">Here is a JSON representation of the resource.</span></span>
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
