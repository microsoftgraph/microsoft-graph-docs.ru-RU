---
title: Тип удостоверению пользователя
description: 'Для Azure AD вызвать обзоры, этот тип представляет удостоверение пользователя Azure AD для рецензент проверки доступа.  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 80e8cc68d4fc2f642be6c748b762fe47c7489d59
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932282"
---
# <a name="useridentity-type"></a><span data-ttu-id="18cf8-103">Тип удостоверению пользователя</span><span class="sxs-lookup"><span data-stu-id="18cf8-103">userIdentity type</span></span>

> <span data-ttu-id="18cf8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="18cf8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18cf8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18cf8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18cf8-106">Для Azure AD, [дается обзор доступа](accessreviews-root.md)этот тип представляет удостоверение пользователя Azure AD для рецензент проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="18cf8-106">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a reviewer of an access review.</span></span>  
<span data-ttu-id="18cf8-107">В контексте журнал аудита Azure AD представляет сведений о пользователе, который инициировал или затронутого пользователем действия аудита.</span><span class="sxs-lookup"><span data-stu-id="18cf8-107">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="18cf8-108">Этот тип наследуется от [удостоверения](identity.md) и одного дополнительного свойства имя участника-пользователя пользователя.</span><span class="sxs-lookup"><span data-stu-id="18cf8-108">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="18cf8-109">Methods</span><span class="sxs-lookup"><span data-stu-id="18cf8-109">Methods</span></span>

<span data-ttu-id="18cf8-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="18cf8-110">None.</span></span>  <span data-ttu-id="18cf8-111">Объекты этого типа будет включать в теле запроса при [создании accessReview](../api/accessreview-create.md).</span><span class="sxs-lookup"><span data-stu-id="18cf8-111">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="18cf8-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="18cf8-112">Properties</span></span>
| <span data-ttu-id="18cf8-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="18cf8-113">Property</span></span>     | <span data-ttu-id="18cf8-114">Тип</span><span class="sxs-lookup"><span data-stu-id="18cf8-114">Type</span></span>   |<span data-ttu-id="18cf8-115">Описание</span><span class="sxs-lookup"><span data-stu-id="18cf8-115">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="18cf8-116">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="18cf8-116">The identity's display name.</span></span> <span data-ttu-id="18cf8-117">Обратите внимание, что не всегда возможно, доступен или актуальными.</span><span class="sxs-lookup"><span data-stu-id="18cf8-117">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="18cf8-118">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="18cf8-118">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="18cf8-119">Указывает IP-адрес клиента, используемых пользователь, выполняющий действие (только для журнала аудита).</span><span class="sxs-lookup"><span data-stu-id="18cf8-119">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="18cf8-120">Атрибут userPrincipalName пользователя.</span><span class="sxs-lookup"><span data-stu-id="18cf8-120">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="18cf8-121">Заметки</span><span class="sxs-lookup"><span data-stu-id="18cf8-121">Remarks</span></span>

<span data-ttu-id="18cf8-p104">В некоторых случаях уникальный идентификатор субъекта может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.</span><span class="sxs-lookup"><span data-stu-id="18cf8-p104">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="18cf8-124">Связи</span><span class="sxs-lookup"><span data-stu-id="18cf8-124">Relationships</span></span>

<span data-ttu-id="18cf8-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="18cf8-125">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="18cf8-126">См. также</span><span class="sxs-lookup"><span data-stu-id="18cf8-126">See also</span></span>

| <span data-ttu-id="18cf8-127">Метод</span><span class="sxs-lookup"><span data-stu-id="18cf8-127">Method</span></span>           | <span data-ttu-id="18cf8-128">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="18cf8-128">Return Type</span></span>    |<span data-ttu-id="18cf8-129">Описание</span><span class="sxs-lookup"><span data-stu-id="18cf8-129">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="18cf8-130">Получение accessReview рецензентов</span><span class="sxs-lookup"><span data-stu-id="18cf8-130">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="18cf8-131">Коллекция [удостоверению пользователя](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="18cf8-131">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="18cf8-132">Получите рецензентов accessReview.</span><span class="sxs-lookup"><span data-stu-id="18cf8-132">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="18cf8-133">Добавление accessReview редактор</span><span class="sxs-lookup"><span data-stu-id="18cf8-133">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="18cf8-134">Нет.</span><span class="sxs-lookup"><span data-stu-id="18cf8-134">None.</span></span>   |   <span data-ttu-id="18cf8-135">Добавьте проверяющий accessReview.</span><span class="sxs-lookup"><span data-stu-id="18cf8-135">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="18cf8-136">Удаление accessReview редактор</span><span class="sxs-lookup"><span data-stu-id="18cf8-136">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="18cf8-137">Нет.</span><span class="sxs-lookup"><span data-stu-id="18cf8-137">None.</span></span>  |   <span data-ttu-id="18cf8-138">Удаление рецензента из accessReview.</span><span class="sxs-lookup"><span data-stu-id="18cf8-138">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="18cf8-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18cf8-139">JSON representation</span></span>

<span data-ttu-id="18cf8-140">Ниже представлена JSON типа.</span><span class="sxs-lookup"><span data-stu-id="18cf8-140">Here is a JSON representation of the type.</span></span>

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
 "userPrincipalName": "String"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
