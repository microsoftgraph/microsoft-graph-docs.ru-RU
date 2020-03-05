---
title: Тип userIdentity
description: 'Для проверок доступа Azure AD этот тип представляет удостоверение пользователя Azure AD для проверяющего, проверяющего доступ.  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 466b39a52f2bc2b9e20f313f3f80926855f492f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519528"
---
# <a name="useridentity-type"></a><span data-ttu-id="21601-103">Тип userIdentity</span><span class="sxs-lookup"><span data-stu-id="21601-103">userIdentity type</span></span>

<span data-ttu-id="21601-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="21601-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21601-105">Для [просмотров Access](accessreviews-root.md)Azure AD этот тип представляет собой удостоверение пользователя Azure AD для создателя или рецензента проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="21601-105">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a creator or reviewer of an access review.</span></span>  
<span data-ttu-id="21601-106">В контексте журнала аудита Azure AD — это сведения о пользователях, которые были инициированы или затронуты действием аудита.</span><span class="sxs-lookup"><span data-stu-id="21601-106">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="21601-107">Этот тип наследуется от [Identity](identity.md) и имеет одно дополнительное свойство, имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="21601-107">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="21601-108">Методы</span><span class="sxs-lookup"><span data-stu-id="21601-108">Methods</span></span>

<span data-ttu-id="21601-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="21601-109">None.</span></span>  <span data-ttu-id="21601-110">При [создании акцессревиев](../api/accessreview-create.md)необходимо включить в текст запроса объекты этого типа.</span><span class="sxs-lookup"><span data-stu-id="21601-110">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="21601-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="21601-111">Properties</span></span>
| <span data-ttu-id="21601-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="21601-112">Property</span></span>     | <span data-ttu-id="21601-113">Тип</span><span class="sxs-lookup"><span data-stu-id="21601-113">Type</span></span>   |<span data-ttu-id="21601-114">Описание</span><span class="sxs-lookup"><span data-stu-id="21601-114">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="21601-115">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="21601-115">The identity's display name.</span></span> <span data-ttu-id="21601-116">Обратите внимание, что эта возможность не всегда доступна или не актуальна.</span><span class="sxs-lookup"><span data-stu-id="21601-116">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="21601-117">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="21601-117">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="21601-118">IP-адрес клиента, используемый пользователем для выполнения действия (только журнал аудита).</span><span class="sxs-lookup"><span data-stu-id="21601-118">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="21601-119">Атрибут userPrincipalName пользователя.</span><span class="sxs-lookup"><span data-stu-id="21601-119">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="21601-120">Заметки</span><span class="sxs-lookup"><span data-stu-id="21601-120">Remarks</span></span>

<span data-ttu-id="21601-p103">В некоторых случаях уникальный идентификатор субъекта может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.</span><span class="sxs-lookup"><span data-stu-id="21601-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="21601-123">Связи</span><span class="sxs-lookup"><span data-stu-id="21601-123">Relationships</span></span>

<span data-ttu-id="21601-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="21601-124">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="21601-125">См. также</span><span class="sxs-lookup"><span data-stu-id="21601-125">See also</span></span>

| <span data-ttu-id="21601-126">Метод</span><span class="sxs-lookup"><span data-stu-id="21601-126">Method</span></span>           | <span data-ttu-id="21601-127">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="21601-127">Return Type</span></span>    |<span data-ttu-id="21601-128">Описание</span><span class="sxs-lookup"><span data-stu-id="21601-128">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="21601-129">Получение рецензентов Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="21601-129">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="21601-130">Коллекция [userIdentity](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="21601-130">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="21601-131">Получение рецензентов объекта Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="21601-131">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="21601-132">Добавление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="21601-132">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="21601-133">Нет.</span><span class="sxs-lookup"><span data-stu-id="21601-133">None.</span></span>   |   <span data-ttu-id="21601-134">Добавьте проверяющего в объект Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="21601-134">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="21601-135">Удаление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="21601-135">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="21601-136">Нет.</span><span class="sxs-lookup"><span data-stu-id="21601-136">None.</span></span>  |   <span data-ttu-id="21601-137">Удаление проверяющего из Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="21601-137">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="21601-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21601-138">JSON representation</span></span>

<span data-ttu-id="21601-139">Ниже показано представление типа в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21601-139">Here is a JSON representation of the type.</span></span>

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
