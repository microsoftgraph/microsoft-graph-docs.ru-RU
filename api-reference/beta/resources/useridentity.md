---
title: тип userIdentity
description: Представляет идентификатор пользователя Azure AD для рецензента обзора доступа.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 9379955a4356ff9c969e4813fbf9b812316aa821
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719859"
---
# <a name="useridentity-type"></a><span data-ttu-id="4599e-103">тип userIdentity</span><span class="sxs-lookup"><span data-stu-id="4599e-103">userIdentity type</span></span>

<span data-ttu-id="4599e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4599e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4599e-105">Для обзоров доступа к Azure [AD](accessreviews-root.md)этот тип представляет идентификатор пользователя Azure AD для создателя или рецензента обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="4599e-105">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a creator or reviewer of an access review.</span></span>
<span data-ttu-id="4599e-106">В контексте журнала аудита Azure AD это представляет сведения пользователей, которые инициировали или пострадали от действий аудита.</span><span class="sxs-lookup"><span data-stu-id="4599e-106">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="4599e-107">Этот тип наследуется от [удостоверения](identity.md) и имеет одно дополнительное свойство, основное имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="4599e-107">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="4599e-108">Methods</span><span class="sxs-lookup"><span data-stu-id="4599e-108">Methods</span></span>

<span data-ttu-id="4599e-109">Нет</span><span class="sxs-lookup"><span data-stu-id="4599e-109">None.</span></span>  <span data-ttu-id="4599e-110">При создании [accessReview](../api/accessreview-create.md)в тело запроса будут включены объекты этого типа.</span><span class="sxs-lookup"><span data-stu-id="4599e-110">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4599e-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="4599e-111">Properties</span></span>

| <span data-ttu-id="4599e-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="4599e-112">Property</span></span> | <span data-ttu-id="4599e-113">Тип</span><span class="sxs-lookup"><span data-stu-id="4599e-113">Type</span></span> | <span data-ttu-id="4599e-114">Описание</span><span class="sxs-lookup"><span data-stu-id="4599e-114">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="4599e-115">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4599e-115">The identity's display name.</span></span> <span data-ttu-id="4599e-116">Обратите внимание, что это может быть не всегда доступно или в курсе.</span><span class="sxs-lookup"><span data-stu-id="4599e-116">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="4599e-117">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4599e-117">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="4599e-118">Указывает IP-адрес клиента, используемый пользователем для выполнения действия (только журнал аудита).</span><span class="sxs-lookup"><span data-stu-id="4599e-118">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="4599e-119">Атрибут userPrincipalName пользователя.</span><span class="sxs-lookup"><span data-stu-id="4599e-119">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="4599e-120">Заметки</span><span class="sxs-lookup"><span data-stu-id="4599e-120">Remarks</span></span>

<span data-ttu-id="4599e-p104">В некоторых случаях уникальный идентификатор субъекта может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.</span><span class="sxs-lookup"><span data-stu-id="4599e-p104">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="4599e-123">Связи</span><span class="sxs-lookup"><span data-stu-id="4599e-123">Relationships</span></span>

<span data-ttu-id="4599e-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4599e-124">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="4599e-125">См. также</span><span class="sxs-lookup"><span data-stu-id="4599e-125">See also</span></span>

| <span data-ttu-id="4599e-126">Метод</span><span class="sxs-lookup"><span data-stu-id="4599e-126">Method</span></span>                                                                | <span data-ttu-id="4599e-127">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4599e-127">Return Type</span></span>                                | <span data-ttu-id="4599e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4599e-128">Description</span></span>                             |
|:----------------------------------------------------------------------|:-------------------------------------------|:----------------------------------------|
| [<span data-ttu-id="4599e-129">Получите рецензенты accessReview</span><span class="sxs-lookup"><span data-stu-id="4599e-129">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md)    | <span data-ttu-id="4599e-130">[коллекция userIdentity](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="4599e-130">[userIdentity](useridentity.md) collection</span></span> | <span data-ttu-id="4599e-131">Получите рецензентов accessReview.</span><span class="sxs-lookup"><span data-stu-id="4599e-131">Get the reviewers of an accessReview.</span></span>   |
| [<span data-ttu-id="4599e-132">Добавление рецензента accessReview</span><span class="sxs-lookup"><span data-stu-id="4599e-132">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md)       | <span data-ttu-id="4599e-133">Нет</span><span class="sxs-lookup"><span data-stu-id="4599e-133">None.</span></span>                                      | <span data-ttu-id="4599e-134">Добавление рецензента в accessReview.</span><span class="sxs-lookup"><span data-stu-id="4599e-134">Add a reviewer to an accessReview.</span></span>      |
| [<span data-ttu-id="4599e-135">Удаление рецензента accessReview</span><span class="sxs-lookup"><span data-stu-id="4599e-135">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="4599e-136">Нет</span><span class="sxs-lookup"><span data-stu-id="4599e-136">None.</span></span>                                      | <span data-ttu-id="4599e-137">Удаление рецензента из accessReview.</span><span class="sxs-lookup"><span data-stu-id="4599e-137">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4599e-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4599e-138">JSON representation</span></span>

<span data-ttu-id="4599e-139">Вот представление JSON этого типа.</span><span class="sxs-lookup"><span data-stu-id="4599e-139">Here is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
"displayName", "thumbnails"
  ],
  "@odata.type": "microsoft.graph.userIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string",
  "userPrincipalName": "String",
  "ipAddress": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


