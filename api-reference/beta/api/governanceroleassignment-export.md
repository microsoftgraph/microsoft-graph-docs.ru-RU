---
title: Экспорт governanceRoleAssignmentRequests
description: Получить коллекцию governanceRoleAssignmentRequests в формате `application/octet-stream`, который можно преобразовать в файл CSV в браузере.
localization_priority: Normal
ms.openlocfilehash: 10fd7c720bf7b6f162a4d8c2189e81a9205e53ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828730"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="f5ffd-103">Экспорт governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="f5ffd-103">Export governanceRoleAssignmentRequests</span></span>

> <span data-ttu-id="f5ffd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f5ffd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5ffd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5ffd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5ffd-106">Получить коллекцию [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) в формате `application/octet-stream`, который можно преобразовать в файл CSV в браузере.</span><span class="sxs-lookup"><span data-stu-id="f5ffd-106">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5ffd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5ffd-107">Permissions</span></span>
<span data-ttu-id="f5ffd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5ffd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5ffd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5ffd-110">Permission type</span></span>      | <span data-ttu-id="f5ffd-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="f5ffd-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5ffd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5ffd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f5ffd-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f5ffd-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="f5ffd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5ffd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5ffd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5ffd-115">Not supported.</span></span>    |
|<span data-ttu-id="f5ffd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5ffd-116">Application</span></span> | <span data-ttu-id="f5ffd-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f5ffd-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="f5ffd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5ffd-118">HTTP request</span></span>
<span data-ttu-id="f5ffd-119"><!-- { "blockType": "ignored" } -->Экспорт коллекции [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) на ресурс</span><span class="sxs-lookup"><span data-stu-id="f5ffd-119"><!-- { "blockType": "ignored" } --> Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="f5ffd-120">**Примечание:** Помимо области разрешений для этого запроса требуется инициатор запроса может иметь по крайней мере одна роль назначения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="f5ffd-120">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="f5ffd-121">Экспорт коллекции [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) Мой</span><span class="sxs-lookup"><span data-stu-id="f5ffd-121">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f5ffd-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f5ffd-122">Optional query parameters</span></span>
<span data-ttu-id="f5ffd-123">Этот метод поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="f5ffd-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5ffd-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5ffd-124">Request headers</span></span>
| <span data-ttu-id="f5ffd-125">Имя</span><span class="sxs-lookup"><span data-stu-id="f5ffd-125">Name</span></span>      |<span data-ttu-id="f5ffd-126">Описание</span><span class="sxs-lookup"><span data-stu-id="f5ffd-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f5ffd-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5ffd-127">Authorization</span></span>  | <span data-ttu-id="f5ffd-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f5ffd-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5ffd-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f5ffd-129">Request body</span></span>
<span data-ttu-id="f5ffd-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f5ffd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5ffd-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="f5ffd-131">Response</span></span>
<span data-ttu-id="f5ffd-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и содержимое типа `application/octet-stream`.</span><span class="sxs-lookup"><span data-stu-id="f5ffd-132">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="f5ffd-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f5ffd-133">Example</span></span>
<span data-ttu-id="f5ffd-134">В этом примере сохраняет все назначения ролей в виде CSV-файла в подписке Wingtip Toys - производственного.</span><span class="sxs-lookup"><span data-stu-id="f5ffd-134">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="f5ffd-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5ffd-135">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="f5ffd-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f5ffd-136">Response</span></span>
<span data-ttu-id="f5ffd-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f5ffd-137">Here is an example of the response.</span></span> 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
