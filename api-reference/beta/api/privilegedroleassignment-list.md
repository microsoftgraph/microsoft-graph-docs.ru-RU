---
title: Список privilegedRoleAssignments
description: Получение списка privilegedRoleAssignment объекты, которые соответствуют все назначения ролей для организации.
ms.openlocfilehash: 7642768348e2fff43f52c6865cabf85aa16ef893
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080825"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="8aa0c-103">Список privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="8aa0c-103">List privilegedRoleAssignments</span></span>

> <span data-ttu-id="8aa0c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8aa0c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8aa0c-106">Получение списка [privilegedRoleAssignment](../resources/privilegedroleassignment.md) объекты, которые соответствуют все назначения ролей для организации.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-106">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="8aa0c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8aa0c-107">Permissions</span></span>
<span data-ttu-id="8aa0c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8aa0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8aa0c-110">Запросившая сторона должен иметь одно из следующих ролей: _Привилегированной роль администратора_, _Глобального администратора_, _Администратора безопасности_или _Безопасности чтения_.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="8aa0c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8aa0c-111">Permission type</span></span>      | <span data-ttu-id="8aa0c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8aa0c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8aa0c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8aa0c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8aa0c-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8aa0c-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8aa0c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8aa0c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8aa0c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-116">Not supported.</span></span>    |
|<span data-ttu-id="8aa0c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8aa0c-117">Application</span></span> | <span data-ttu-id="8aa0c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8aa0c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8aa0c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8aa0c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8aa0c-120">Optional query parameters</span></span>
<span data-ttu-id="8aa0c-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8aa0c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8aa0c-122">Request headers</span></span>
| <span data-ttu-id="8aa0c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8aa0c-123">Name</span></span>      |<span data-ttu-id="8aa0c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8aa0c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8aa0c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8aa0c-125">Authorization</span></span>  | <span data-ttu-id="8aa0c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8aa0c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8aa0c-128">Request body</span></span>
<span data-ttu-id="8aa0c-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8aa0c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="8aa0c-130">Response</span></span>

<span data-ttu-id="8aa0c-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [privilegedRoleAssignment](../resources/privilegedroleassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-131">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="8aa0c-132">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="8aa0c-133">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="8aa0c-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="8aa0c-134">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="8aa0c-135">Получите все назначения ролей</span><span class="sxs-lookup"><span data-stu-id="8aa0c-135">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="8aa0c-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="8aa0c-136">Request</span></span>
<span data-ttu-id="8aa0c-137">В следующем примере показано запрос на получение все назначения ролей:</span><span class="sxs-lookup"><span data-stu-id="8aa0c-137">The following example shows a request to get all role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
##### <a name="response"></a><span data-ttu-id="8aa0c-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="8aa0c-138">Response</span></span>
<span data-ttu-id="8aa0c-139">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-139">The following example shows the response.</span></span> <span data-ttu-id="8aa0c-140">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8aa0c-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-141">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-active-role-assignments"></a><span data-ttu-id="8aa0c-142">Получение назначения ролей active</span><span class="sxs-lookup"><span data-stu-id="8aa0c-142">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="8aa0c-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="8aa0c-143">Request</span></span> 
<span data-ttu-id="8aa0c-144">В следующем примере показано запроса для назначения ролей active запроса:</span><span class="sxs-lookup"><span data-stu-id="8aa0c-144">The following example shows a request to query active role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
##### <a name="response"></a><span data-ttu-id="8aa0c-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="8aa0c-145">Response</span></span>
<span data-ttu-id="8aa0c-146">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-146">The following example shows the response.</span></span> <span data-ttu-id="8aa0c-147">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8aa0c-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-148">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="8aa0c-149">Получение назначения ролей постоянное</span><span class="sxs-lookup"><span data-stu-id="8aa0c-149">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="8aa0c-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="8aa0c-150">Request</span></span> 
<span data-ttu-id="8aa0c-151">В следующем примере показан запрос для назначения ролей постоянных запросов, где ``expirationDateTime`` значение — ``null``:</span><span class="sxs-lookup"><span data-stu-id="8aa0c-151">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
##### <a name="response"></a><span data-ttu-id="8aa0c-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="8aa0c-152">Response</span></span>
<span data-ttu-id="8aa0c-153">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-153">The following example shows the response.</span></span> <span data-ttu-id="8aa0c-154">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8aa0c-155">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-155">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="8aa0c-156">Получение назначения ролей право</span><span class="sxs-lookup"><span data-stu-id="8aa0c-156">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="8aa0c-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="8aa0c-157">Request</span></span> 
<span data-ttu-id="8aa0c-158">В следующем примере показано запроса для назначения ролей подходящими запроса, включая активных и неактивная:</span><span class="sxs-lookup"><span data-stu-id="8aa0c-158">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
##### <a name="response"></a><span data-ttu-id="8aa0c-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="8aa0c-159">Response</span></span> 
<span data-ttu-id="8aa0c-160">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-160">The following example shows the response.</span></span> <span data-ttu-id="8aa0c-161">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-161">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8aa0c-162">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8aa0c-162">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
