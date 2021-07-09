---
title: Управление экспортомRoleAssignmentRequests
description: Извлеките коллекцию файлов governanceRoleAssignmentRequests в формате, которые можно .csv в `application/octet-stream` браузере.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8faff2bbd4b41eda693467b55641204cb6bbaef3
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350854"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="8c528-103">Управление экспортомRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="8c528-103">Export governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="8c528-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c528-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c528-105">Извлеките коллекцию [файлов governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) в формате, которые можно .csv в `application/octet-stream` браузере.</span><span class="sxs-lookup"><span data-stu-id="8c528-105">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c528-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c528-106">Permissions</span></span>
<span data-ttu-id="8c528-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="8c528-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="8c528-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="8c528-109">Azure resources</span></span>

| <span data-ttu-id="8c528-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c528-110">Permission type</span></span> | <span data-ttu-id="8c528-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c528-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="8c528-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c528-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8c528-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="8c528-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="8c528-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c528-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c528-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c528-115">Not supported.</span></span> |
| <span data-ttu-id="8c528-116">Application</span><span class="sxs-lookup"><span data-stu-id="8c528-116">Application</span></span> | <span data-ttu-id="8c528-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="8c528-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="8c528-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="8c528-118">Azure AD</span></span>

| <span data-ttu-id="8c528-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c528-119">Permission type</span></span> | <span data-ttu-id="8c528-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c528-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="8c528-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c528-121">Delegated (work or school account)</span></span> | <span data-ttu-id="8c528-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="8c528-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="8c528-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c528-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c528-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c528-124">Not supported.</span></span> |
| <span data-ttu-id="8c528-125">Application</span><span class="sxs-lookup"><span data-stu-id="8c528-125">Application</span></span> | <span data-ttu-id="8c528-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="8c528-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="8c528-127">Группы</span><span class="sxs-lookup"><span data-stu-id="8c528-127">Groups</span></span>

|<span data-ttu-id="8c528-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c528-128">Permission type</span></span> | <span data-ttu-id="8c528-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c528-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="8c528-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c528-130">Delegated (work or school account)</span></span> | <span data-ttu-id="8c528-131">PrivilegedAccess.ReadWrite.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="8c528-131">PrivilegedAccess.ReadWrite.AzureADGroup</span></span> |
| <span data-ttu-id="8c528-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c528-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c528-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c528-133">Not supported.</span></span> |
| <span data-ttu-id="8c528-134">Application</span><span class="sxs-lookup"><span data-stu-id="8c528-134">Application</span></span> | <span data-ttu-id="8c528-135">PrivilegedAccess.Read.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="8c528-135">PrivilegedAccess.Read.AzureADGroup</span></span> |


## <a name="http-request"></a><span data-ttu-id="8c528-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c528-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="8c528-137">Экспорт коллекции [governanceRoleAssignmentRequests на](../resources/governanceroleassignmentrequest.md) ресурсе</span><span class="sxs-lookup"><span data-stu-id="8c528-137">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="8c528-138">**Примечание:** Помимо области разрешений, для этого запроса требуется, чтобы у запросителя было по крайней мере одно назначение ролей на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="8c528-138">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="8c528-139">Экспорт коллекции [моих произведений governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="8c528-139">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8c528-140">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8c528-140">Optional query parameters</span></span>
<span data-ttu-id="8c528-141">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8c528-141">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c528-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c528-142">Request headers</span></span>
| <span data-ttu-id="8c528-143">Имя</span><span class="sxs-lookup"><span data-stu-id="8c528-143">Name</span></span>      |<span data-ttu-id="8c528-144">Описание</span><span class="sxs-lookup"><span data-stu-id="8c528-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c528-145">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c528-145">Authorization</span></span>  | <span data-ttu-id="8c528-146">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8c528-146">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c528-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c528-147">Request body</span></span>
<span data-ttu-id="8c528-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c528-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c528-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c528-149">Response</span></span>
<span data-ttu-id="8c528-150">В случае успешной работы этот метод возвращает код `200 OK` ответа и содержимое `application/octet-stream` типа.</span><span class="sxs-lookup"><span data-stu-id="8c528-150">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="8c528-151">Пример</span><span class="sxs-lookup"><span data-stu-id="8c528-151">Example</span></span>
<span data-ttu-id="8c528-152">В этом примере сохраняется все назначения ролей в .csv в подписной папке Wingtip Toys — Prod.</span><span class="sxs-lookup"><span data-stu-id="8c528-152">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="8c528-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c528-153">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="8c528-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c528-154">Response</span></span>
<span data-ttu-id="8c528-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c528-155">Here is an example of the response.</span></span> 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


