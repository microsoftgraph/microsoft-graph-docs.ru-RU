---
title: Список Говернанцеролеассигнментс
description: Получение коллекции Говернанцеролеассигнментс.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 338fb9c4d02b87e940fbb0fc867edbb374e9d42b
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635028"
---
# <a name="list-governanceroleassignments"></a><span data-ttu-id="f3f00-103">Список Говернанцеролеассигнментс</span><span class="sxs-lookup"><span data-stu-id="f3f00-103">List governanceRoleAssignments</span></span>

<span data-ttu-id="f3f00-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3f00-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3f00-105">Получение коллекции [говернанцеролеассигнментс](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f3f00-105">Retrieve a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f3f00-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3f00-106">Permissions</span></span>
<span data-ttu-id="f3f00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="f3f00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="f3f00-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="f3f00-109">Azure resources</span></span>

| <span data-ttu-id="f3f00-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3f00-110">Permission type</span></span> | <span data-ttu-id="f3f00-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3f00-111">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="f3f00-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3f00-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f3f00-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f3f00-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="f3f00-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3f00-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3f00-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3f00-115">Not supported.</span></span> |
| <span data-ttu-id="f3f00-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="f3f00-116">Application</span></span> | <span data-ttu-id="f3f00-117">Привилежедакцесс. Read. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="f3f00-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="f3f00-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="f3f00-118">Azure AD</span></span>

| <span data-ttu-id="f3f00-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3f00-119">Permission type</span></span> | <span data-ttu-id="f3f00-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3f00-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="f3f00-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3f00-121">Delegated (work or school account)</span></span> | <span data-ttu-id="f3f00-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="f3f00-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="f3f00-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3f00-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3f00-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3f00-124">Not supported.</span></span> |
| <span data-ttu-id="f3f00-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="f3f00-125">Application</span></span> | <span data-ttu-id="f3f00-126">Привилежедакцесс. Read. AzureAD</span><span class="sxs-lookup"><span data-stu-id="f3f00-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="f3f00-127">Группы</span><span class="sxs-lookup"><span data-stu-id="f3f00-127">Groups</span></span>

|<span data-ttu-id="f3f00-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3f00-128">Permission type</span></span> | <span data-ttu-id="f3f00-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3f00-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="f3f00-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3f00-130">Delegated (work or school account)</span></span> | <span data-ttu-id="f3f00-131">Привилежедакцесс. ReadWrite. Азуреадграупс</span><span class="sxs-lookup"><span data-stu-id="f3f00-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="f3f00-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3f00-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3f00-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3f00-133">Not supported.</span></span> |
| <span data-ttu-id="f3f00-134">Приложение</span><span class="sxs-lookup"><span data-stu-id="f3f00-134">Application</span></span> | <span data-ttu-id="f3f00-135">Привилежедакцесс. Read. Азуреадграупс</span><span class="sxs-lookup"><span data-stu-id="f3f00-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3f00-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3f00-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="f3f00-137">Перечисление коллекции [говернанцеролеассигнментс](../resources/governanceroleassignment.md) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="f3f00-137">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) on a resource.</span></span>

><span data-ttu-id="f3f00-138">**Примечание:** Кроме области разрешений, этот запрос требует, чтобы запрашивающая сторона состроила по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="f3f00-138">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments
GET /privilegedAccess/azureResources/roleAssignments?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="f3f00-139">Перечисление коллекции [говернанцеролеассигнментс](../resources/governanceroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="f3f00-139">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) of mine.</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f3f00-140">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f3f00-140">Optional query parameters</span></span>
<span data-ttu-id="f3f00-141">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f3f00-141">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3f00-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3f00-142">Request headers</span></span>
| <span data-ttu-id="f3f00-143">Имя</span><span class="sxs-lookup"><span data-stu-id="f3f00-143">Name</span></span>      |<span data-ttu-id="f3f00-144">Описание</span><span class="sxs-lookup"><span data-stu-id="f3f00-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f3f00-145">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3f00-145">Authorization</span></span>  | <span data-ttu-id="f3f00-146">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f3f00-146">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3f00-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3f00-147">Request body</span></span>
<span data-ttu-id="f3f00-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3f00-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3f00-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3f00-149">Response</span></span>
<span data-ttu-id="f3f00-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [governanceRoleAssignment](../resources/governanceroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f3f00-150">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignment](../resources/governanceroleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f3f00-151">Пример</span><span class="sxs-lookup"><span data-stu-id="f3f00-151">Example</span></span>

<span data-ttu-id="f3f00-152">В этом примере показано, как получить назначения ролей для подписки Wingtip Toys — произ.</span><span class="sxs-lookup"><span data-stu-id="f3f00-152">This example shows how to get my role assignments on the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignments"
}-->
##### <a name="request"></a><span data-ttu-id="f3f00-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3f00-153">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'918e54be-12c4-4f4c-a6d3-2ee0e3661c51'
```
##### <a name="response"></a><span data-ttu-id="f3f00-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3f00-154">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 2062

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignments",
    "value": [
        {
            "id": "20f4157d-5837-4356-9630-ebd3a832f227",
            "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
            "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": null,
            "externalId": null,
            "startDateTime": "2018-03-13T01:19:08.59Z",
            "endDateTime": "2018-06-11T01:18:37.08Z",
            "memberType": "Direct",
            "assignmentState": "Eligible",
            "status": "Provisioned"
        },
        {
            "id": "e327f4be-42a0-47a2-8579-0a39b025b394",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": null,
            "externalId": null,
            "startDateTime": "2018-03-28T16:56:48.243Z",
            "endDateTime": "2018-09-24T16:56:30.547Z",
            "memberType": "Direct",
            "assignmentState": "Eligible",
            "status": "Provisioned"
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
  "description": "List roleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


