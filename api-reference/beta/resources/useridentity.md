---
title: Тип userIdentity
description: 'Для проверок доступа Azure AD этот тип представляет удостоверение пользователя Azure AD для проверяющего, проверяющего доступ.  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 554aa9d38b4635ab3410fd95441b5c5045a1f1f6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345051"
---
# <a name="useridentity-type"></a><span data-ttu-id="8db5e-103">Тип userIdentity</span><span class="sxs-lookup"><span data-stu-id="8db5e-103">userIdentity type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8db5e-104">Для [просмотров Access](accessreviews-root.md)Azure AD этот тип представляет собой удостоверение пользователя Azure AD для создателя или рецензента проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="8db5e-104">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a creator or reviewer of an access review.</span></span>  
<span data-ttu-id="8db5e-105">В контексте журнала аудита Azure AD — это сведения о пользователях, которые были инициированы или затронуты действием аудита.</span><span class="sxs-lookup"><span data-stu-id="8db5e-105">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="8db5e-106">Этот тип наследуется от [Identity](identity.md) и имеет одно дополнительное свойство, имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="8db5e-106">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="8db5e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8db5e-107">Methods</span></span>

<span data-ttu-id="8db5e-108">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8db5e-108">None.</span></span>  <span data-ttu-id="8db5e-109">При [создании Акцессревиев](../api/accessreview-create.md)необходимо включить в текст запроса объекты этого типа.</span><span class="sxs-lookup"><span data-stu-id="8db5e-109">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8db5e-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="8db5e-110">Properties</span></span>
| <span data-ttu-id="8db5e-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="8db5e-111">Property</span></span>     | <span data-ttu-id="8db5e-112">Тип</span><span class="sxs-lookup"><span data-stu-id="8db5e-112">Type</span></span>   |<span data-ttu-id="8db5e-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8db5e-113">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="8db5e-114">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="8db5e-114">The identity's display name.</span></span> <span data-ttu-id="8db5e-115">Обратите внимание, что эта возможность не всегда доступна или не актуальна.</span><span class="sxs-lookup"><span data-stu-id="8db5e-115">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="8db5e-116">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="8db5e-116">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="8db5e-117">IP-адрес клиента, используемый пользователем для выполнения действия (только журнал аудита).</span><span class="sxs-lookup"><span data-stu-id="8db5e-117">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="8db5e-118">Атрибут userPrincipalName пользователя.</span><span class="sxs-lookup"><span data-stu-id="8db5e-118">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="8db5e-119">Заметки</span><span class="sxs-lookup"><span data-stu-id="8db5e-119">Remarks</span></span>

<span data-ttu-id="8db5e-p103">В некоторых случаях уникальный идентификатор субъекта может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.</span><span class="sxs-lookup"><span data-stu-id="8db5e-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="8db5e-122">Связи</span><span class="sxs-lookup"><span data-stu-id="8db5e-122">Relationships</span></span>

<span data-ttu-id="8db5e-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8db5e-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="8db5e-124">См. также</span><span class="sxs-lookup"><span data-stu-id="8db5e-124">See also</span></span>

| <span data-ttu-id="8db5e-125">Метод</span><span class="sxs-lookup"><span data-stu-id="8db5e-125">Method</span></span>           | <span data-ttu-id="8db5e-126">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8db5e-126">Return Type</span></span>    |<span data-ttu-id="8db5e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="8db5e-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8db5e-128">Получение рецензентов Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="8db5e-128">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="8db5e-129">Коллекция [userIdentity](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="8db5e-129">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="8db5e-130">Получение рецензентов объекта Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="8db5e-130">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="8db5e-131">Добавление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="8db5e-131">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="8db5e-132">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8db5e-132">None.</span></span>   |   <span data-ttu-id="8db5e-133">Добавьте проверяющего в объект Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="8db5e-133">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="8db5e-134">Удаление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="8db5e-134">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="8db5e-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8db5e-135">None.</span></span>  |   <span data-ttu-id="8db5e-136">Удаление проверяющего из Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="8db5e-136">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8db5e-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8db5e-137">JSON representation</span></span>

<span data-ttu-id="8db5e-138">Ниже показано представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8db5e-138">Here is a JSON representation of the type.</span></span>

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
