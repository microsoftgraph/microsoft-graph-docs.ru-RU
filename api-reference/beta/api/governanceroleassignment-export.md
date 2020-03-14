---
title: Экспорт Говернанцеролеассигнментрекуестс
description: Получение коллекции Говернанцеролеассигнментрекуестс в формате `application/octet-stream`, который можно проанализировать как CSV-файл в браузере.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identitiy-platform
ms.openlocfilehash: 5a4440a8a7870522e50cee7622c6ec7ef95393a9
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639858"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="d5a41-103">Экспорт Говернанцеролеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="d5a41-103">Export governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="d5a41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5a41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5a41-105">Получение коллекции [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md) в формате `application/octet-stream`, который можно проанализировать как CSV-файл в браузере.</span><span class="sxs-lookup"><span data-stu-id="d5a41-105">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5a41-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5a41-106">Permissions</span></span>
<span data-ttu-id="d5a41-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5a41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5a41-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5a41-109">Permission type</span></span>      | <span data-ttu-id="d5a41-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="d5a41-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5a41-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5a41-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d5a41-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="d5a41-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="d5a41-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5a41-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5a41-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5a41-114">Not supported.</span></span>    |
|<span data-ttu-id="d5a41-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d5a41-115">Application</span></span> | <span data-ttu-id="d5a41-116">Привилежедакцесс. Read. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="d5a41-116">PrivilegedAccess.Read.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="d5a41-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5a41-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d5a41-118">Экспорт коллекции [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md) для ресурса</span><span class="sxs-lookup"><span data-stu-id="d5a41-118">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="d5a41-119">**Примечание:** Кроме области разрешений, этот запрос требует, чтобы запрашивающая сторона состроила по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="d5a41-119">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="d5a41-120">Экспорт коллекции [говернанцеролеассигнментрекуестс](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="d5a41-120">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d5a41-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d5a41-121">Optional query parameters</span></span>
<span data-ttu-id="d5a41-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d5a41-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5a41-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5a41-123">Request headers</span></span>
| <span data-ttu-id="d5a41-124">Имя</span><span class="sxs-lookup"><span data-stu-id="d5a41-124">Name</span></span>      |<span data-ttu-id="d5a41-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d5a41-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d5a41-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5a41-126">Authorization</span></span>  | <span data-ttu-id="d5a41-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d5a41-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5a41-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5a41-128">Request body</span></span>
<span data-ttu-id="d5a41-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d5a41-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5a41-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d5a41-130">Response</span></span>
<span data-ttu-id="d5a41-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и содержимое `application/octet-stream`типа.</span><span class="sxs-lookup"><span data-stu-id="d5a41-131">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="d5a41-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d5a41-132">Example</span></span>
<span data-ttu-id="d5a41-133">В этом примере все назначения ролей сохраняются в виде CSV-файла в подписке Wingtip Toys-произ.</span><span class="sxs-lookup"><span data-stu-id="d5a41-133">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="d5a41-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5a41-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="d5a41-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5a41-135">Response</span></span>
<span data-ttu-id="d5a41-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d5a41-136">Here is an example of the response.</span></span> 
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
