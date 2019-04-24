---
title: Экспорт Говернанцеролеассигнментрекуестс
description: Получение коллекции Говернанцеролеассигнментрекуестс в формате `application/octet-stream`, который можно проанализировать как CSV-файл в браузере.
localization_priority: Normal
ms.openlocfilehash: 82c36f176dfed1a4a848c045ce3274e1152bb953
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457177"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="979dc-103">Экспорт Говернанцеролеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="979dc-103">Export governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="979dc-104">Получение коллекции [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md) в формате `application/octet-stream`, который можно проанализировать как CSV-файл в браузере.</span><span class="sxs-lookup"><span data-stu-id="979dc-104">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="979dc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="979dc-105">Permissions</span></span>
<span data-ttu-id="979dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="979dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="979dc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="979dc-108">Permission type</span></span>      | <span data-ttu-id="979dc-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="979dc-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="979dc-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="979dc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="979dc-111">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="979dc-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="979dc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="979dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="979dc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="979dc-113">Not supported.</span></span>    |
|<span data-ttu-id="979dc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="979dc-114">Application</span></span> | <span data-ttu-id="979dc-115">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="979dc-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="979dc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="979dc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="979dc-117">Экспорт коллекции [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md) для ресурса</span><span class="sxs-lookup"><span data-stu-id="979dc-117">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="979dc-118">**Примечание:** Кроме области разрешений, этот запрос требует, чтобы запрашивающая сторона состроила по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="979dc-118">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="979dc-119">Экспорт коллекции [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="979dc-119">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="979dc-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="979dc-120">Optional query parameters</span></span>
<span data-ttu-id="979dc-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="979dc-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="979dc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="979dc-122">Request headers</span></span>
| <span data-ttu-id="979dc-123">Имя</span><span class="sxs-lookup"><span data-stu-id="979dc-123">Name</span></span>      |<span data-ttu-id="979dc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="979dc-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="979dc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="979dc-125">Authorization</span></span>  | <span data-ttu-id="979dc-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="979dc-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="979dc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="979dc-127">Request body</span></span>
<span data-ttu-id="979dc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="979dc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="979dc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="979dc-129">Response</span></span>
<span data-ttu-id="979dc-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и содержимое `application/octet-stream`типа.</span><span class="sxs-lookup"><span data-stu-id="979dc-130">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="979dc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="979dc-131">Example</span></span>
<span data-ttu-id="979dc-132">В этом примере все назначения ролей сохраняются в виде CSV-файла в подписке Wingtip Toys-произ.</span><span class="sxs-lookup"><span data-stu-id="979dc-132">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="979dc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="979dc-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="979dc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="979dc-134">Response</span></span>
<span data-ttu-id="979dc-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="979dc-135">Here is an example of the response.</span></span> 
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
