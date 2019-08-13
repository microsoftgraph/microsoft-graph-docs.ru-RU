---
title: 'Привилежедроле: Селфактивате'
description: Активируйте роль, назначенную инициатору запроса.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7fbe9b8a0f37238c393d5c9848b578263b5318ae
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361251"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="cc062-103">Привилежедроле: Селфактивате</span><span class="sxs-lookup"><span data-stu-id="cc062-103">privilegedRole: selfActivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc062-104">Активируйте роль, назначенную инициатору запроса.</span><span class="sxs-lookup"><span data-stu-id="cc062-104">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="cc062-105">**Примечание:** Эффективный 2018 декабря этот API больше не поддерживается и не должен использоваться.</span><span class="sxs-lookup"><span data-stu-id="cc062-105">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="cc062-106">Используйте вместо этого [CREATE привилежедролеассигнментрекуест](privilegedroleassignmentrequest-post.md) .</span><span class="sxs-lookup"><span data-stu-id="cc062-106">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="cc062-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc062-107">Permissions</span></span>
<span data-ttu-id="cc062-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc062-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="cc062-110">Запрашивающая сторона может вызвать ```selfActivate``` только назначенную ему роль.</span><span class="sxs-lookup"><span data-stu-id="cc062-110">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="cc062-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc062-111">Permission type</span></span>      | <span data-ttu-id="cc062-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc062-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc062-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc062-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cc062-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cc062-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cc062-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc062-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc062-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc062-116">Not supported.</span></span>    |
|<span data-ttu-id="cc062-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc062-117">Application</span></span> | <span data-ttu-id="cc062-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc062-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc062-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc062-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="cc062-120">Обратите ``<id>`` внимание, что это идентификатор целевой роли.</span><span class="sxs-lookup"><span data-stu-id="cc062-120">Note that ``<id>`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cc062-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc062-121">Request headers</span></span>
| <span data-ttu-id="cc062-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cc062-122">Name</span></span>       | <span data-ttu-id="cc062-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cc062-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cc062-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc062-124">Authorization</span></span>  | <span data-ttu-id="cc062-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc062-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc062-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cc062-127">Request body</span></span>
<span data-ttu-id="cc062-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="cc062-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cc062-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="cc062-129">Parameter</span></span>    | <span data-ttu-id="cc062-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cc062-130">Type</span></span>   |<span data-ttu-id="cc062-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cc062-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc062-132">причиной</span><span class="sxs-lookup"><span data-stu-id="cc062-132">reason</span></span>|<span data-ttu-id="cc062-133">string</span><span class="sxs-lookup"><span data-stu-id="cc062-133">string</span></span>|<span data-ttu-id="cc062-134">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="cc062-134">Optional.</span></span> <span data-ttu-id="cc062-135">Описание причины активации этой роли.</span><span class="sxs-lookup"><span data-stu-id="cc062-135">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="cc062-136">duration</span><span class="sxs-lookup"><span data-stu-id="cc062-136">duration</span></span>|<span data-ttu-id="cc062-137">string</span><span class="sxs-lookup"><span data-stu-id="cc062-137">string</span></span>|<span data-ttu-id="cc062-138">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="cc062-138">Optional.</span></span> <span data-ttu-id="cc062-139">Допустимые значения ```min``` : (минимальная длительность активации), ```default``` (длительность активации по умолчанию для роли) или значение Double, определяющее количество часов активации.</span><span class="sxs-lookup"><span data-stu-id="cc062-139">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="cc062-140">Указанное время не может быть длиннее, чем длительность активации роли из параметра Role.</span><span class="sxs-lookup"><span data-stu-id="cc062-140">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="cc062-141">тиккетнумбер</span><span class="sxs-lookup"><span data-stu-id="cc062-141">ticketNumber</span></span>|<span data-ttu-id="cc062-142">string</span><span class="sxs-lookup"><span data-stu-id="cc062-142">string</span></span>|<span data-ttu-id="cc062-143">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="cc062-143">Optional.</span></span> <span data-ttu-id="cc062-144">Номер билета, который используется для отслеживания активации этой роли.</span><span class="sxs-lookup"><span data-stu-id="cc062-144">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="cc062-145">тиккетсистем</span><span class="sxs-lookup"><span data-stu-id="cc062-145">ticketSystem</span></span>|<span data-ttu-id="cc062-146">string</span><span class="sxs-lookup"><span data-stu-id="cc062-146">string</span></span>|<span data-ttu-id="cc062-147">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="cc062-147">Optional.</span></span> <span data-ttu-id="cc062-148">Система билетов.</span><span class="sxs-lookup"><span data-stu-id="cc062-148">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="cc062-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc062-149">Response</span></span>

<span data-ttu-id="cc062-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cc062-150">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="cc062-151">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="cc062-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="cc062-152">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="cc062-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="cc062-153">Пример</span><span class="sxs-lookup"><span data-stu-id="cc062-153">Example</span></span>
<span data-ttu-id="cc062-154">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="cc062-154">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cc062-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc062-155">Request</span></span>
<span data-ttu-id="cc062-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc062-156">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cc062-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc062-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfActivate
Content-type: application/json
Content-length: 142

{
  "reason": "reason-value",
  "duration": "duration-value",
  "ticketNumber": "ticketNumber-value",
  "ticketSystem": "ticketSystem-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cc062-158">C#</span><span class="sxs-lookup"><span data-stu-id="cc062-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cc062-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc062-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cc062-160">Цель — C</span><span class="sxs-lookup"><span data-stu-id="cc062-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cc062-161">Java</span><span class="sxs-lookup"><span data-stu-id="cc062-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedrole-selfactivate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cc062-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc062-162">Response</span></span>
<span data-ttu-id="cc062-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc062-163">Here is an example of the response.</span></span> 

><span data-ttu-id="cc062-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc062-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole: selfActivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
