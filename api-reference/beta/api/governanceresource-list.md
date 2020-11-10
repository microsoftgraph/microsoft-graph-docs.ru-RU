---
title: Список Говернанцересаурцес
description: Получение коллекции governanceResource, к которой у запрашивающего есть доступ.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: a2414c02c2526ffccb1aab6bd75101047e5bbe6c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954425"
---
# <a name="list-governanceresources"></a><span data-ttu-id="7b05a-103">Список Говернанцересаурцес</span><span class="sxs-lookup"><span data-stu-id="7b05a-103">List governanceResources</span></span>

<span data-ttu-id="7b05a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b05a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b05a-105">Получение коллекции [governanceResource](../resources/governanceresource.md) , к которой у запрашивающего есть доступ.</span><span class="sxs-lookup"><span data-stu-id="7b05a-105">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b05a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b05a-106">Permissions</span></span>
<span data-ttu-id="7b05a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="7b05a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="7b05a-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="7b05a-109">Azure resources</span></span>

| <span data-ttu-id="7b05a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b05a-110">Permission type</span></span> | <span data-ttu-id="7b05a-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b05a-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="7b05a-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b05a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7b05a-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="7b05a-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="7b05a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b05a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b05a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b05a-115">Not supported.</span></span> |
| <span data-ttu-id="7b05a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b05a-116">Application</span></span> | <span data-ttu-id="7b05a-117">Привилежедакцесс. Read. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="7b05a-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="7b05a-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="7b05a-118">Azure AD</span></span>

| <span data-ttu-id="7b05a-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b05a-119">Permission type</span></span> | <span data-ttu-id="7b05a-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b05a-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="7b05a-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b05a-121">Delegated (work or school account)</span></span> | <span data-ttu-id="7b05a-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="7b05a-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="7b05a-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b05a-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b05a-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b05a-124">Not supported.</span></span> |
| <span data-ttu-id="7b05a-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b05a-125">Application</span></span> | <span data-ttu-id="7b05a-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="7b05a-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="7b05a-127">Группы</span><span class="sxs-lookup"><span data-stu-id="7b05a-127">Groups</span></span>

|<span data-ttu-id="7b05a-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b05a-128">Permission type</span></span> | <span data-ttu-id="7b05a-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b05a-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="7b05a-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b05a-130">Delegated (work or school account)</span></span> | <span data-ttu-id="7b05a-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="7b05a-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="7b05a-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b05a-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b05a-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b05a-133">Not supported.</span></span> |
| <span data-ttu-id="7b05a-134">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b05a-134">Application</span></span> | <span data-ttu-id="7b05a-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="7b05a-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b05a-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b05a-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7b05a-137">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7b05a-137">Optional query parameters</span></span>
<span data-ttu-id="7b05a-138">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7b05a-138">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b05a-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b05a-139">Request headers</span></span>
| <span data-ttu-id="7b05a-140">Имя</span><span class="sxs-lookup"><span data-stu-id="7b05a-140">Name</span></span>      |<span data-ttu-id="7b05a-141">Описание</span><span class="sxs-lookup"><span data-stu-id="7b05a-141">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7b05a-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b05a-142">Authorization</span></span>  | <span data-ttu-id="7b05a-143">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7b05a-143">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b05a-144">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b05a-144">Request body</span></span>
<span data-ttu-id="7b05a-145">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b05a-145">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7b05a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b05a-146">Response</span></span>
<span data-ttu-id="7b05a-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [governanceResource](../resources/governanceresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7b05a-147">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="7b05a-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="7b05a-148">Examples</span></span>

<span data-ttu-id="7b05a-149">В этом примере выводится список всех ресурсов, к которым я могу получить доступ.</span><span class="sxs-lookup"><span data-stu-id="7b05a-149">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="7b05a-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b05a-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7b05a-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b05a-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
# <a name="c"></a>[<span data-ttu-id="7b05a-152">C#</span><span class="sxs-lookup"><span data-stu-id="7b05a-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-governanceresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b05a-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b05a-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-governanceresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b05a-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b05a-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-governanceresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b05a-155">Java</span><span class="sxs-lookup"><span data-stu-id="7b05a-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-governanceresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7b05a-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b05a-156">Response</span></span>
<span data-ttu-id="7b05a-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7b05a-157">Here is an example of the response.</span></span> 

><span data-ttu-id="7b05a-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b05a-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


