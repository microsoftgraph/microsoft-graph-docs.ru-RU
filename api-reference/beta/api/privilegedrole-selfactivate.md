---
title: 'Привилежедроле: Селфактивате'
description: Активируйте роль, назначенную инициатору запроса.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 1beddad763dbe4f7d70ffeeeef0c5131f6df1157
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035108"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="7b69b-103">Привилежедроле: Селфактивате</span><span class="sxs-lookup"><span data-stu-id="7b69b-103">privilegedRole: selfActivate</span></span>

<span data-ttu-id="7b69b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b69b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b69b-105">Активируйте роль, назначенную инициатору запроса.</span><span class="sxs-lookup"><span data-stu-id="7b69b-105">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="7b69b-106">**Примечание:** Эффективный 2018 декабря этот API больше не поддерживается и не должен использоваться.</span><span class="sxs-lookup"><span data-stu-id="7b69b-106">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="7b69b-107">Используйте вместо этого [CREATE привилежедролеассигнментрекуест](privilegedroleassignmentrequest-post.md) .</span><span class="sxs-lookup"><span data-stu-id="7b69b-107">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="7b69b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b69b-108">Permissions</span></span>
<span data-ttu-id="7b69b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b69b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7b69b-111">Запрашивающая сторона может вызвать только ```selfActivate``` назначенную ему роль.</span><span class="sxs-lookup"><span data-stu-id="7b69b-111">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="7b69b-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b69b-112">Permission type</span></span>      | <span data-ttu-id="7b69b-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b69b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b69b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b69b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7b69b-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7b69b-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7b69b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b69b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b69b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b69b-117">Not supported.</span></span>    |
|<span data-ttu-id="7b69b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b69b-118">Application</span></span> | <span data-ttu-id="7b69b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b69b-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b69b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b69b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="7b69b-121">Обратите внимание, что ``{id}`` это идентификатор целевой роли.</span><span class="sxs-lookup"><span data-stu-id="7b69b-121">Note that ``{id}`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7b69b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b69b-122">Request headers</span></span>
| <span data-ttu-id="7b69b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="7b69b-123">Name</span></span>       | <span data-ttu-id="7b69b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7b69b-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7b69b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b69b-125">Authorization</span></span>  | <span data-ttu-id="7b69b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b69b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b69b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b69b-128">Request body</span></span>
<span data-ttu-id="7b69b-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7b69b-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7b69b-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="7b69b-130">Parameter</span></span>    | <span data-ttu-id="7b69b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7b69b-131">Type</span></span>   |<span data-ttu-id="7b69b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7b69b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b69b-133">reason</span><span class="sxs-lookup"><span data-stu-id="7b69b-133">reason</span></span>|<span data-ttu-id="7b69b-134">string</span><span class="sxs-lookup"><span data-stu-id="7b69b-134">string</span></span>|<span data-ttu-id="7b69b-135">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="7b69b-135">Optional.</span></span> <span data-ttu-id="7b69b-136">Описание причины активации этой роли.</span><span class="sxs-lookup"><span data-stu-id="7b69b-136">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="7b69b-137">duration</span><span class="sxs-lookup"><span data-stu-id="7b69b-137">duration</span></span>|<span data-ttu-id="7b69b-138">string</span><span class="sxs-lookup"><span data-stu-id="7b69b-138">string</span></span>|<span data-ttu-id="7b69b-139">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="7b69b-139">Optional.</span></span> <span data-ttu-id="7b69b-140">Допустимые значения ```min``` : (минимальная длительность активации), ```default``` (длительность активации по умолчанию для роли) или значение Double, определяющее количество часов активации.</span><span class="sxs-lookup"><span data-stu-id="7b69b-140">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="7b69b-141">Указанное время не может быть длиннее, чем длительность активации роли из параметра Role.</span><span class="sxs-lookup"><span data-stu-id="7b69b-141">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="7b69b-142">тиккетнумбер</span><span class="sxs-lookup"><span data-stu-id="7b69b-142">ticketNumber</span></span>|<span data-ttu-id="7b69b-143">string</span><span class="sxs-lookup"><span data-stu-id="7b69b-143">string</span></span>|<span data-ttu-id="7b69b-144">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="7b69b-144">Optional.</span></span> <span data-ttu-id="7b69b-145">Номер билета, который используется для отслеживания активации этой роли.</span><span class="sxs-lookup"><span data-stu-id="7b69b-145">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="7b69b-146">тиккетсистем</span><span class="sxs-lookup"><span data-stu-id="7b69b-146">ticketSystem</span></span>|<span data-ttu-id="7b69b-147">string</span><span class="sxs-lookup"><span data-stu-id="7b69b-147">string</span></span>|<span data-ttu-id="7b69b-148">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="7b69b-148">Optional.</span></span> <span data-ttu-id="7b69b-149">Система билетов.</span><span class="sxs-lookup"><span data-stu-id="7b69b-149">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="7b69b-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b69b-150">Response</span></span>

<span data-ttu-id="7b69b-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7b69b-151">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="7b69b-152">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="7b69b-152">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="7b69b-153">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="7b69b-153">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="7b69b-154">Пример</span><span class="sxs-lookup"><span data-stu-id="7b69b-154">Example</span></span>
<span data-ttu-id="7b69b-155">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="7b69b-155">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7b69b-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b69b-156">Request</span></span>
<span data-ttu-id="7b69b-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b69b-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7b69b-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b69b-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7b69b-159">C#</span><span class="sxs-lookup"><span data-stu-id="7b69b-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b69b-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b69b-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b69b-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b69b-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7b69b-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b69b-162">Response</span></span>
<span data-ttu-id="7b69b-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7b69b-163">Here is an example of the response.</span></span> 

><span data-ttu-id="7b69b-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b69b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


