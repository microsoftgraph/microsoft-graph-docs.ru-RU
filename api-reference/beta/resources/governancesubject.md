---
title: Тип ресурса Говернанцесубжект
description: Представляет пользователей, группы и субъекты-службы, которыми управляет привилегированный Диспетчер удостоверений (PIM).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4d1fbf75b4e9643dc0e3b968ace7a013616904ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497173"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="a3172-103">Тип ресурса Говернанцесубжект</span><span class="sxs-lookup"><span data-stu-id="a3172-103">governanceSubject resource type</span></span>

<span data-ttu-id="a3172-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a3172-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3172-105">Представляет пользователей, группы и субъекты-службы, которыми управляет привилегированный Диспетчер удостоверений (PIM).</span><span class="sxs-lookup"><span data-stu-id="a3172-105">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="a3172-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3172-106">Properties</span></span>
| <span data-ttu-id="a3172-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3172-107">Property</span></span>  | <span data-ttu-id="a3172-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a3172-108">Type</span></span>       |<span data-ttu-id="a3172-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a3172-109">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="a3172-110">id</span><span class="sxs-lookup"><span data-stu-id="a3172-110">id</span></span>         |<span data-ttu-id="a3172-111">String</span><span class="sxs-lookup"><span data-stu-id="a3172-111">String</span></span>     | <span data-ttu-id="a3172-112">Идентификатор субъекта.</span><span class="sxs-lookup"><span data-stu-id="a3172-112">The id of the subject.</span></span>|
|<span data-ttu-id="a3172-113">type</span><span class="sxs-lookup"><span data-stu-id="a3172-113">type</span></span>       |<span data-ttu-id="a3172-114">String</span><span class="sxs-lookup"><span data-stu-id="a3172-114">String</span></span>     |<span data-ttu-id="a3172-115">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="a3172-115">The type of the subject.</span></span> <span data-ttu-id="a3172-116">Возможные значения: ``User``, ``Group``и. ``ServicePrincipal``</span><span class="sxs-lookup"><span data-stu-id="a3172-116">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="a3172-117">displayName</span><span class="sxs-lookup"><span data-stu-id="a3172-117">displayName</span></span>|<span data-ttu-id="a3172-118">Строка</span><span class="sxs-lookup"><span data-stu-id="a3172-118">String</span></span>     |<span data-ttu-id="a3172-119">Отображаемое имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="a3172-119">The display name of the subject.</span></span>|
|<span data-ttu-id="a3172-120">email</span><span class="sxs-lookup"><span data-stu-id="a3172-120">email</span></span>      |<span data-ttu-id="a3172-121">String</span><span class="sxs-lookup"><span data-stu-id="a3172-121">String</span></span>     |<span data-ttu-id="a3172-122">Адрес электронной почты субъекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="a3172-122">The email address of the user subject.</span></span> <span data-ttu-id="a3172-123">Если тема находится в других типах, она пуста.</span><span class="sxs-lookup"><span data-stu-id="a3172-123">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="a3172-124">principalName</span><span class="sxs-lookup"><span data-stu-id="a3172-124">principalName</span></span>|<span data-ttu-id="a3172-125">String</span><span class="sxs-lookup"><span data-stu-id="a3172-125">String</span></span>   |<span data-ttu-id="a3172-126">Имя субъекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="a3172-126">The principal name of the user subject.</span></span> <span data-ttu-id="a3172-127">Если тема находится в других типах, она пуста.</span><span class="sxs-lookup"><span data-stu-id="a3172-127">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3172-128">Связи</span><span class="sxs-lookup"><span data-stu-id="a3172-128">Relationships</span></span>
<span data-ttu-id="a3172-129">Нет</span><span class="sxs-lookup"><span data-stu-id="a3172-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a3172-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3172-130">JSON representation</span></span>

<span data-ttu-id="a3172-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3172-131">Here is a JSON representation of the resource.</span></span>

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
