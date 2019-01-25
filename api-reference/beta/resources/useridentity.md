---
title: Тип удостоверению пользователя
description: 'Для Azure AD вызвать обзоры, этот тип представляет удостоверение пользователя Azure AD для рецензент проверки доступа.  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ab8076c5ff24e20006b5a5569dacf4c45d987512
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529469"
---
# <a name="useridentity-type"></a><span data-ttu-id="36ecb-103">Тип удостоверению пользователя</span><span class="sxs-lookup"><span data-stu-id="36ecb-103">userIdentity type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36ecb-104">Для Azure AD, [дается обзор доступа](accessreviews-root.md)этот тип представляет удостоверение пользователя Azure AD для рецензент проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="36ecb-104">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a reviewer of an access review.</span></span>  
<span data-ttu-id="36ecb-105">В контексте журнал аудита Azure AD представляет сведений о пользователе, который инициировал или затронутого пользователем действия аудита.</span><span class="sxs-lookup"><span data-stu-id="36ecb-105">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="36ecb-106">Этот тип наследуется от [удостоверения](identity.md) и одного дополнительного свойства имя участника-пользователя пользователя.</span><span class="sxs-lookup"><span data-stu-id="36ecb-106">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="36ecb-107">Методы</span><span class="sxs-lookup"><span data-stu-id="36ecb-107">Methods</span></span>

<span data-ttu-id="36ecb-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="36ecb-108">None.</span></span>  <span data-ttu-id="36ecb-109">Объекты этого типа будет включать в теле запроса при [создании accessReview](../api/accessreview-create.md).</span><span class="sxs-lookup"><span data-stu-id="36ecb-109">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="36ecb-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="36ecb-110">Properties</span></span>
| <span data-ttu-id="36ecb-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="36ecb-111">Property</span></span>     | <span data-ttu-id="36ecb-112">Тип</span><span class="sxs-lookup"><span data-stu-id="36ecb-112">Type</span></span>   |<span data-ttu-id="36ecb-113">Описание</span><span class="sxs-lookup"><span data-stu-id="36ecb-113">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="36ecb-114">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="36ecb-114">The identity's display name.</span></span> <span data-ttu-id="36ecb-115">Обратите внимание, что не всегда возможно, доступен или актуальными.</span><span class="sxs-lookup"><span data-stu-id="36ecb-115">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="36ecb-116">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="36ecb-116">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="36ecb-117">Указывает IP-адрес клиента, используемых пользователь, выполняющий действие (только для журнала аудита).</span><span class="sxs-lookup"><span data-stu-id="36ecb-117">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="36ecb-118">Атрибут userPrincipalName пользователя.</span><span class="sxs-lookup"><span data-stu-id="36ecb-118">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="36ecb-119">Заметки</span><span class="sxs-lookup"><span data-stu-id="36ecb-119">Remarks</span></span>

<span data-ttu-id="36ecb-p103">В некоторых случаях уникальный идентификатор субъекта может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.</span><span class="sxs-lookup"><span data-stu-id="36ecb-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="36ecb-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="36ecb-122">Relationships</span></span>

<span data-ttu-id="36ecb-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="36ecb-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="36ecb-124">См. также</span><span class="sxs-lookup"><span data-stu-id="36ecb-124">See also</span></span>

| <span data-ttu-id="36ecb-125">Метод</span><span class="sxs-lookup"><span data-stu-id="36ecb-125">Method</span></span>           | <span data-ttu-id="36ecb-126">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="36ecb-126">Return Type</span></span>    |<span data-ttu-id="36ecb-127">Описание</span><span class="sxs-lookup"><span data-stu-id="36ecb-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="36ecb-128">Получение accessReview рецензентов</span><span class="sxs-lookup"><span data-stu-id="36ecb-128">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="36ecb-129">Коллекция [удостоверению пользователя](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="36ecb-129">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="36ecb-130">Получите рецензентов accessReview.</span><span class="sxs-lookup"><span data-stu-id="36ecb-130">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="36ecb-131">Добавление accessReview редактор</span><span class="sxs-lookup"><span data-stu-id="36ecb-131">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="36ecb-132">Нет.</span><span class="sxs-lookup"><span data-stu-id="36ecb-132">None.</span></span>   |   <span data-ttu-id="36ecb-133">Добавьте проверяющий accessReview.</span><span class="sxs-lookup"><span data-stu-id="36ecb-133">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="36ecb-134">Удаление accessReview редактор</span><span class="sxs-lookup"><span data-stu-id="36ecb-134">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="36ecb-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="36ecb-135">None.</span></span>  |   <span data-ttu-id="36ecb-136">Удаление рецензента из accessReview.</span><span class="sxs-lookup"><span data-stu-id="36ecb-136">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="36ecb-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36ecb-137">JSON representation</span></span>

<span data-ttu-id="36ecb-138">Ниже представлена JSON типа.</span><span class="sxs-lookup"><span data-stu-id="36ecb-138">Here is a JSON representation of the type.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/useridentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
