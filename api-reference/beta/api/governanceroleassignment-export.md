---
title: Экспорт governanceRoleAssignmentRequests
description: Получить коллекцию governanceRoleAssignmentRequests в формате `application/octet-stream`, который можно преобразовать в файл CSV в браузере.
localization_priority: Normal
ms.openlocfilehash: 82c36f176dfed1a4a848c045ce3274e1152bb953
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522429"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="dddec-103">Экспорт governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="dddec-103">Export governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dddec-104">Получить коллекцию [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) в формате `application/octet-stream`, который можно преобразовать в файл CSV в браузере.</span><span class="sxs-lookup"><span data-stu-id="dddec-104">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="dddec-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dddec-105">Permissions</span></span>
<span data-ttu-id="dddec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dddec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dddec-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dddec-108">Permission type</span></span>      | <span data-ttu-id="dddec-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dddec-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dddec-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dddec-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dddec-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="dddec-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="dddec-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dddec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dddec-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dddec-113">Not supported.</span></span>    |
|<span data-ttu-id="dddec-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dddec-114">Application</span></span> | <span data-ttu-id="dddec-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="dddec-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="dddec-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dddec-116">HTTP request</span></span>
<span data-ttu-id="dddec-117"><!-- { "blockType": "ignored" } -->Экспорт коллекции [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) на ресурс</span><span class="sxs-lookup"><span data-stu-id="dddec-117"><!-- { "blockType": "ignored" } --> Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="dddec-118">**Примечание:** Помимо области разрешений для этого запроса требуется инициатор запроса может иметь по крайней мере одна роль назначения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="dddec-118">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="dddec-119">Экспорт коллекции [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) Мой</span><span class="sxs-lookup"><span data-stu-id="dddec-119">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dddec-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dddec-120">Optional query parameters</span></span>
<span data-ttu-id="dddec-121">Этот метод поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="dddec-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dddec-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dddec-122">Request headers</span></span>
| <span data-ttu-id="dddec-123">Имя</span><span class="sxs-lookup"><span data-stu-id="dddec-123">Name</span></span>      |<span data-ttu-id="dddec-124">Описание</span><span class="sxs-lookup"><span data-stu-id="dddec-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dddec-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="dddec-125">Authorization</span></span>  | <span data-ttu-id="dddec-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="dddec-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="dddec-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dddec-127">Request body</span></span>
<span data-ttu-id="dddec-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dddec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dddec-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="dddec-129">Response</span></span>
<span data-ttu-id="dddec-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и содержимое типа `application/octet-stream`.</span><span class="sxs-lookup"><span data-stu-id="dddec-130">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="dddec-131">Пример</span><span class="sxs-lookup"><span data-stu-id="dddec-131">Example</span></span>
<span data-ttu-id="dddec-132">В этом примере сохраняет все назначения ролей в виде CSV-файла в подписке Wingtip Toys - производственного.</span><span class="sxs-lookup"><span data-stu-id="dddec-132">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="dddec-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="dddec-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="dddec-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="dddec-134">Response</span></span>
<span data-ttu-id="dddec-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dddec-135">Here is an example of the response.</span></span> 
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
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignment-export.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
