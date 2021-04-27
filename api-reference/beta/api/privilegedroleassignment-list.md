---
title: Список privilegedRoleAssignments
description: Извлечение списка объектов privilegedRoleAssignment, соответствующих всем назначениям ролей для организации.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 01ca1661045d2f6c5695ad3879beec3cf9f5bf5e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049865"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="2e094-103">Список privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="2e094-103">List privilegedRoleAssignments</span></span>

<span data-ttu-id="2e094-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e094-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e094-105">Извлечение списка [объектов privilegedRoleAssignment,](../resources/privilegedroleassignment.md) соответствующих всем назначениям ролей для организации.</span><span class="sxs-lookup"><span data-stu-id="2e094-105">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="2e094-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e094-106">Permissions</span></span>
<span data-ttu-id="2e094-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e094-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2e094-109">У запросителя должна быть одна из следующих ролей: _администратор_ привилегированных _ролей,_ глобальный _администратор,_ администратор безопасности или _читатель безопасности._</span><span class="sxs-lookup"><span data-stu-id="2e094-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="2e094-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e094-110">Permission type</span></span>      | <span data-ttu-id="2e094-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e094-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e094-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e094-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2e094-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2e094-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2e094-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e094-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e094-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e094-115">Not supported.</span></span>    |
|<span data-ttu-id="2e094-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e094-116">Application</span></span> | <span data-ttu-id="2e094-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e094-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e094-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e094-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2e094-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2e094-119">Optional query parameters</span></span>
<span data-ttu-id="2e094-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2e094-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e094-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e094-121">Request headers</span></span>
| <span data-ttu-id="2e094-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2e094-122">Name</span></span>      |<span data-ttu-id="2e094-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2e094-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2e094-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e094-124">Authorization</span></span>  | <span data-ttu-id="2e094-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e094-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e094-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e094-127">Request body</span></span>
<span data-ttu-id="2e094-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e094-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e094-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e094-129">Response</span></span>

<span data-ttu-id="2e094-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [privilegedRoleAssignment](../resources/privilegedroleassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2e094-130">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="2e094-131">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="2e094-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="2e094-132">В противном случае код запретного статуса HTTP 403 будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="2e094-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="2e094-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="2e094-133">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="2e094-134">Получить все назначения ролей</span><span class="sxs-lookup"><span data-stu-id="2e094-134">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="2e094-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e094-135">Request</span></span>
<span data-ttu-id="2e094-136">В следующем примере показан запрос на выполнение всех назначений ролей:</span><span class="sxs-lookup"><span data-stu-id="2e094-136">The following example shows a request to get all role assignments:</span></span>

# <a name="http"></a>[<span data-ttu-id="2e094-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e094-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="2e094-138">C#</span><span class="sxs-lookup"><span data-stu-id="2e094-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e094-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e094-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e094-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e094-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e094-141">Java</span><span class="sxs-lookup"><span data-stu-id="2e094-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2e094-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e094-142">Response</span></span>
<span data-ttu-id="2e094-143">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2e094-143">The following example shows the response.</span></span> <span data-ttu-id="2e094-144">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2e094-144">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```
### <a name="get-active-role-assignments"></a><span data-ttu-id="2e094-145">Получать назначения активных ролей</span><span class="sxs-lookup"><span data-stu-id="2e094-145">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="2e094-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e094-146">Request</span></span> 
<span data-ttu-id="2e094-147">В следующем примере показан запрос на запрос о назначениях активных ролей:</span><span class="sxs-lookup"><span data-stu-id="2e094-147">The following example shows a request to query active role assignments:</span></span>

# <a name="http"></a>[<span data-ttu-id="2e094-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e094-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
# <a name="c"></a>[<span data-ttu-id="2e094-149">C#</span><span class="sxs-lookup"><span data-stu-id="2e094-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e094-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e094-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e094-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e094-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e094-152">Java</span><span class="sxs-lookup"><span data-stu-id="2e094-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2e094-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e094-153">Response</span></span>
<span data-ttu-id="2e094-154">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2e094-154">The following example shows the response.</span></span> <span data-ttu-id="2e094-155">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2e094-155">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_62e90394-69f5-4237-9190-012177145e10",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "62e90394-69f5-4237-9190-012177145e10",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": true,
            "expirationDateTime": "2017-07-25T17:38:49.563Z",
            "resultMessage": null
        }
  ]
}
```
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="2e094-156">Получить постоянные назначения ролей</span><span class="sxs-lookup"><span data-stu-id="2e094-156">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="2e094-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e094-157">Request</span></span> 
<span data-ttu-id="2e094-158">В следующем примере показан запрос на запрос постоянных назначений ролей, где ``expirationDateTime`` ``null`` значение:</span><span class="sxs-lookup"><span data-stu-id="2e094-158">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>

# <a name="http"></a>[<span data-ttu-id="2e094-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e094-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
# <a name="c"></a>[<span data-ttu-id="2e094-160">C#</span><span class="sxs-lookup"><span data-stu-id="2e094-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e094-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e094-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e094-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e094-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e094-163">Java</span><span class="sxs-lookup"><span data-stu-id="2e094-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2e094-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e094-164">Response</span></span>
<span data-ttu-id="2e094-165">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2e094-165">The following example shows the response.</span></span> <span data-ttu-id="2e094-166">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2e094-166">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_194ae4cb-b126-40b2-bd5b-6091b380977d",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_44367163-eba1-44c3-98af-f5787879f96a",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "44367163-eba1-44c3-98af-f5787879f96a",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        }
  ]
}
```
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="2e094-167">Получение подходящих назначений ролей</span><span class="sxs-lookup"><span data-stu-id="2e094-167">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="2e094-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e094-168">Request</span></span> 
<span data-ttu-id="2e094-169">В следующем примере показан запрос на запрос подходящих назначений ролей, в том числе активных и неавтных:</span><span class="sxs-lookup"><span data-stu-id="2e094-169">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>

# <a name="http"></a>[<span data-ttu-id="2e094-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e094-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments_4"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
# <a name="c"></a>[<span data-ttu-id="2e094-171">C#</span><span class="sxs-lookup"><span data-stu-id="2e094-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e094-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e094-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e094-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e094-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e094-174">Java</span><span class="sxs-lookup"><span data-stu-id="2e094-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2e094-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e094-175">Response</span></span> 
<span data-ttu-id="2e094-176">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2e094-176">The following example shows the response.</span></span> <span data-ttu-id="2e094-177">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2e094-177">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": true,
            "expirationDateTime": "2017-07-25T18:42:26.823Z",
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_194ae4cb-b126-40b2-bd5b-6091b380977d",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_9360feb5-f418-4baa-8175-e2a00bac4301",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "9360feb5-f418-4baa-8175-e2a00bac4301",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
