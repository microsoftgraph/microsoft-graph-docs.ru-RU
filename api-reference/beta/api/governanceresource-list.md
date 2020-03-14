---
title: Список Говернанцересаурцес
description: Получение коллекции governanceResource, к которой у запрашивающего есть доступ.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identitiy-platform
ms.openlocfilehash: 98c19e86b80a95d23e12508740f082370997f147
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639872"
---
# <a name="list-governanceresources"></a><span data-ttu-id="45fa0-103">Список Говернанцересаурцес</span><span class="sxs-lookup"><span data-stu-id="45fa0-103">List governanceResources</span></span>

<span data-ttu-id="45fa0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45fa0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45fa0-105">Получение коллекции [governanceResource](../resources/governanceresource.md) , к которой у запрашивающего есть доступ.</span><span class="sxs-lookup"><span data-stu-id="45fa0-105">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="45fa0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45fa0-106">Permissions</span></span>
<span data-ttu-id="45fa0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45fa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45fa0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45fa0-109">Permission type</span></span>      | <span data-ttu-id="45fa0-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="45fa0-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45fa0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45fa0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="45fa0-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="45fa0-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="45fa0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45fa0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45fa0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45fa0-114">Not supported.</span></span>    |
|<span data-ttu-id="45fa0-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="45fa0-115">Application</span></span> | <span data-ttu-id="45fa0-116">Привилежедакцесс. Read. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="45fa0-116">PrivilegedAccess.Read.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="45fa0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45fa0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="45fa0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="45fa0-118">Optional query parameters</span></span>
<span data-ttu-id="45fa0-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="45fa0-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45fa0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45fa0-120">Request headers</span></span>
| <span data-ttu-id="45fa0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="45fa0-121">Name</span></span>      |<span data-ttu-id="45fa0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="45fa0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="45fa0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45fa0-123">Authorization</span></span>  | <span data-ttu-id="45fa0-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="45fa0-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="45fa0-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45fa0-125">Request body</span></span>
<span data-ttu-id="45fa0-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45fa0-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="45fa0-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="45fa0-127">Response</span></span>
<span data-ttu-id="45fa0-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [governanceResource](../resources/governanceresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45fa0-128">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="45fa0-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="45fa0-129">Examples</span></span>

<span data-ttu-id="45fa0-130">В этом примере выводится список всех ресурсов, к которым я могу получить доступ.</span><span class="sxs-lookup"><span data-stu-id="45fa0-130">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="45fa0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="45fa0-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="45fa0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="45fa0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
# <a name="c"></a>[<span data-ttu-id="45fa0-133">C#</span><span class="sxs-lookup"><span data-stu-id="45fa0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-governanceresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45fa0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45fa0-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-governanceresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45fa0-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45fa0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-governanceresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="45fa0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="45fa0-136">Response</span></span>
<span data-ttu-id="45fa0-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="45fa0-137">Here is an example of the response.</span></span> 

><span data-ttu-id="45fa0-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45fa0-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
