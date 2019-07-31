---
title: Тип ресурса Говернанцесубжект
description: Представляет пользователей, группы и субъекты-службы, которыми управляет привилегированный Диспетчер удостоверений (PIM).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 26f6c6904de97fc96eb1b29b9bcbc376bcf69c61
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005977"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="3c1f5-103">Тип ресурса Говернанцесубжект</span><span class="sxs-lookup"><span data-stu-id="3c1f5-103">governanceSubject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c1f5-104">Представляет пользователей, группы и субъекты-службы, которыми управляет привилегированный Диспетчер удостоверений (PIM).</span><span class="sxs-lookup"><span data-stu-id="3c1f5-104">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="3c1f5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c1f5-105">Properties</span></span>
| <span data-ttu-id="3c1f5-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c1f5-106">Property</span></span>  | <span data-ttu-id="3c1f5-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3c1f5-107">Type</span></span>       |<span data-ttu-id="3c1f5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3c1f5-108">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="3c1f5-109">id</span><span class="sxs-lookup"><span data-stu-id="3c1f5-109">id</span></span>         |<span data-ttu-id="3c1f5-110">String</span><span class="sxs-lookup"><span data-stu-id="3c1f5-110">String</span></span>     | <span data-ttu-id="3c1f5-111">Идентификатор субъекта.</span><span class="sxs-lookup"><span data-stu-id="3c1f5-111">The id of the subject.</span></span>|
|<span data-ttu-id="3c1f5-112">type</span><span class="sxs-lookup"><span data-stu-id="3c1f5-112">type</span></span>       |<span data-ttu-id="3c1f5-113">String</span><span class="sxs-lookup"><span data-stu-id="3c1f5-113">String</span></span>     |<span data-ttu-id="3c1f5-114">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="3c1f5-114">The type of the subject.</span></span> <span data-ttu-id="3c1f5-115">Возможные значения: ``User``, ``Group``и. ``ServicePrincipal``</span><span class="sxs-lookup"><span data-stu-id="3c1f5-115">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="3c1f5-116">displayName</span><span class="sxs-lookup"><span data-stu-id="3c1f5-116">displayName</span></span>|<span data-ttu-id="3c1f5-117">Строка</span><span class="sxs-lookup"><span data-stu-id="3c1f5-117">String</span></span>     |<span data-ttu-id="3c1f5-118">Отображаемое имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="3c1f5-118">The display name of the subject.</span></span>|
|<span data-ttu-id="3c1f5-119">email</span><span class="sxs-lookup"><span data-stu-id="3c1f5-119">email</span></span>      |<span data-ttu-id="3c1f5-120">String</span><span class="sxs-lookup"><span data-stu-id="3c1f5-120">String</span></span>     |<span data-ttu-id="3c1f5-121">Адрес электронной почты субъекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="3c1f5-121">The email address of the user subject.</span></span> <span data-ttu-id="3c1f5-122">Если тема находится в других типах, она пуста.</span><span class="sxs-lookup"><span data-stu-id="3c1f5-122">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="3c1f5-123">principalName</span><span class="sxs-lookup"><span data-stu-id="3c1f5-123">principalName</span></span>|<span data-ttu-id="3c1f5-124">String</span><span class="sxs-lookup"><span data-stu-id="3c1f5-124">String</span></span>   |<span data-ttu-id="3c1f5-125">Имя субъекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="3c1f5-125">The principal name of the user subject.</span></span> <span data-ttu-id="3c1f5-126">Если тема находится в других типах, она пуста.</span><span class="sxs-lookup"><span data-stu-id="3c1f5-126">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c1f5-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="3c1f5-127">Relationships</span></span>
<span data-ttu-id="3c1f5-128">Нет</span><span class="sxs-lookup"><span data-stu-id="3c1f5-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3c1f5-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c1f5-129">JSON representation</span></span>

<span data-ttu-id="3c1f5-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c1f5-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSubject"
}-->

```json
{
  "id": "String",  
  "displayName": "String",
  "email": "String",
  "principalName": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
