---
title: Список governanceRoleAssignmentRequests
description: 'Получите коллекцию governanceRoleAssignmentRequests. '
localization_priority: Normal
ms.openlocfilehash: 24391cf851ddb7de698a0798a85bf6e7a8aa9770
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878995"
---
# <a name="list-governanceroleassignmentrequests"></a><span data-ttu-id="e6c06-103">Список governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="e6c06-103">List governanceRoleAssignmentRequests</span></span>

> <span data-ttu-id="e6c06-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e6c06-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6c06-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6c06-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e6c06-106">Получите коллекцию [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="e6c06-106">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="e6c06-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6c06-107">Permissions</span></span>
<span data-ttu-id="e6c06-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6c06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6c06-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6c06-110">Permission type</span></span>      | <span data-ttu-id="e6c06-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="e6c06-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6c06-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6c06-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e6c06-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e6c06-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="e6c06-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6c06-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6c06-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6c06-115">Not supported.</span></span>    |
|<span data-ttu-id="e6c06-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6c06-116">Application</span></span> | <span data-ttu-id="e6c06-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="e6c06-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6c06-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6c06-118">HTTP request</span></span>
<span data-ttu-id="e6c06-119"><!-- { "blockType": "ignored" } -->Список коллекцию [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="e6c06-119"><!-- { "blockType": "ignored" } --> List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource.</span></span>
    
><span data-ttu-id="e6c06-120">**Примечание:** Помимо области разрешений для запроса требуется инициатор запроса может иметь по крайней мере одна роль назначения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="e6c06-120">**Note:** Besides the permission scope, the request requires the requestor to have at least one role assignment on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignmentRequests
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="e6c06-121">Список коллекцию [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) моей.</span><span class="sxs-lookup"><span data-stu-id="e6c06-121">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=subjectId+eq+'{myId}'
```

<span data-ttu-id="e6c06-122">Список коллекцию [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) , которые решения ожидающие администратора.</span><span class="sxs-lookup"><span data-stu-id="e6c06-122">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are pending administrator decisions.</span></span>
    
><span data-ttu-id="e6c06-123">**Примечание:** Помимо области разрешений для этого запроса требуется инициатор запроса может иметь по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="e6c06-123">**Note:** Besides the permission scope, this request requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=status/subStatus+eq+'PendingAdminDecision'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e6c06-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e6c06-124">Optional query parameters</span></span>
<span data-ttu-id="e6c06-125">Этот метод поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="e6c06-125">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6c06-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6c06-126">Request headers</span></span>
| <span data-ttu-id="e6c06-127">Имя</span><span class="sxs-lookup"><span data-stu-id="e6c06-127">Name</span></span>      |<span data-ttu-id="e6c06-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e6c06-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e6c06-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6c06-129">Authorization</span></span>  | <span data-ttu-id="e6c06-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e6c06-130">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6c06-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e6c06-131">Request body</span></span>
<span data-ttu-id="e6c06-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6c06-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6c06-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6c06-133">Response</span></span>
<span data-ttu-id="e6c06-134">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e6c06-134">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6c06-135">Пример</span><span class="sxs-lookup"><span data-stu-id="e6c06-135">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequests"
}-->
<span data-ttu-id="e6c06-136">Администраторы запросов ожидающие роль назначения для подписки на Wingtip Toys - производственного.</span><span class="sxs-lookup"><span data-stu-id="e6c06-136">Administrators query pending role assignment requests for subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="e6c06-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6c06-137">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="e6c06-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6c06-138">Response</span></span>
<span data-ttu-id="e6c06-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e6c06-139">Here is an example of the response.</span></span> 

><span data-ttu-id="e6c06-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6c06-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
