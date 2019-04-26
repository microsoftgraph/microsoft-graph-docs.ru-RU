---
title: Удаление рецензента Акцессревиев
description: 'В функции рецензирования Access в Azure AD обновите существующий объект Акцессревиев, чтобы удалить пользователя в качестве проверяющего.  Эта операция разрешена только для проверки доступа, которая еще не завершена, и только для проверки доступа, в которой явно указаны рецензенты. Эта операция не разрешена для проверки доступа, при которой пользователи просматривают собственный доступ, и не предназначены для проверки доступа, в которой владельцы группы назначаются в качестве проверяющих. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7c2b80659ae1f9d4ce547a9d64d81f1fdb0403c3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323099"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="36a14-105">Удаление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="36a14-105">Remove accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36a14-106">В функции рецензирования [Access](../resources/accessreviews-root.md) в Azure AD обновите существующий объект [акцессревиев](../resources/accessreview.md) , чтобы удалить пользователя в качестве проверяющего.</span><span class="sxs-lookup"><span data-stu-id="36a14-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="36a14-107">Эта операция разрешена только для проверки доступа, которая еще не завершена, и только для проверки доступа, в которой явно указаны рецензенты.</span><span class="sxs-lookup"><span data-stu-id="36a14-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="36a14-108">Эта операция не разрешена для проверки доступа, при которой пользователи просматривают собственный доступ, и не предназначены для проверки доступа, в которой владельцы группы назначаются в качестве проверяющих.</span><span class="sxs-lookup"><span data-stu-id="36a14-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="36a14-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36a14-109">Permissions</span></span>
<span data-ttu-id="36a14-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36a14-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36a14-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36a14-112">Permission type</span></span>                        | <span data-ttu-id="36a14-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36a14-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="36a14-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36a14-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="36a14-115">Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="36a14-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="36a14-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36a14-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36a14-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36a14-117">Not supported.</span></span> |
|<span data-ttu-id="36a14-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36a14-118">Application</span></span>                            | <span data-ttu-id="36a14-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36a14-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36a14-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36a14-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a><span data-ttu-id="36a14-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36a14-121">Request headers</span></span>
| <span data-ttu-id="36a14-122">Имя</span><span class="sxs-lookup"><span data-stu-id="36a14-122">Name</span></span>         | <span data-ttu-id="36a14-123">Тип</span><span class="sxs-lookup"><span data-stu-id="36a14-123">Type</span></span>        | <span data-ttu-id="36a14-124">Описание</span><span class="sxs-lookup"><span data-stu-id="36a14-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="36a14-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="36a14-125">Authorization</span></span> | <span data-ttu-id="36a14-126">string</span><span class="sxs-lookup"><span data-stu-id="36a14-126">string</span></span> | <span data-ttu-id="36a14-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36a14-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36a14-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="36a14-129">Request body</span></span>
<span data-ttu-id="36a14-130">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="36a14-130">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="36a14-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="36a14-131">Response</span></span>
<span data-ttu-id="36a14-132">В случае успешного выполнения этот метод возвращает код ответа серии 200.</span><span class="sxs-lookup"><span data-stu-id="36a14-132">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="36a14-133">Пример</span><span class="sxs-lookup"><span data-stu-id="36a14-133">Example</span></span>

<span data-ttu-id="36a14-134">В этом примере показано, как обновить доступ к одноразовой (не возможной) проверке доступа, чтобы удалить ненужного проверяющего.</span><span class="sxs-lookup"><span data-stu-id="36a14-134">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="36a14-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="36a14-135">Request</span></span>
<span data-ttu-id="36a14-136">В URL-АДРЕСе запроса укажите идентификатор объекта Акцессревиев, а затем идентификатор объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="36a14-136">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b

```

##### <a name="response"></a><span data-ttu-id="36a14-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="36a14-137">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
