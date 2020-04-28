---
title: Список Привилежедролеассигнментс
description: Получение списка объектов Привилежедролеассигнмент, соответствующих всем назначениям ролей для Организации.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 4baf83cd05010a179fe47c86e949f2bd6aa70f16
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218726"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="f7964-103">Список Привилежедролеассигнментс</span><span class="sxs-lookup"><span data-stu-id="f7964-103">List privilegedRoleAssignments</span></span>

<span data-ttu-id="f7964-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7964-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7964-105">Получение списка объектов [привилежедролеассигнмент](../resources/privilegedroleassignment.md) , соответствующих всем назначениям ролей для Организации.</span><span class="sxs-lookup"><span data-stu-id="f7964-105">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="f7964-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7964-106">Permissions</span></span>
<span data-ttu-id="f7964-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f7964-109">Запрашивающая сторона должна иметь одну из следующих ролей: _привилегированный администратор ролей_, _глобальный администратор_, _администратор безопасности_или _средство чтения безопасности_.</span><span class="sxs-lookup"><span data-stu-id="f7964-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="f7964-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7964-110">Permission type</span></span>      | <span data-ttu-id="f7964-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7964-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7964-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7964-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f7964-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f7964-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f7964-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7964-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7964-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7964-115">Not supported.</span></span>    |
|<span data-ttu-id="f7964-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7964-116">Application</span></span> | <span data-ttu-id="f7964-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7964-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7964-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7964-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f7964-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f7964-119">Optional query parameters</span></span>
<span data-ttu-id="f7964-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f7964-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7964-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7964-121">Request headers</span></span>
| <span data-ttu-id="f7964-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f7964-122">Name</span></span>      |<span data-ttu-id="f7964-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f7964-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f7964-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7964-124">Authorization</span></span>  | <span data-ttu-id="f7964-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7964-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7964-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f7964-127">Request body</span></span>
<span data-ttu-id="f7964-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7964-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7964-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7964-129">Response</span></span>

<span data-ttu-id="f7964-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7964-130">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="f7964-131">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="f7964-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="f7964-132">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="f7964-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="f7964-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="f7964-133">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="f7964-134">Получение всех назначений ролей</span><span class="sxs-lookup"><span data-stu-id="f7964-134">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="f7964-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7964-135">Request</span></span>
<span data-ttu-id="f7964-136">В приведенном ниже примере показан запрос на получение всех назначений ролей:</span><span class="sxs-lookup"><span data-stu-id="f7964-136">The following example shows a request to get all role assignments:</span></span>

# <a name="http"></a>[<span data-ttu-id="f7964-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7964-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="f7964-138">C#</span><span class="sxs-lookup"><span data-stu-id="f7964-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7964-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7964-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7964-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7964-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f7964-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7964-141">Response</span></span>
<span data-ttu-id="f7964-142">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7964-142">The following example shows the response.</span></span> <span data-ttu-id="f7964-143">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="f7964-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f7964-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7964-144">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-active-role-assignments"></a><span data-ttu-id="f7964-145">Получение активных назначений ролей</span><span class="sxs-lookup"><span data-stu-id="f7964-145">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="f7964-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7964-146">Request</span></span> 
<span data-ttu-id="f7964-147">В приведенном ниже примере показан запрос на запросы о назначениях активных ролей.</span><span class="sxs-lookup"><span data-stu-id="f7964-147">The following example shows a request to query active role assignments:</span></span>

# <a name="http"></a>[<span data-ttu-id="f7964-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7964-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
# <a name="c"></a>[<span data-ttu-id="f7964-149">C#</span><span class="sxs-lookup"><span data-stu-id="f7964-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7964-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7964-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7964-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7964-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f7964-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7964-152">Response</span></span>
<span data-ttu-id="f7964-153">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7964-153">The following example shows the response.</span></span> <span data-ttu-id="f7964-154">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="f7964-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f7964-155">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7964-155">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="f7964-156">Получение постоянных назначений ролей</span><span class="sxs-lookup"><span data-stu-id="f7964-156">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="f7964-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7964-157">Request</span></span> 
<span data-ttu-id="f7964-158">В приведенном ниже примере показан запрос на запрос постоянных назначений ролей ``expirationDateTime`` , где ``null``значение:</span><span class="sxs-lookup"><span data-stu-id="f7964-158">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>

# <a name="http"></a>[<span data-ttu-id="f7964-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7964-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
# <a name="c"></a>[<span data-ttu-id="f7964-160">C#</span><span class="sxs-lookup"><span data-stu-id="f7964-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7964-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7964-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7964-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7964-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f7964-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7964-163">Response</span></span>
<span data-ttu-id="f7964-164">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7964-164">The following example shows the response.</span></span> <span data-ttu-id="f7964-165">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="f7964-165">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f7964-166">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7964-166">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="f7964-167">Получение подходящих назначений ролей</span><span class="sxs-lookup"><span data-stu-id="f7964-167">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="f7964-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7964-168">Request</span></span> 
<span data-ttu-id="f7964-169">В приведенном ниже примере показан запрос на запросы о подходящих назначениях ролей, включая активные и неактивные.</span><span class="sxs-lookup"><span data-stu-id="f7964-169">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>

# <a name="http"></a>[<span data-ttu-id="f7964-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7964-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
# <a name="c"></a>[<span data-ttu-id="f7964-171">C#</span><span class="sxs-lookup"><span data-stu-id="f7964-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7964-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7964-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7964-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7964-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f7964-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7964-174">Response</span></span> 
<span data-ttu-id="f7964-175">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7964-175">The following example shows the response.</span></span> <span data-ttu-id="f7964-176">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="f7964-176">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f7964-177">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7964-177">All of the properties will be returned from an actual call.</span></span>
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
