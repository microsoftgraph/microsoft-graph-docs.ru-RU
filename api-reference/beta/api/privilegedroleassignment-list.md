---
title: Список Привилежедролеассигнментс
description: Получение списка объектов Привилежедролеассигнмент, соответствующих всем назначениям ролей для Организации.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 31bbf6221c4d8b9fc021aabd8678acb7c64b74a2
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412735"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="3795b-103">Список Привилежедролеассигнментс</span><span class="sxs-lookup"><span data-stu-id="3795b-103">List privilegedRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3795b-104">Получение списка объектов [привилежедролеассигнмент](../resources/privilegedroleassignment.md) , соответствующих всем назначениям ролей для Организации.</span><span class="sxs-lookup"><span data-stu-id="3795b-104">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="3795b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3795b-105">Permissions</span></span>
<span data-ttu-id="3795b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3795b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3795b-108">Запрашивающая сторона должна иметь одну из следующих ролей: привилегированный _Администратор ролей_, _глобальный администратор_, _администратор безопасности_или _средство чтения безопасности_.</span><span class="sxs-lookup"><span data-stu-id="3795b-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="3795b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3795b-109">Permission type</span></span>      | <span data-ttu-id="3795b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3795b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3795b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3795b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3795b-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3795b-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3795b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3795b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3795b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3795b-114">Not supported.</span></span>    |
|<span data-ttu-id="3795b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3795b-115">Application</span></span> | <span data-ttu-id="3795b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3795b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3795b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3795b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3795b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3795b-118">Optional query parameters</span></span>
<span data-ttu-id="3795b-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3795b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3795b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3795b-120">Request headers</span></span>
| <span data-ttu-id="3795b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3795b-121">Name</span></span>      |<span data-ttu-id="3795b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3795b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3795b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3795b-123">Authorization</span></span>  | <span data-ttu-id="3795b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3795b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3795b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3795b-126">Request body</span></span>
<span data-ttu-id="3795b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3795b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3795b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3795b-128">Response</span></span>

<span data-ttu-id="3795b-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3795b-129">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="3795b-130">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="3795b-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="3795b-131">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="3795b-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="3795b-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="3795b-132">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="3795b-133">Получение всех назначений ролей</span><span class="sxs-lookup"><span data-stu-id="3795b-133">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="3795b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3795b-134">Request</span></span>
<span data-ttu-id="3795b-135">В приведенном ниже примере показан запрос на получение всех назначений ролей:</span><span class="sxs-lookup"><span data-stu-id="3795b-135">The following example shows a request to get all role assignments:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3795b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3795b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3795b-137">C#</span><span class="sxs-lookup"><span data-stu-id="3795b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3795b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3795b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3795b-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3795b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3795b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3795b-140">Response</span></span>
<span data-ttu-id="3795b-141">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3795b-141">The following example shows the response.</span></span> <span data-ttu-id="3795b-142">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="3795b-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3795b-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3795b-143">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-active-role-assignments"></a><span data-ttu-id="3795b-144">Получение активных назначений ролей</span><span class="sxs-lookup"><span data-stu-id="3795b-144">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="3795b-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="3795b-145">Request</span></span> 
<span data-ttu-id="3795b-146">В приведенном ниже примере показан запрос на запросы о назначениях активных ролей.</span><span class="sxs-lookup"><span data-stu-id="3795b-146">The following example shows a request to query active role assignments:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3795b-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="3795b-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3795b-148">C#</span><span class="sxs-lookup"><span data-stu-id="3795b-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3795b-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3795b-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3795b-150">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3795b-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3795b-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="3795b-151">Response</span></span>
<span data-ttu-id="3795b-152">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3795b-152">The following example shows the response.</span></span> <span data-ttu-id="3795b-153">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="3795b-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3795b-154">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3795b-154">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="3795b-155">Получение постоянных назначений ролей</span><span class="sxs-lookup"><span data-stu-id="3795b-155">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="3795b-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="3795b-156">Request</span></span> 
<span data-ttu-id="3795b-157">В приведенном ниже примере показан запрос на запрос постоянных назначений ролей ``expirationDateTime`` , где ``null``значение:</span><span class="sxs-lookup"><span data-stu-id="3795b-157">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3795b-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="3795b-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3795b-159">C#</span><span class="sxs-lookup"><span data-stu-id="3795b-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3795b-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3795b-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3795b-161">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3795b-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3795b-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="3795b-162">Response</span></span>
<span data-ttu-id="3795b-163">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3795b-163">The following example shows the response.</span></span> <span data-ttu-id="3795b-164">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="3795b-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3795b-165">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3795b-165">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="3795b-166">Получение подходящих назначений ролей</span><span class="sxs-lookup"><span data-stu-id="3795b-166">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="3795b-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="3795b-167">Request</span></span> 
<span data-ttu-id="3795b-168">В приведенном ниже примере показан запрос на запросы о подходящих назначениях ролей, включая активные и неактивные.</span><span class="sxs-lookup"><span data-stu-id="3795b-168">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3795b-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="3795b-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3795b-170">C#</span><span class="sxs-lookup"><span data-stu-id="3795b-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3795b-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3795b-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3795b-172">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3795b-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3795b-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="3795b-173">Response</span></span> 
<span data-ttu-id="3795b-174">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3795b-174">The following example shows the response.</span></span> <span data-ttu-id="3795b-175">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="3795b-175">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3795b-176">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3795b-176">All of the properties will be returned from an actual call.</span></span>
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
