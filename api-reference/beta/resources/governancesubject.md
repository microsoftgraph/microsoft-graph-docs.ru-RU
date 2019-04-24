---
title: Тип ресурса Говернанцесубжект
description: Представляет пользователей, группы и субъекты-службы, которыми управляет привилегированный Диспетчер удостоверений (PIM).
localization_priority: Normal
ms.openlocfilehash: a83825a147429c81b3e83b2f2fb384672d2f527e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506436"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="2d935-103">Тип ресурса Говернанцесубжект</span><span class="sxs-lookup"><span data-stu-id="2d935-103">governanceSubject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d935-104">Представляет пользователей, группы и субъекты-службы, которыми управляет привилегированный Диспетчер удостоверений (PIM).</span><span class="sxs-lookup"><span data-stu-id="2d935-104">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="2d935-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d935-105">Properties</span></span>
| <span data-ttu-id="2d935-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d935-106">Property</span></span>  | <span data-ttu-id="2d935-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2d935-107">Type</span></span>       |<span data-ttu-id="2d935-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2d935-108">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="2d935-109">id</span><span class="sxs-lookup"><span data-stu-id="2d935-109">id</span></span>         |<span data-ttu-id="2d935-110">String</span><span class="sxs-lookup"><span data-stu-id="2d935-110">String</span></span>     | <span data-ttu-id="2d935-111">Идентификатор субъекта.</span><span class="sxs-lookup"><span data-stu-id="2d935-111">The id of the subject.</span></span>|
|<span data-ttu-id="2d935-112">type</span><span class="sxs-lookup"><span data-stu-id="2d935-112">type</span></span>       |<span data-ttu-id="2d935-113">String</span><span class="sxs-lookup"><span data-stu-id="2d935-113">String</span></span>     |<span data-ttu-id="2d935-114">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="2d935-114">The type of the subject.</span></span> <span data-ttu-id="2d935-115">Возможные значения: ``User``, ``Group``и. ``ServicePrincipal``</span><span class="sxs-lookup"><span data-stu-id="2d935-115">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="2d935-116">displayName</span><span class="sxs-lookup"><span data-stu-id="2d935-116">displayName</span></span>|<span data-ttu-id="2d935-117">Строка</span><span class="sxs-lookup"><span data-stu-id="2d935-117">String</span></span>     |<span data-ttu-id="2d935-118">Отображаемое имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="2d935-118">The display name of the subject.</span></span>|
|<span data-ttu-id="2d935-119">email</span><span class="sxs-lookup"><span data-stu-id="2d935-119">email</span></span>      |<span data-ttu-id="2d935-120">String</span><span class="sxs-lookup"><span data-stu-id="2d935-120">String</span></span>     |<span data-ttu-id="2d935-121">Адрес электронной почты субъекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d935-121">The email address of the user subject.</span></span> <span data-ttu-id="2d935-122">Если тема находится в других типах, она пуста.</span><span class="sxs-lookup"><span data-stu-id="2d935-122">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="2d935-123">principalName</span><span class="sxs-lookup"><span data-stu-id="2d935-123">principalName</span></span>|<span data-ttu-id="2d935-124">String</span><span class="sxs-lookup"><span data-stu-id="2d935-124">String</span></span>   |<span data-ttu-id="2d935-125">Имя субъекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d935-125">The principal name of the user subject.</span></span> <span data-ttu-id="2d935-126">Если тема находится в других типах, она пуста.</span><span class="sxs-lookup"><span data-stu-id="2d935-126">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d935-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="2d935-127">Relationships</span></span>
<span data-ttu-id="2d935-128">Нет</span><span class="sxs-lookup"><span data-stu-id="2d935-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2d935-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d935-129">JSON representation</span></span>

<span data-ttu-id="2d935-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d935-130">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/governancesubject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
