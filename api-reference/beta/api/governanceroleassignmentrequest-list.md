---
title: Список governanceRoleAssignmentRequests
description: 'Извлечение коллекции governanceRoleAssignmentRequests. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 9e86f3bb7e6e234d46379660150c1a4e110c1c75
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042172"
---
# <a name="list-governanceroleassignmentrequests"></a><span data-ttu-id="71064-103">Список governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="71064-103">List governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="71064-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71064-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71064-105">Извлечения коллекции [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="71064-105">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="71064-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71064-106">Permissions</span></span>
<span data-ttu-id="71064-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="71064-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="71064-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="71064-109">Azure resources</span></span>

| <span data-ttu-id="71064-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71064-110">Permission type</span></span> | <span data-ttu-id="71064-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71064-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="71064-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71064-112">Delegated (work or school account)</span></span> | <span data-ttu-id="71064-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="71064-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="71064-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71064-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71064-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71064-115">Not supported.</span></span> |
| <span data-ttu-id="71064-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71064-116">Application</span></span> | <span data-ttu-id="71064-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="71064-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="71064-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="71064-118">Azure AD</span></span>

| <span data-ttu-id="71064-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71064-119">Permission type</span></span> | <span data-ttu-id="71064-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71064-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="71064-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71064-121">Delegated (work or school account)</span></span> | <span data-ttu-id="71064-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="71064-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="71064-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71064-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71064-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71064-124">Not supported.</span></span> |
| <span data-ttu-id="71064-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71064-125">Application</span></span> | <span data-ttu-id="71064-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="71064-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="71064-127">Группы</span><span class="sxs-lookup"><span data-stu-id="71064-127">Groups</span></span>

|<span data-ttu-id="71064-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71064-128">Permission type</span></span> | <span data-ttu-id="71064-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71064-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="71064-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71064-130">Delegated (work or school account)</span></span> | <span data-ttu-id="71064-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="71064-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="71064-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71064-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71064-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71064-133">Not supported.</span></span> |
| <span data-ttu-id="71064-134">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71064-134">Application</span></span> | <span data-ttu-id="71064-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="71064-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

## <a name="http-request"></a><span data-ttu-id="71064-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71064-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="71064-137">Список коллекции [governanceRoleAssignmentRequests на](../resources/governanceroleassignmentrequest.md) ресурсе.</span><span class="sxs-lookup"><span data-stu-id="71064-137">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource.</span></span>
    
><span data-ttu-id="71064-138">**Примечание:** Кроме области разрешений, запрос требует, чтобы у запроса было хотя бы одно назначение роли на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="71064-138">**Note:** Besides the permission scope, the request requires the requestor to have at least one role assignment on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignmentRequests
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="71064-139">Список коллекции [моих произведений governanceRoleAssignmentRequests.](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="71064-139">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=subjectId+eq+'{myId}'
```

<span data-ttu-id="71064-140">Список коллекции [управляющегоRoleAssignmentRequests,](../resources/governanceroleassignmentrequest.md) которые находятся в ожидании решений администратора.</span><span class="sxs-lookup"><span data-stu-id="71064-140">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are pending administrator decisions.</span></span>
    
><span data-ttu-id="71064-141">**Примечание:** Помимо области разрешений, для этого запроса требуется, чтобы у запросителя было по крайней мере одно назначение роли администратора `Active` `owner` `user access administrator` (или) на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="71064-141">**Note:** Besides the permission scope, this request requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=status/subStatus+eq+'PendingAdminDecision'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71064-142">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="71064-142">Optional query parameters</span></span>
<span data-ttu-id="71064-143">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="71064-143">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71064-144">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71064-144">Request headers</span></span>
| <span data-ttu-id="71064-145">Имя</span><span class="sxs-lookup"><span data-stu-id="71064-145">Name</span></span>      |<span data-ttu-id="71064-146">Описание</span><span class="sxs-lookup"><span data-stu-id="71064-146">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="71064-147">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71064-147">Authorization</span></span>  | <span data-ttu-id="71064-148">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="71064-148">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="71064-149">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71064-149">Request body</span></span>
<span data-ttu-id="71064-150">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71064-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71064-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="71064-151">Response</span></span>
<span data-ttu-id="71064-152">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="71064-152">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71064-153">Пример</span><span class="sxs-lookup"><span data-stu-id="71064-153">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequests"
}-->
<span data-ttu-id="71064-154">Администраторы запрашивают запросы о назначении ролей для подписки Wingtip Toys - Prod.</span><span class="sxs-lookup"><span data-stu-id="71064-154">Administrators query pending role assignment requests for subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="71064-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="71064-155">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="71064-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="71064-156">Response</span></span>
<span data-ttu-id="71064-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="71064-157">Here is an example of the response.</span></span> 

><span data-ttu-id="71064-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="71064-158">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests",
    "value": [
        {
            "id": "d75c65d8-9e66-44ff-b1cd-1ab0947fde1d",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": "",
            "type": "UserRemove",
            "assignmentState": "Active",
            "requestedDateTime": "2018-01-09T23:41:34.367Z",
            "reason": "Deactivation request",
            "schedule": null,
            "status": {
                "status": "Closed",
                "subStatus": "Revoked",
                "statusDetails": []
            }
        },
        {
            "id": "38f42071-3e81-4191-8c0b-11450fb6b547",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": "",
            "type": "UserAdd",
            "assignmentState": "Active",
            "requestedDateTime": "2018-01-10T20:58:09.163Z",
            "reason": "test activations",
            "status": {
                "status": "Closed",
                "subStatus": "Provisioned",
                "statusDetails": [
                    {
                        "key": "EligibilityRule",
                        "value": "Grant"
                    },
                    {
                        "key": "ExpirationRule",
                        "value": "Grant"
                    },
                    {
                        "key": "MfaRule",
                        "value": "Grant"
                    },
                    {
                        "key": "JustificationRule",
                        "value": "Grant"
                    },
                    {
                        "key": "ActivationDayRule",
                        "value": "Grant"
                    },
                    {
                        "key": "ApprovalRule",
                        "value": "Grant"
                    }
                ]
            },
            "schedule": {
                "type": "Once",
                "startDateTime": "2018-01-10T20:58:11.363914Z",
                "endDateTime": "0001-01-01T00:00:00Z",
                "duration": "PT5H"
            }
        },
        ...
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


