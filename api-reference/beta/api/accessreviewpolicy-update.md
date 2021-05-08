---
title: Обновление accessReviewPolicy
description: Обновление свойств объекта accessReviewPolicy.
author: kafen
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: cd774e18586218182379a0523df304a20a8e7e7c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240650"
---
# <a name="update-accessreviewpolicy"></a><span data-ttu-id="f7a88-103">Обновление accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="f7a88-103">Update accessReviewPolicy</span></span>
<span data-ttu-id="f7a88-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7a88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7a88-105">Обновление свойств объекта [accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f7a88-105">Update the properties of an [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7a88-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7a88-106">Permissions</span></span>
<span data-ttu-id="f7a88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7a88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7a88-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7a88-109">Permission type</span></span>|<span data-ttu-id="f7a88-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7a88-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7a88-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7a88-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f7a88-112">Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="f7a88-112">Policy.ReadWrite.AccessReviews</span></span>|
|<span data-ttu-id="f7a88-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7a88-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7a88-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7a88-114">Not supported.</span></span>|
|<span data-ttu-id="f7a88-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7a88-115">Application</span></span>|<span data-ttu-id="f7a88-116">Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="f7a88-116">Policy.ReadWrite.AccessReviews</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7a88-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7a88-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/accessReviewPolicy
PATCH /identityGovernance/accessReviews/policy
```

## <a name="request-headers"></a><span data-ttu-id="f7a88-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7a88-118">Request headers</span></span>
|<span data-ttu-id="f7a88-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f7a88-119">Name</span></span>|<span data-ttu-id="f7a88-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f7a88-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f7a88-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7a88-121">Authorization</span></span>|<span data-ttu-id="f7a88-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7a88-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f7a88-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7a88-124">Content-Type</span></span>|<span data-ttu-id="f7a88-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7a88-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7a88-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7a88-127">Request body</span></span>
<span data-ttu-id="f7a88-128">В теле запроса поставляем представление JSON объекта [accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f7a88-128">In the request body, supply a JSON representation of the [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>

<span data-ttu-id="f7a88-129">В следующей таблице показаны свойства, необходимые при обновлении [accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f7a88-129">The following table shows the properties that are required when you update the [accessReviewPolicy](../resources/accessreviewpolicy.md).</span></span>

|<span data-ttu-id="f7a88-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7a88-130">Property</span></span>|<span data-ttu-id="f7a88-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f7a88-131">Type</span></span>|<span data-ttu-id="f7a88-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f7a88-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7a88-133">isGroupOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="f7a88-133">isGroupOwnerManagementEnabled</span></span>|<span data-ttu-id="f7a88-134">Логический</span><span class="sxs-lookup"><span data-stu-id="f7a88-134">Boolean</span></span>|<span data-ttu-id="f7a88-135">Если `true` владельцы групп могут создавать и управлять отзывами доступа в группах, которые им принадлежат.</span><span class="sxs-lookup"><span data-stu-id="f7a88-135">If `true`, group owners can create and manage access reviews on groups they own.</span></span>|



## <a name="response"></a><span data-ttu-id="f7a88-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7a88-136">Response</span></span>

<span data-ttu-id="f7a88-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f7a88-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f7a88-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="f7a88-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7a88-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7a88-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f7a88-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7a88-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessreviewpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/accessReviewPolicy
Content-Type: application/json

{
  "isGroupOwnerManagementEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="f7a88-141">C#</span><span class="sxs-lookup"><span data-stu-id="f7a88-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7a88-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7a88-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7a88-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7a88-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7a88-144">Java</span><span class="sxs-lookup"><span data-stu-id="f7a88-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f7a88-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7a88-145">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="request"></a><span data-ttu-id="f7a88-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7a88-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f7a88-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7a88-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessreviewpolicy_2"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/accessReviews/policy
Content-Type: application/json

{
  "isGroupOwnerManagementEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="f7a88-148">C#</span><span class="sxs-lookup"><span data-stu-id="f7a88-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewpolicy-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7a88-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7a88-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewpolicy-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7a88-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7a88-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewpolicy-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7a88-151">Java</span><span class="sxs-lookup"><span data-stu-id="f7a88-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewpolicy-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f7a88-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7a88-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
