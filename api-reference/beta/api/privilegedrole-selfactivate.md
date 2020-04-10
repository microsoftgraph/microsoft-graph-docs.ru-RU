---
title: 'Привилежедроле: Селфактивате'
description: Активируйте роль, назначенную инициатору запроса.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 79891be7aa63269cb0d1f96393756f9d41d046d0
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218754"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="0c2f9-103">Привилежедроле: Селфактивате</span><span class="sxs-lookup"><span data-stu-id="0c2f9-103">privilegedRole: selfActivate</span></span>

<span data-ttu-id="0c2f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c2f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c2f9-105">Активируйте роль, назначенную инициатору запроса.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-105">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="0c2f9-106">**Примечание:** Эффективный 2018 декабря этот API больше не поддерживается и не должен использоваться.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-106">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="0c2f9-107">Используйте вместо этого [CREATE привилежедролеассигнментрекуест](privilegedroleassignmentrequest-post.md) .</span><span class="sxs-lookup"><span data-stu-id="0c2f9-107">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="0c2f9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c2f9-108">Permissions</span></span>
<span data-ttu-id="0c2f9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c2f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0c2f9-111">Запрашивающая сторона может вызвать ```selfActivate``` только назначенную ему роль.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-111">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="0c2f9-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c2f9-112">Permission type</span></span>      | <span data-ttu-id="0c2f9-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c2f9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c2f9-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c2f9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0c2f9-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0c2f9-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0c2f9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c2f9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c2f9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-117">Not supported.</span></span>    |
|<span data-ttu-id="0c2f9-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c2f9-118">Application</span></span> | <span data-ttu-id="0c2f9-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c2f9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c2f9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="0c2f9-121">Обратите ``{id}`` внимание, что это идентификатор целевой роли.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-121">Note that ``{id}`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0c2f9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c2f9-122">Request headers</span></span>
| <span data-ttu-id="0c2f9-123">Имя</span><span class="sxs-lookup"><span data-stu-id="0c2f9-123">Name</span></span>       | <span data-ttu-id="0c2f9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0c2f9-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0c2f9-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c2f9-125">Authorization</span></span>  | <span data-ttu-id="0c2f9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c2f9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c2f9-128">Request body</span></span>
<span data-ttu-id="0c2f9-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0c2f9-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="0c2f9-130">Parameter</span></span>    | <span data-ttu-id="0c2f9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0c2f9-131">Type</span></span>   |<span data-ttu-id="0c2f9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0c2f9-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c2f9-133">reason</span><span class="sxs-lookup"><span data-stu-id="0c2f9-133">reason</span></span>|<span data-ttu-id="0c2f9-134">string</span><span class="sxs-lookup"><span data-stu-id="0c2f9-134">string</span></span>|<span data-ttu-id="0c2f9-135">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-135">Optional.</span></span> <span data-ttu-id="0c2f9-136">Описание причины активации этой роли.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-136">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="0c2f9-137">duration</span><span class="sxs-lookup"><span data-stu-id="0c2f9-137">duration</span></span>|<span data-ttu-id="0c2f9-138">string</span><span class="sxs-lookup"><span data-stu-id="0c2f9-138">string</span></span>|<span data-ttu-id="0c2f9-139">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-139">Optional.</span></span> <span data-ttu-id="0c2f9-140">Допустимые значения ```min``` : (минимальная длительность активации), ```default``` (длительность активации по умолчанию для роли) или значение Double, определяющее количество часов активации.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-140">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="0c2f9-141">Указанное время не может быть длиннее, чем длительность активации роли из параметра Role.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-141">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="0c2f9-142">тиккетнумбер</span><span class="sxs-lookup"><span data-stu-id="0c2f9-142">ticketNumber</span></span>|<span data-ttu-id="0c2f9-143">string</span><span class="sxs-lookup"><span data-stu-id="0c2f9-143">string</span></span>|<span data-ttu-id="0c2f9-144">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-144">Optional.</span></span> <span data-ttu-id="0c2f9-145">Номер билета, который используется для отслеживания активации этой роли.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-145">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="0c2f9-146">тиккетсистем</span><span class="sxs-lookup"><span data-stu-id="0c2f9-146">ticketSystem</span></span>|<span data-ttu-id="0c2f9-147">string</span><span class="sxs-lookup"><span data-stu-id="0c2f9-147">string</span></span>|<span data-ttu-id="0c2f9-148">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-148">Optional.</span></span> <span data-ttu-id="0c2f9-149">Система билетов.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-149">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="0c2f9-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c2f9-150">Response</span></span>

<span data-ttu-id="0c2f9-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-151">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="0c2f9-152">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-152">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="0c2f9-153">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-153">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="0c2f9-154">Пример</span><span class="sxs-lookup"><span data-stu-id="0c2f9-154">Example</span></span>
<span data-ttu-id="0c2f9-155">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-155">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0c2f9-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c2f9-156">Request</span></span>
<span data-ttu-id="0c2f9-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0c2f9-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c2f9-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0c2f9-159">C#</span><span class="sxs-lookup"><span data-stu-id="0c2f9-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c2f9-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c2f9-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c2f9-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c2f9-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0c2f9-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c2f9-162">Response</span></span>
<span data-ttu-id="0c2f9-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-163">Here is an example of the response.</span></span> 

><span data-ttu-id="0c2f9-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c2f9-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
