---
title: Список Говернанцеролеассигнментрекуестс
description: 'Получение коллекции Говернанцеролеассигнментрекуестс. '
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 096ef64c786c35d9b82a45ac4fba75904b743536
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954195"
---
# <a name="list-governanceroleassignmentrequests"></a><span data-ttu-id="451e1-103">Список Говернанцеролеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="451e1-103">List governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="451e1-104">Получение коллекции [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="451e1-104">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="451e1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="451e1-105">Permissions</span></span>
<span data-ttu-id="451e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="451e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="451e1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="451e1-108">Permission type</span></span>      | <span data-ttu-id="451e1-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="451e1-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="451e1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="451e1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="451e1-111">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="451e1-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="451e1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="451e1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="451e1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="451e1-113">Not supported.</span></span>    |
|<span data-ttu-id="451e1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="451e1-114">Application</span></span> | <span data-ttu-id="451e1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="451e1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="451e1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="451e1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="451e1-117">Перечисление коллекции [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="451e1-117">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource.</span></span>
    
><span data-ttu-id="451e1-118">**Примечание:** Кроме области разрешений, запрос должен иметь по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="451e1-118">**Note:** Besides the permission scope, the request requires the requestor to have at least one role assignment on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignmentRequests
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="451e1-119">Перечисление коллекции [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="451e1-119">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=subjectId+eq+'{myId}'
```

<span data-ttu-id="451e1-120">Перечисление коллекции [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md) , которые являются ожидающими решениями администратора.</span><span class="sxs-lookup"><span data-stu-id="451e1-120">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are pending administrator decisions.</span></span>
    
><span data-ttu-id="451e1-121">**Примечание:** В этом запросе, кроме области разрешений, должен быть по крайней мере одно `Active` назначение роли администратора (`owner` или `user access administrator`) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="451e1-121">**Note:** Besides the permission scope, this request requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=status/subStatus+eq+'PendingAdminDecision'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="451e1-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="451e1-122">Optional query parameters</span></span>
<span data-ttu-id="451e1-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="451e1-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="451e1-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="451e1-124">Request headers</span></span>
| <span data-ttu-id="451e1-125">Имя</span><span class="sxs-lookup"><span data-stu-id="451e1-125">Name</span></span>      |<span data-ttu-id="451e1-126">Описание</span><span class="sxs-lookup"><span data-stu-id="451e1-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="451e1-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="451e1-127">Authorization</span></span>  | <span data-ttu-id="451e1-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="451e1-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="451e1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="451e1-129">Request body</span></span>
<span data-ttu-id="451e1-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="451e1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="451e1-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="451e1-131">Response</span></span>
<span data-ttu-id="451e1-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="451e1-132">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="451e1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="451e1-133">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequests"
}-->
<span data-ttu-id="451e1-134">Администраторы запрашивают запросы о назначениях ролей, ожидающие утверждения, для подписки Wingtip Toys — произ.</span><span class="sxs-lookup"><span data-stu-id="451e1-134">Administrators query pending role assignment requests for subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="451e1-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="451e1-135">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="451e1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="451e1-136">Response</span></span>
<span data-ttu-id="451e1-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="451e1-137">Here is an example of the response.</span></span> 

><span data-ttu-id="451e1-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="451e1-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
