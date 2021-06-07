---
title: тип userIdentity
description: Представляет идентификатор пользователя Azure AD для рецензента обзора доступа.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 94c0af9a5909966471594ab4c23003282f416849
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52750367"
---
# <a name="useridentity-type"></a><span data-ttu-id="05f97-103">тип userIdentity</span><span class="sxs-lookup"><span data-stu-id="05f97-103">userIdentity type</span></span>

<span data-ttu-id="05f97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05f97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05f97-105">Для обзоров доступа к Azure [AD](accessreviews-root.md)этот тип представляет идентификатор пользователя Azure AD для создателя или рецензента обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="05f97-105">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a creator or reviewer of an access review.</span></span>
<span data-ttu-id="05f97-106">В контексте журнала аудита Azure AD это представляет сведения пользователей, которые инициировали или пострадали от действий аудита.</span><span class="sxs-lookup"><span data-stu-id="05f97-106">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="05f97-107">Этот тип наследуется от [удостоверения](identity.md) и имеет одно дополнительное свойство, основное имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="05f97-107">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="05f97-108">Methods</span><span class="sxs-lookup"><span data-stu-id="05f97-108">Methods</span></span>

<span data-ttu-id="05f97-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="05f97-109">None.</span></span>  <span data-ttu-id="05f97-110">При создании [accessReview](../api/accessreview-create.md)в тело запроса будут включены объекты этого типа.</span><span class="sxs-lookup"><span data-stu-id="05f97-110">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="05f97-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="05f97-111">Properties</span></span>

| <span data-ttu-id="05f97-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="05f97-112">Property</span></span>          | <span data-ttu-id="05f97-113">Тип</span><span class="sxs-lookup"><span data-stu-id="05f97-113">Type</span></span>   | <span data-ttu-id="05f97-114">Описание</span><span class="sxs-lookup"><span data-stu-id="05f97-114">Description</span></span>                                                                            |
|:------------------|:-------|:---------------------------------------------------------------------------------------|
| <span data-ttu-id="05f97-115">displayName</span><span class="sxs-lookup"><span data-stu-id="05f97-115">displayName</span></span>       | <span data-ttu-id="05f97-116">String</span><span class="sxs-lookup"><span data-stu-id="05f97-116">String</span></span> | <span data-ttu-id="05f97-117">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="05f97-117">The identity's display name.</span></span> <span data-ttu-id="05f97-118">Обратите внимание, что это может быть не всегда доступно или в курсе.</span><span class="sxs-lookup"><span data-stu-id="05f97-118">Note that this may not always be available or up-to-date.</span></span> |
| <span data-ttu-id="05f97-119">id</span><span class="sxs-lookup"><span data-stu-id="05f97-119">id</span></span>                | <span data-ttu-id="05f97-120">String</span><span class="sxs-lookup"><span data-stu-id="05f97-120">String</span></span> | <span data-ttu-id="05f97-121">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="05f97-121">Unique identifier for the identity.</span></span> <span data-ttu-id="05f97-122">Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="05f97-122">Nullable.</span></span>                                                   |
| <span data-ttu-id="05f97-123">ipAddress</span><span class="sxs-lookup"><span data-stu-id="05f97-123">ipAddress</span></span>         | <span data-ttu-id="05f97-124">String</span><span class="sxs-lookup"><span data-stu-id="05f97-124">String</span></span> | <span data-ttu-id="05f97-125">Указывает IP-адрес клиента, используемый пользователем для выполнения действия (только журнал аудита).</span><span class="sxs-lookup"><span data-stu-id="05f97-125">Indicates the client IP address used by user performing the activity (audit log only).</span></span> |
| <span data-ttu-id="05f97-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="05f97-126">userPrincipalName</span></span> | <span data-ttu-id="05f97-127">String</span><span class="sxs-lookup"><span data-stu-id="05f97-127">String</span></span> | <span data-ttu-id="05f97-128">Атрибут userPrincipalName пользователя.</span><span class="sxs-lookup"><span data-stu-id="05f97-128">The userPrincipalName attribute of the user.</span></span>                                           |

### <a name="remarks"></a><span data-ttu-id="05f97-129">Заметки</span><span class="sxs-lookup"><span data-stu-id="05f97-129">Remarks</span></span>

<span data-ttu-id="05f97-p105">В некоторых случаях уникальный идентификатор субъекта может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.</span><span class="sxs-lookup"><span data-stu-id="05f97-p105">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="05f97-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="05f97-132">Relationships</span></span>

<span data-ttu-id="05f97-133">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="05f97-133">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="05f97-134">См. также</span><span class="sxs-lookup"><span data-stu-id="05f97-134">See also</span></span>

| <span data-ttu-id="05f97-135">Метод</span><span class="sxs-lookup"><span data-stu-id="05f97-135">Method</span></span>                                                                | <span data-ttu-id="05f97-136">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="05f97-136">Return Type</span></span>                                | <span data-ttu-id="05f97-137">Описание</span><span class="sxs-lookup"><span data-stu-id="05f97-137">Description</span></span>                             |
|:----------------------------------------------------------------------|:-------------------------------------------|:----------------------------------------|
| [<span data-ttu-id="05f97-138">Получите рецензенты accessReview</span><span class="sxs-lookup"><span data-stu-id="05f97-138">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md)    | <span data-ttu-id="05f97-139">[коллекция userIdentity](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="05f97-139">[userIdentity](useridentity.md) collection</span></span> | <span data-ttu-id="05f97-140">Получите рецензентов accessReview.</span><span class="sxs-lookup"><span data-stu-id="05f97-140">Get the reviewers of an accessReview.</span></span>   |
| [<span data-ttu-id="05f97-141">Добавление рецензента accessReview</span><span class="sxs-lookup"><span data-stu-id="05f97-141">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md)       | <span data-ttu-id="05f97-142">Нет.</span><span class="sxs-lookup"><span data-stu-id="05f97-142">None.</span></span>                                      | <span data-ttu-id="05f97-143">Добавление рецензента в accessReview.</span><span class="sxs-lookup"><span data-stu-id="05f97-143">Add a reviewer to an accessReview.</span></span>      |
| [<span data-ttu-id="05f97-144">Удаление рецензента accessReview</span><span class="sxs-lookup"><span data-stu-id="05f97-144">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="05f97-145">Нет.</span><span class="sxs-lookup"><span data-stu-id="05f97-145">None.</span></span>                                      | <span data-ttu-id="05f97-146">Удаление рецензента из accessReview.</span><span class="sxs-lookup"><span data-stu-id="05f97-146">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="05f97-147">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="05f97-147">JSON representation</span></span>

<span data-ttu-id="05f97-148">Вот представление JSON этого типа.</span><span class="sxs-lookup"><span data-stu-id="05f97-148">Here is a JSON representation of the type.</span></span>

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


