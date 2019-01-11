---
title: Тип ресурса governanceSubject
description: Представляет пользователей, групп и субъектов-служб, управляемых в управления правами Identity (PIM).
localization_priority: Normal
ms.openlocfilehash: f3f8762c9136a3ae92269f6c06f52000fb73f710
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832594"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="b9ed8-103">Тип ресурса governanceSubject</span><span class="sxs-lookup"><span data-stu-id="b9ed8-103">governanceSubject resource type</span></span>

> <span data-ttu-id="b9ed8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b9ed8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9ed8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9ed8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9ed8-106">Представляет пользователей, групп и субъектов-служб, управляемых в управления правами Identity (PIM).</span><span class="sxs-lookup"><span data-stu-id="b9ed8-106">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="b9ed8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9ed8-107">Properties</span></span>
| <span data-ttu-id="b9ed8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9ed8-108">Property</span></span>  | <span data-ttu-id="b9ed8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b9ed8-109">Type</span></span>       |<span data-ttu-id="b9ed8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b9ed8-110">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="b9ed8-111">id</span><span class="sxs-lookup"><span data-stu-id="b9ed8-111">id</span></span>         |<span data-ttu-id="b9ed8-112">Строка</span><span class="sxs-lookup"><span data-stu-id="b9ed8-112">String</span></span>     | <span data-ttu-id="b9ed8-113">Идентификатор субъекта.</span><span class="sxs-lookup"><span data-stu-id="b9ed8-113">The id of the subject.</span></span>|
|<span data-ttu-id="b9ed8-114">type</span><span class="sxs-lookup"><span data-stu-id="b9ed8-114">type</span></span>       |<span data-ttu-id="b9ed8-115">Строка</span><span class="sxs-lookup"><span data-stu-id="b9ed8-115">String</span></span>     |<span data-ttu-id="b9ed8-116">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="b9ed8-116">The type of the subject.</span></span> <span data-ttu-id="b9ed8-117">Значение может быть ``User``, ``Group``, и ``ServicePrincipal``.</span><span class="sxs-lookup"><span data-stu-id="b9ed8-117">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="b9ed8-118">displayName</span><span class="sxs-lookup"><span data-stu-id="b9ed8-118">displayName</span></span>|<span data-ttu-id="b9ed8-119">Строка</span><span class="sxs-lookup"><span data-stu-id="b9ed8-119">String</span></span>     |<span data-ttu-id="b9ed8-120">Отображаемое имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="b9ed8-120">The display name of the subject.</span></span>|
|<span data-ttu-id="b9ed8-121">email</span><span class="sxs-lookup"><span data-stu-id="b9ed8-121">email</span></span>      |<span data-ttu-id="b9ed8-122">String</span><span class="sxs-lookup"><span data-stu-id="b9ed8-122">String</span></span>     |<span data-ttu-id="b9ed8-123">Адрес электронной почты субъекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9ed8-123">The email address of the user subject.</span></span> <span data-ttu-id="b9ed8-124">Если темы в других типах, он будет пустым.</span><span class="sxs-lookup"><span data-stu-id="b9ed8-124">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="b9ed8-125">principalName</span><span class="sxs-lookup"><span data-stu-id="b9ed8-125">principalName</span></span>|<span data-ttu-id="b9ed8-126">String</span><span class="sxs-lookup"><span data-stu-id="b9ed8-126">String</span></span>   |<span data-ttu-id="b9ed8-127">Имя субъекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9ed8-127">The principal name of the user subject.</span></span> <span data-ttu-id="b9ed8-128">Если темы в других типах, он будет пустым.</span><span class="sxs-lookup"><span data-stu-id="b9ed8-128">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9ed8-129">Связи</span><span class="sxs-lookup"><span data-stu-id="b9ed8-129">Relationships</span></span>
<span data-ttu-id="b9ed8-130">Нет</span><span class="sxs-lookup"><span data-stu-id="b9ed8-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b9ed8-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b9ed8-131">JSON representation</span></span>

<span data-ttu-id="b9ed8-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9ed8-132">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
