---
title: Список governanceResources
description: Извлечение коллекции governanceResource, к которую имеет доступ запроситель.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: d8f78f1e52c91981cef4f0be9a5101f2a7ef9feb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042200"
---
# <a name="list-governanceresources"></a><span data-ttu-id="b8834-103">Список governanceResources</span><span class="sxs-lookup"><span data-stu-id="b8834-103">List governanceResources</span></span>

<span data-ttu-id="b8834-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8834-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8834-105">Извлечение коллекции [governanceResource,](../resources/governanceresource.md) к которую имеет доступ запроситель.</span><span class="sxs-lookup"><span data-stu-id="b8834-105">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8834-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8834-106">Permissions</span></span>
<span data-ttu-id="b8834-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="b8834-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="b8834-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="b8834-109">Azure resources</span></span>

| <span data-ttu-id="b8834-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8834-110">Permission type</span></span> | <span data-ttu-id="b8834-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8834-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="b8834-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8834-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b8834-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b8834-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="b8834-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8834-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8834-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8834-115">Not supported.</span></span> |
| <span data-ttu-id="b8834-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8834-116">Application</span></span> | <span data-ttu-id="b8834-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b8834-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="b8834-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="b8834-118">Azure AD</span></span>

| <span data-ttu-id="b8834-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8834-119">Permission type</span></span> | <span data-ttu-id="b8834-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8834-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="b8834-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8834-121">Delegated (work or school account)</span></span> | <span data-ttu-id="b8834-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="b8834-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="b8834-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8834-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8834-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8834-124">Not supported.</span></span> |
| <span data-ttu-id="b8834-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8834-125">Application</span></span> | <span data-ttu-id="b8834-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="b8834-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="b8834-127">Группы</span><span class="sxs-lookup"><span data-stu-id="b8834-127">Groups</span></span>

|<span data-ttu-id="b8834-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8834-128">Permission type</span></span> | <span data-ttu-id="b8834-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8834-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="b8834-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8834-130">Delegated (work or school account)</span></span> | <span data-ttu-id="b8834-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="b8834-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="b8834-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8834-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8834-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8834-133">Not supported.</span></span> |
| <span data-ttu-id="b8834-134">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8834-134">Application</span></span> | <span data-ttu-id="b8834-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="b8834-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8834-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8834-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b8834-137">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b8834-137">Optional query parameters</span></span>
<span data-ttu-id="b8834-138">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b8834-138">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8834-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8834-139">Request headers</span></span>
| <span data-ttu-id="b8834-140">Имя</span><span class="sxs-lookup"><span data-stu-id="b8834-140">Name</span></span>      |<span data-ttu-id="b8834-141">Описание</span><span class="sxs-lookup"><span data-stu-id="b8834-141">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b8834-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8834-142">Authorization</span></span>  | <span data-ttu-id="b8834-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b8834-143">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8834-144">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8834-144">Request body</span></span>
<span data-ttu-id="b8834-145">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b8834-145">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b8834-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8834-146">Response</span></span>
<span data-ttu-id="b8834-147">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` объектов [governanceResource](../resources/governanceresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b8834-147">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="b8834-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="b8834-148">Examples</span></span>

<span data-ttu-id="b8834-149">В этом примере перечислены все ресурсы, к которые в настоящее время можно получить доступ.</span><span class="sxs-lookup"><span data-stu-id="b8834-149">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="b8834-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8834-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b8834-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8834-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
# <a name="c"></a>[<span data-ttu-id="b8834-152">C#</span><span class="sxs-lookup"><span data-stu-id="b8834-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-governanceresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8834-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8834-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-governanceresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8834-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8834-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-governanceresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b8834-155">Java</span><span class="sxs-lookup"><span data-stu-id="b8834-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-governanceresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b8834-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8834-156">Response</span></span>
<span data-ttu-id="b8834-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b8834-157">Here is an example of the response.</span></span> 

><span data-ttu-id="b8834-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b8834-158">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1289

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceResources",
    "value":[
        {
            "id": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/resourceGroups/AnujRG/providers/Microsoft.Storage/storageAccounts/anujstoragefimdev",
            "type": "Microsoft.Storage/storageAccounts",
            "displayName": "anujstoragefimdev",
            "status": "Active",
            "registeredDateTime": "2018-04-05T22:30:37.13Z",
            "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",  
        },
        {
            "id": "0e0e4461-0c46-4d13-bf69-7cacbec75471",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/resourceGroups/ARPJ-TESTRG-01/providers/Microsoft.Compute/virtualMachines/APRJ-VM-01-T",
            "type": "Microsoft.Compute/virtualMachines",
            "displayName": "APRJ-VM-01-T",
            "status": "Active",
            "registeredDateTime": "2018-04-05T22:30:37.13Z",
            "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",  
        },
        {
            "id": "c072eb85-e47b-4627-81cb-5af82a8fc9fb",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/resourceGroups/ARPJ-TESTRG-01/providers/Microsoft.Compute/virtualMachines/APRJ-VM-01-T/extensions/IaaSAntimalware",
            "type": "Microsoft.Compute/virtualMachines/extensions",
            "displayName": "APRJ-VM-01-T/IaaSAntimalware",
            "status": "Active",
            "registeredDateTime": "2018-04-05T22:30:37.13Z",
            "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",  
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


