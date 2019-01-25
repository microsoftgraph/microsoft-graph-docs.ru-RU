---
title: Список privilegedRoleAssignments
description: Получение списка privilegedRoleAssignment объекты, которые соответствуют все назначения ролей для организации.
localization_priority: Normal
ms.openlocfilehash: c576e0d9c0a278e02159e02cea94ddd927561e08
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516590"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="a2fa8-103">Список privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="a2fa8-103">List privilegedRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2fa8-104">Получение списка [privilegedRoleAssignment](../resources/privilegedroleassignment.md) объекты, которые соответствуют все назначения ролей для организации.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-104">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="a2fa8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2fa8-105">Permissions</span></span>
<span data-ttu-id="a2fa8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2fa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a2fa8-108">Запросившая сторона должен иметь одно из следующих ролей: _Привилегированной роль администратора_, _Глобального администратора_, _Администратора безопасности_или _Безопасности чтения_.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="a2fa8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2fa8-109">Permission type</span></span>      | <span data-ttu-id="a2fa8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2fa8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2fa8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2fa8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a2fa8-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a2fa8-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a2fa8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2fa8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2fa8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-114">Not supported.</span></span>    |
|<span data-ttu-id="a2fa8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2fa8-115">Application</span></span> | <span data-ttu-id="a2fa8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2fa8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2fa8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a2fa8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a2fa8-118">Optional query parameters</span></span>
<span data-ttu-id="a2fa8-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2fa8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2fa8-120">Request headers</span></span>
| <span data-ttu-id="a2fa8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a2fa8-121">Name</span></span>      |<span data-ttu-id="a2fa8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a2fa8-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a2fa8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2fa8-123">Authorization</span></span>  | <span data-ttu-id="a2fa8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2fa8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2fa8-126">Request body</span></span>
<span data-ttu-id="a2fa8-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2fa8-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2fa8-128">Response</span></span>

<span data-ttu-id="a2fa8-129">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [privilegedRoleAssignment](../resources/privilegedroleassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-129">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="a2fa8-130">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="a2fa8-131">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="a2fa8-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="a2fa8-132">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="a2fa8-133">Получите все назначения ролей</span><span class="sxs-lookup"><span data-stu-id="a2fa8-133">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="a2fa8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2fa8-134">Request</span></span>
<span data-ttu-id="a2fa8-135">В следующем примере показано запрос на получение все назначения ролей:</span><span class="sxs-lookup"><span data-stu-id="a2fa8-135">The following example shows a request to get all role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
##### <a name="response"></a><span data-ttu-id="a2fa8-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2fa8-136">Response</span></span>
<span data-ttu-id="a2fa8-137">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-137">The following example shows the response.</span></span> <span data-ttu-id="a2fa8-138">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a2fa8-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-139">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-active-role-assignments"></a><span data-ttu-id="a2fa8-140">Получение назначения ролей active</span><span class="sxs-lookup"><span data-stu-id="a2fa8-140">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="a2fa8-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2fa8-141">Request</span></span> 
<span data-ttu-id="a2fa8-142">В следующем примере показано запроса для назначения ролей active запроса:</span><span class="sxs-lookup"><span data-stu-id="a2fa8-142">The following example shows a request to query active role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
##### <a name="response"></a><span data-ttu-id="a2fa8-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2fa8-143">Response</span></span>
<span data-ttu-id="a2fa8-144">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-144">The following example shows the response.</span></span> <span data-ttu-id="a2fa8-145">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-145">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a2fa8-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-146">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="a2fa8-147">Получение назначения ролей постоянное</span><span class="sxs-lookup"><span data-stu-id="a2fa8-147">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="a2fa8-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2fa8-148">Request</span></span> 
<span data-ttu-id="a2fa8-149">В следующем примере показан запрос для назначения ролей постоянных запросов, где ``expirationDateTime`` значение — ``null``:</span><span class="sxs-lookup"><span data-stu-id="a2fa8-149">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
##### <a name="response"></a><span data-ttu-id="a2fa8-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2fa8-150">Response</span></span>
<span data-ttu-id="a2fa8-151">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-151">The following example shows the response.</span></span> <span data-ttu-id="a2fa8-152">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a2fa8-153">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-153">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="a2fa8-154">Получение назначения ролей право</span><span class="sxs-lookup"><span data-stu-id="a2fa8-154">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="a2fa8-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2fa8-155">Request</span></span> 
<span data-ttu-id="a2fa8-156">В следующем примере показано запроса для назначения ролей подходящими запроса, включая активных и неактивная:</span><span class="sxs-lookup"><span data-stu-id="a2fa8-156">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
##### <a name="response"></a><span data-ttu-id="a2fa8-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2fa8-157">Response</span></span> 
<span data-ttu-id="a2fa8-158">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-158">The following example shows the response.</span></span> <span data-ttu-id="a2fa8-159">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a2fa8-160">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2fa8-160">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/privilegedroleassignment-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
