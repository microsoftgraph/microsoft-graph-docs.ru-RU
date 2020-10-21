---
title: Получение governanceRoleAssignment
description: Получение свойств и связей объекта governanceRoleAssignment.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: de602313da0528255893c4729200387fcaff971d
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635035"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="23ae0-103">Получение governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="23ae0-103">Get governanceRoleAssignment</span></span>

<span data-ttu-id="23ae0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23ae0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23ae0-105">Получение свойств и связей объекта [governanceRoleAssignment](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="23ae0-105">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="23ae0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23ae0-106">Permissions</span></span>
<span data-ttu-id="23ae0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="23ae0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="23ae0-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="23ae0-109">Azure resources</span></span>

| <span data-ttu-id="23ae0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23ae0-110">Permission type</span></span> | <span data-ttu-id="23ae0-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23ae0-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="23ae0-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23ae0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="23ae0-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="23ae0-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="23ae0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23ae0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23ae0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23ae0-115">Not supported.</span></span> |
| <span data-ttu-id="23ae0-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="23ae0-116">Application</span></span> | <span data-ttu-id="23ae0-117">Привилежедакцесс. Read. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="23ae0-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="23ae0-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="23ae0-118">Azure AD</span></span>

| <span data-ttu-id="23ae0-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23ae0-119">Permission type</span></span> | <span data-ttu-id="23ae0-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23ae0-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="23ae0-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23ae0-121">Delegated (work or school account)</span></span> | <span data-ttu-id="23ae0-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="23ae0-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="23ae0-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23ae0-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23ae0-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23ae0-124">Not supported.</span></span> |
| <span data-ttu-id="23ae0-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="23ae0-125">Application</span></span> | <span data-ttu-id="23ae0-126">Привилежедакцесс. Read. AzureAD</span><span class="sxs-lookup"><span data-stu-id="23ae0-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="23ae0-127">Группы</span><span class="sxs-lookup"><span data-stu-id="23ae0-127">Groups</span></span>

|<span data-ttu-id="23ae0-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23ae0-128">Permission type</span></span> | <span data-ttu-id="23ae0-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23ae0-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="23ae0-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23ae0-130">Delegated (work or school account)</span></span> | <span data-ttu-id="23ae0-131">Привилежедакцесс. ReadWrite. Азуреадграупс</span><span class="sxs-lookup"><span data-stu-id="23ae0-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="23ae0-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23ae0-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23ae0-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23ae0-133">Not supported.</span></span> |
| <span data-ttu-id="23ae0-134">Приложение</span><span class="sxs-lookup"><span data-stu-id="23ae0-134">Application</span></span> | <span data-ttu-id="23ae0-135">Привилежедакцесс. Read. Азуреадграупс</span><span class="sxs-lookup"><span data-stu-id="23ae0-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

## <a name="http-request"></a><span data-ttu-id="23ae0-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23ae0-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="23ae0-137">Получение [governanceRoleAssignment](../resources/governanceroleassignment.md) для ресурса</span><span class="sxs-lookup"><span data-stu-id="23ae0-137">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="23ae0-138">*Примечание. Кроме области разрешений, необходимо, чтобы запрашивающий был иметь по крайней мере одно назначение роли для ресурса.*</span><span class="sxs-lookup"><span data-stu-id="23ae0-138">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="23ae0-139">Получение [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="23ae0-139">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23ae0-140">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="23ae0-140">Optional query parameters</span></span>
<span data-ttu-id="23ae0-141">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters) , не позволяющие `$filter` настраивать ответ.</span><span class="sxs-lookup"><span data-stu-id="23ae0-141">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23ae0-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23ae0-142">Request headers</span></span>
| <span data-ttu-id="23ae0-143">Имя</span><span class="sxs-lookup"><span data-stu-id="23ae0-143">Name</span></span>      |<span data-ttu-id="23ae0-144">Описание</span><span class="sxs-lookup"><span data-stu-id="23ae0-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="23ae0-145">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23ae0-145">Authorization</span></span>  | <span data-ttu-id="23ae0-146">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="23ae0-146">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="23ae0-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23ae0-147">Request body</span></span>
<span data-ttu-id="23ae0-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23ae0-148">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="23ae0-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="23ae0-149">Response</span></span>
<span data-ttu-id="23ae0-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [governanceRoleAssignment](../resources/governanceroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23ae0-150">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23ae0-151">Пример</span><span class="sxs-lookup"><span data-stu-id="23ae0-151">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="23ae0-152">Получение [governanceRoleAssignment](../resources/governanceroleassignment.md) по подписке "Wingtip Toys — произ"</span><span class="sxs-lookup"><span data-stu-id="23ae0-152">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="23ae0-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="23ae0-153">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="23ae0-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="23ae0-154">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 182

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignments/$entity",
    "id": "0ba78f41-ee7a-4227-adb9-1499431b2164",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
    "subjectId": "74487eb5-1630-4fa8-9581-0bb076ea5de3",
    "linkedEligibleRoleAssignmentId": null,
    "externalId": null,
    "startDateTime": "2018-01-22T23:47:19.687Z",
    "endDateTime": "2018-07-21T23:47:02.887Z",
    "memberType": "Direct",
    "assignmentState": "Eligible",
    "status": "Provisioned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


