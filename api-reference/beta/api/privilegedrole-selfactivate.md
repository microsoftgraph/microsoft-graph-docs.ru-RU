---
title: 'privilegedRole: selfActivate'
description: Активируйте роль, назначенную запрашиваемой.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 45aea40e3fcdf2d9aff1590636411afdfb8cc4b1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441318"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="12437-103">privilegedRole: selfActivate</span><span class="sxs-lookup"><span data-stu-id="12437-103">privilegedRole: selfActivate</span></span>

<span data-ttu-id="12437-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12437-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12437-105">Активируйте роль, назначенную запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="12437-105">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="12437-106">**Примечание:** С декабря 2018 г. этот API больше не будет поддерживаться и не должен использоваться.</span><span class="sxs-lookup"><span data-stu-id="12437-106">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="12437-107">Вместо этого [используйте create PrivilegedRoleAssignmentRequest.](privilegedroleassignmentrequest-post.md)</span><span class="sxs-lookup"><span data-stu-id="12437-107">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="12437-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12437-108">Permissions</span></span>
<span data-ttu-id="12437-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12437-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="12437-111">Запросчик может вызывать только назначенную ему ```selfActivate``` роль.</span><span class="sxs-lookup"><span data-stu-id="12437-111">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="12437-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12437-112">Permission type</span></span>      | <span data-ttu-id="12437-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12437-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12437-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12437-114">Delegated (work or school account)</span></span> | <span data-ttu-id="12437-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="12437-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="12437-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12437-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12437-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12437-117">Not supported.</span></span>    |
|<span data-ttu-id="12437-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12437-118">Application</span></span> | <span data-ttu-id="12437-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12437-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12437-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12437-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="12437-121">Обратите ``{id}`` внимание, что это ИД целевой роли.</span><span class="sxs-lookup"><span data-stu-id="12437-121">Note that ``{id}`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="12437-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12437-122">Request headers</span></span>
| <span data-ttu-id="12437-123">Имя</span><span class="sxs-lookup"><span data-stu-id="12437-123">Name</span></span>       | <span data-ttu-id="12437-124">Описание</span><span class="sxs-lookup"><span data-stu-id="12437-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="12437-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12437-125">Authorization</span></span>  | <span data-ttu-id="12437-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12437-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12437-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="12437-128">Request body</span></span>
<span data-ttu-id="12437-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="12437-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="12437-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="12437-130">Parameter</span></span>    | <span data-ttu-id="12437-131">Тип</span><span class="sxs-lookup"><span data-stu-id="12437-131">Type</span></span>   |<span data-ttu-id="12437-132">Описание</span><span class="sxs-lookup"><span data-stu-id="12437-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12437-133">reason</span><span class="sxs-lookup"><span data-stu-id="12437-133">reason</span></span>|<span data-ttu-id="12437-134">string</span><span class="sxs-lookup"><span data-stu-id="12437-134">string</span></span>|<span data-ttu-id="12437-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="12437-135">Optional.</span></span> <span data-ttu-id="12437-136">Описание причины активации этой роли.</span><span class="sxs-lookup"><span data-stu-id="12437-136">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="12437-137">duration</span><span class="sxs-lookup"><span data-stu-id="12437-137">duration</span></span>|<span data-ttu-id="12437-138">string</span><span class="sxs-lookup"><span data-stu-id="12437-138">string</span></span>|<span data-ttu-id="12437-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="12437-139">Optional.</span></span> <span data-ttu-id="12437-140">Допустимые значения могут быть (минимальная продолжительность активации), (продолжительность активации по умолчанию для роли) или двойное значение, чтобы указать, сколько часов ```min``` ```default``` является активацией.</span><span class="sxs-lookup"><span data-stu-id="12437-140">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="12437-141">Указанная продолжительность не может быть больше, чем продолжительность активации роли из параметра роли.</span><span class="sxs-lookup"><span data-stu-id="12437-141">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="12437-142">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="12437-142">ticketNumber</span></span>|<span data-ttu-id="12437-143">string</span><span class="sxs-lookup"><span data-stu-id="12437-143">string</span></span>|<span data-ttu-id="12437-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="12437-144">Optional.</span></span> <span data-ttu-id="12437-145">Номер билета, используемый для отслеживания активации этой роли.</span><span class="sxs-lookup"><span data-stu-id="12437-145">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="12437-146">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="12437-146">ticketSystem</span></span>|<span data-ttu-id="12437-147">string</span><span class="sxs-lookup"><span data-stu-id="12437-147">string</span></span>|<span data-ttu-id="12437-148">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="12437-148">Optional.</span></span> <span data-ttu-id="12437-149">Система билетов.</span><span class="sxs-lookup"><span data-stu-id="12437-149">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="12437-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="12437-150">Response</span></span>

<span data-ttu-id="12437-151">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [privilegedRoleAssignment](../resources/privilegedroleassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="12437-151">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="12437-152">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="12437-152">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="12437-153">В противном случае код запретного статуса HTTP 403 будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="12437-153">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="12437-154">Пример</span><span class="sxs-lookup"><span data-stu-id="12437-154">Example</span></span>
<span data-ttu-id="12437-155">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="12437-155">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="12437-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="12437-156">Request</span></span>
<span data-ttu-id="12437-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12437-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="12437-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="12437-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="12437-159">C#</span><span class="sxs-lookup"><span data-stu-id="12437-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12437-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12437-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12437-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12437-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12437-162">Java</span><span class="sxs-lookup"><span data-stu-id="12437-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedrole-selfactivate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="12437-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="12437-163">Response</span></span>
<span data-ttu-id="12437-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="12437-164">Here is an example of the response.</span></span> 

><span data-ttu-id="12437-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12437-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


