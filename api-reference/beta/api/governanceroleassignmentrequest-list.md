---
title: Список Говернанцеролеассигнментрекуестс
description: 'Получение коллекции Говернанцеролеассигнментрекуестс. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: f7b35d88167a608d2a25ae5a76a1fed8ed539d58
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634916"
---
# <a name="list-governanceroleassignmentrequests"></a><span data-ttu-id="0c310-103">Список Говернанцеролеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="0c310-103">List governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="0c310-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c310-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c310-105">Получение коллекции [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="0c310-105">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="0c310-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c310-106">Permissions</span></span>
<span data-ttu-id="0c310-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="0c310-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="0c310-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="0c310-109">Azure resources</span></span>

| <span data-ttu-id="0c310-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c310-110">Permission type</span></span> | <span data-ttu-id="0c310-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c310-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="0c310-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c310-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0c310-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0c310-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="0c310-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c310-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c310-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c310-115">Not supported.</span></span> |
| <span data-ttu-id="0c310-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0c310-116">Application</span></span> | <span data-ttu-id="0c310-117">Привилежедакцесс. Read. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="0c310-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="0c310-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="0c310-118">Azure AD</span></span>

| <span data-ttu-id="0c310-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c310-119">Permission type</span></span> | <span data-ttu-id="0c310-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c310-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="0c310-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c310-121">Delegated (work or school account)</span></span> | <span data-ttu-id="0c310-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="0c310-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="0c310-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c310-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c310-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c310-124">Not supported.</span></span> |
| <span data-ttu-id="0c310-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="0c310-125">Application</span></span> | <span data-ttu-id="0c310-126">Привилежедакцесс. Read. AzureAD</span><span class="sxs-lookup"><span data-stu-id="0c310-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="0c310-127">Группы</span><span class="sxs-lookup"><span data-stu-id="0c310-127">Groups</span></span>

|<span data-ttu-id="0c310-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c310-128">Permission type</span></span> | <span data-ttu-id="0c310-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c310-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="0c310-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c310-130">Delegated (work or school account)</span></span> | <span data-ttu-id="0c310-131">Привилежедакцесс. ReadWrite. Азуреадграупс</span><span class="sxs-lookup"><span data-stu-id="0c310-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="0c310-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c310-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c310-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c310-133">Not supported.</span></span> |
| <span data-ttu-id="0c310-134">Приложение</span><span class="sxs-lookup"><span data-stu-id="0c310-134">Application</span></span> | <span data-ttu-id="0c310-135">Привилежедакцесс. Read. Азуреадграупс</span><span class="sxs-lookup"><span data-stu-id="0c310-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c310-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c310-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="0c310-137">Перечисление коллекции [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="0c310-137">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource.</span></span>
    
><span data-ttu-id="0c310-138">**Примечание:** Кроме области разрешений, запрос должен иметь по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="0c310-138">**Note:** Besides the permission scope, the request requires the requestor to have at least one role assignment on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignmentRequests
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="0c310-139">Перечисление коллекции [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="0c310-139">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=subjectId+eq+'{myId}'
```

<span data-ttu-id="0c310-140">Перечисление коллекции [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md) , которые являются ожидающими решениями администратора.</span><span class="sxs-lookup"><span data-stu-id="0c310-140">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are pending administrator decisions.</span></span>
    
><span data-ttu-id="0c310-141">**Примечание:** В этом запросе, кроме области разрешений, должен быть по крайней мере одно `Active` назначение роли администратора ( `owner` или `user access administrator` ) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="0c310-141">**Note:** Besides the permission scope, this request requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=status/subStatus+eq+'PendingAdminDecision'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0c310-142">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0c310-142">Optional query parameters</span></span>
<span data-ttu-id="0c310-143">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0c310-143">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c310-144">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c310-144">Request headers</span></span>
| <span data-ttu-id="0c310-145">Имя</span><span class="sxs-lookup"><span data-stu-id="0c310-145">Name</span></span>      |<span data-ttu-id="0c310-146">Описание</span><span class="sxs-lookup"><span data-stu-id="0c310-146">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0c310-147">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c310-147">Authorization</span></span>  | <span data-ttu-id="0c310-148">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0c310-148">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c310-149">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c310-149">Request body</span></span>
<span data-ttu-id="0c310-150">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c310-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c310-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c310-151">Response</span></span>
<span data-ttu-id="0c310-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0c310-152">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c310-153">Пример</span><span class="sxs-lookup"><span data-stu-id="0c310-153">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequests"
}-->
<span data-ttu-id="0c310-154">Администраторы запрашивают запросы о назначениях ролей, ожидающие утверждения, для подписки Wingtip Toys — произ.</span><span class="sxs-lookup"><span data-stu-id="0c310-154">Administrators query pending role assignment requests for subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="0c310-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c310-155">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="0c310-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c310-156">Response</span></span>
<span data-ttu-id="0c310-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0c310-157">Here is an example of the response.</span></span> 

><span data-ttu-id="0c310-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c310-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


