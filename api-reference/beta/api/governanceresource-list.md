---
title: Список Говернанцересаурцес
description: Получение коллекции governanceResource, к которой у запрашивающего есть доступ.
localization_priority: Normal
ms.openlocfilehash: 998e18a0139f0cbe41901da935faee2f7f24e9eb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457181"
---
# <a name="list-governanceresources"></a><span data-ttu-id="71f04-103">Список Говернанцересаурцес</span><span class="sxs-lookup"><span data-stu-id="71f04-103">List governanceResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71f04-104">Получение коллекции [governanceResource](../resources/governanceresource.md) , к которой у запрашивающего есть доступ.</span><span class="sxs-lookup"><span data-stu-id="71f04-104">Retrieve a collection of [governanceResource](../resources/governanceresource.md) that the requestor has access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="71f04-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71f04-105">Permissions</span></span>
<span data-ttu-id="71f04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71f04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71f04-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71f04-108">Permission type</span></span>      | <span data-ttu-id="71f04-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71f04-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71f04-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71f04-110">Delegated (work or school account)</span></span> | <span data-ttu-id="71f04-111">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="71f04-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="71f04-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71f04-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71f04-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71f04-113">Not supported.</span></span>    |
|<span data-ttu-id="71f04-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71f04-114">Application</span></span> | <span data-ttu-id="71f04-115">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="71f04-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="71f04-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71f04-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="71f04-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="71f04-117">Optional query parameters</span></span>
<span data-ttu-id="71f04-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="71f04-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71f04-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71f04-119">Request headers</span></span>
| <span data-ttu-id="71f04-120">Имя</span><span class="sxs-lookup"><span data-stu-id="71f04-120">Name</span></span>      |<span data-ttu-id="71f04-121">Описание</span><span class="sxs-lookup"><span data-stu-id="71f04-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="71f04-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71f04-122">Authorization</span></span>  | <span data-ttu-id="71f04-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="71f04-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="71f04-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71f04-124">Request body</span></span>
<span data-ttu-id="71f04-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71f04-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="71f04-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="71f04-126">Response</span></span>
<span data-ttu-id="71f04-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [governanceResource](../resources/governanceresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71f04-127">If successful, this method returns a `200 OK` response code and collection of [governanceResource](../resources/governanceresource.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="71f04-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="71f04-128">Examples</span></span>

<span data-ttu-id="71f04-129">В этом примере выводится список всех ресурсов, к которым я могу получить доступ.</span><span class="sxs-lookup"><span data-stu-id="71f04-129">This example lists all resources I can currently access.</span></span>
##### <a name="request"></a><span data-ttu-id="71f04-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="71f04-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresources"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources
```
##### <a name="response"></a><span data-ttu-id="71f04-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="71f04-131">Response</span></span>
<span data-ttu-id="71f04-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="71f04-132">Here is an example of the response.</span></span> 

><span data-ttu-id="71f04-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71f04-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
