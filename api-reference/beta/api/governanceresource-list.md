---
title: Список governanceResources
description: Получите коллекцию governanceResource с доступом к инициатора запроса.
localization_priority: Normal
ms.openlocfilehash: 998e18a0139f0cbe41901da935faee2f7f24e9eb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525670"
---
# <a name="list-governanceresources"></a><span data-ttu-id="f015e-103">Список governanceResources</span><span class="sxs-lookup"><span data-stu-id="f015e-103">List governanceResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f015e-104">Получите коллекцию [governanceResource](../resources/governanceresource.md) с доступом к инициатора запроса.</span><span class="sxs-lookup"><span data-stu-id="f015e-104">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="f015e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f015e-105">Permissions</span></span>
<span data-ttu-id="f015e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f015e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f015e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f015e-108">Permission type</span></span>      | <span data-ttu-id="f015e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f015e-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f015e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f015e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f015e-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f015e-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="f015e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f015e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f015e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f015e-113">Not supported.</span></span>    |
|<span data-ttu-id="f015e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f015e-114">Application</span></span> | <span data-ttu-id="f015e-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f015e-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="f015e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f015e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f015e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f015e-117">Optional query parameters</span></span>
<span data-ttu-id="f015e-118">Этот метод поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="f015e-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f015e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f015e-119">Request headers</span></span>
| <span data-ttu-id="f015e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f015e-120">Name</span></span>      |<span data-ttu-id="f015e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f015e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f015e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f015e-122">Authorization</span></span>  | <span data-ttu-id="f015e-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f015e-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f015e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f015e-124">Request body</span></span>
<span data-ttu-id="f015e-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f015e-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f015e-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="f015e-126">Response</span></span>
<span data-ttu-id="f015e-127">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [governanceResource](../resources/governanceresource.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f015e-127">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="f015e-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="f015e-128">Examples</span></span>

<span data-ttu-id="f015e-129">В этом примере выводятся все ресурсы, которые в настоящее время доступна.</span><span class="sxs-lookup"><span data-stu-id="f015e-129">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="f015e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f015e-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
##### <a name="response"></a><span data-ttu-id="f015e-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="f015e-131">Response</span></span>
<span data-ttu-id="f015e-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f015e-132">Here is an example of the response.</span></span> 

><span data-ttu-id="f015e-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f015e-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/governanceresource-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
