---
title: Тип ресурса governanceSubject
description: Представляет пользователей, группы и участников-служб, которыми управляет privileged Identity Management (PIM).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: eedcaff8538d5a0efa110b34cd6a72aef2a3210a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132680"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="96e1b-103">Тип ресурса governanceSubject</span><span class="sxs-lookup"><span data-stu-id="96e1b-103">governanceSubject resource type</span></span>

<span data-ttu-id="96e1b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96e1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96e1b-105">Представляет пользователей, группы и участников-служб, которыми управляет privileged Identity Management (PIM).</span><span class="sxs-lookup"><span data-stu-id="96e1b-105">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="96e1b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="96e1b-106">Properties</span></span>
| <span data-ttu-id="96e1b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="96e1b-107">Property</span></span>  | <span data-ttu-id="96e1b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="96e1b-108">Type</span></span>       |<span data-ttu-id="96e1b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="96e1b-109">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="96e1b-110">id</span><span class="sxs-lookup"><span data-stu-id="96e1b-110">id</span></span>         |<span data-ttu-id="96e1b-111">Строка</span><span class="sxs-lookup"><span data-stu-id="96e1b-111">String</span></span>     | <span data-ttu-id="96e1b-112">ИД темы.</span><span class="sxs-lookup"><span data-stu-id="96e1b-112">The id of the subject.</span></span>|
|<span data-ttu-id="96e1b-113">type</span><span class="sxs-lookup"><span data-stu-id="96e1b-113">type</span></span>       |<span data-ttu-id="96e1b-114">Строка</span><span class="sxs-lookup"><span data-stu-id="96e1b-114">String</span></span>     |<span data-ttu-id="96e1b-115">Тип темы.</span><span class="sxs-lookup"><span data-stu-id="96e1b-115">The type of the subject.</span></span> <span data-ttu-id="96e1b-116">Значение может быть ``User`` , ``Group`` и ``ServicePrincipal`` .</span><span class="sxs-lookup"><span data-stu-id="96e1b-116">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="96e1b-117">displayName</span><span class="sxs-lookup"><span data-stu-id="96e1b-117">displayName</span></span>|<span data-ttu-id="96e1b-118">Строка</span><span class="sxs-lookup"><span data-stu-id="96e1b-118">String</span></span>     |<span data-ttu-id="96e1b-119">Отображаемого имени темы.</span><span class="sxs-lookup"><span data-stu-id="96e1b-119">The display name of the subject.</span></span>|
|<span data-ttu-id="96e1b-120">email</span><span class="sxs-lookup"><span data-stu-id="96e1b-120">email</span></span>      |<span data-ttu-id="96e1b-121">String</span><span class="sxs-lookup"><span data-stu-id="96e1b-121">String</span></span>     |<span data-ttu-id="96e1b-122">Адрес электронной почты субъекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="96e1b-122">The email address of the user subject.</span></span> <span data-ttu-id="96e1b-123">Если тема находится в других типах, она пуста.</span><span class="sxs-lookup"><span data-stu-id="96e1b-123">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="96e1b-124">principalName</span><span class="sxs-lookup"><span data-stu-id="96e1b-124">principalName</span></span>|<span data-ttu-id="96e1b-125">String</span><span class="sxs-lookup"><span data-stu-id="96e1b-125">String</span></span>   |<span data-ttu-id="96e1b-126">Имя субъекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="96e1b-126">The principal name of the user subject.</span></span> <span data-ttu-id="96e1b-127">Если тема находится в других типах, она пуста.</span><span class="sxs-lookup"><span data-stu-id="96e1b-127">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96e1b-128">Связи</span><span class="sxs-lookup"><span data-stu-id="96e1b-128">Relationships</span></span>
<span data-ttu-id="96e1b-129">Нет</span><span class="sxs-lookup"><span data-stu-id="96e1b-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="96e1b-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="96e1b-130">JSON representation</span></span>

<span data-ttu-id="96e1b-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96e1b-131">Here is a JSON representation of the resource.</span></span>

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


