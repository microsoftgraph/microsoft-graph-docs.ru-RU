---
title: Работа с действиями, выполняющимися длительное время (бета-версия)
description: В этой статье описаны принципы работы с действиями, выполняющимися длительное время.
localization_priority: Normal
author: daspek
ms.openlocfilehash: 9623dce367514d86e7dc84df672578cd2a77fad3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332003"
---
# <a name="working-with-long-running-actions-beta"></a><span data-ttu-id="419cd-103">Работа с действиями, выполняющимися длительное время (бета-версия)</span><span class="sxs-lookup"><span data-stu-id="419cd-103">Working with long running actions (beta)</span></span>


<span data-ttu-id="419cd-104">Для выполнения некоторых запросов API требуется неопределенное время.</span><span class="sxs-lookup"><span data-stu-id="419cd-104">Some API responses require indeterminate time to complete.</span></span>
<span data-ttu-id="419cd-105">Вместо того чтобы ожидать завершения действия перед возвращением ответа, Microsoft Graph может использовать шаблон действий, выполняющихся длительное время.</span><span class="sxs-lookup"><span data-stu-id="419cd-105">Instead of waiting until the action is complete before returning a response, Microsoft Graph may use a long running actions pattern.</span></span>
<span data-ttu-id="419cd-106">При использовании этого шаблона вашему приложению предоставляется время для выполнения опроса об изменениях состояния для действия, выполняющегося длительное время, и запросу не нужно ожидать завершения действия.</span><span class="sxs-lookup"><span data-stu-id="419cd-106">This pattern provides your app a wait to poll for status updates on a long running action, without any request waiting for the action to complete.</span></span>

<span data-ttu-id="419cd-107">В стандартном шаблоне выполняются следующие действия:</span><span class="sxs-lookup"><span data-stu-id="419cd-107">The general pattern follows these steps:</span></span>

1. <span data-ttu-id="419cd-108">Ваше приложение запрашивает действие, выполняющееся длительное время, через API.</span><span class="sxs-lookup"><span data-stu-id="419cd-108">Your app requests a long running action via the API.</span></span> <span data-ttu-id="419cd-109">API принимает действие и возвращает ответ `202 Accepted` вместе с заголовком Location для URL-адреса API, чтобы можно было получать отчеты о состоянии действия.</span><span class="sxs-lookup"><span data-stu-id="419cd-109">The API accepts the action and returns a `202 Accepted` response along with a Location header for the API URL to retrieve action status reports.</span></span>
2. <span data-ttu-id="419cd-110">Ваше приложение запрашивает URL-адрес отчета о состоянии действия и получает ответ [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) со сведениями о ходе выполнения действия, выполняющегося длительное время.</span><span class="sxs-lookup"><span data-stu-id="419cd-110">Your app requests the action status report URL and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response with the progress of the long running action.</span></span>
3. <span data-ttu-id="419cd-111">Действие, выполняющееся длительное время, завершается.</span><span class="sxs-lookup"><span data-stu-id="419cd-111">The long running action completes.</span></span> 
4. <span data-ttu-id="419cd-112">Приложение еще раз запрашивает URL-адрес отчета о состоянии действия и получает ответ [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta), в котором сообщается о завершении действия.</span><span class="sxs-lookup"><span data-stu-id="419cd-112">Your app requests the action status report URL again and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response showing the completion of the action.</span></span>

## <a name="initial-action-request"></a><span data-ttu-id="419cd-113">Начальный запрос действия</span><span class="sxs-lookup"><span data-stu-id="419cd-113">Initial action request</span></span>

<span data-ttu-id="419cd-114">Давайте по шагам рассмотрим пример сценария [копирования ресурса DriveItem](/graph/api/driveitem-copy?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="419cd-114">Let's walk through the steps for an example [DriveItem Copy](/graph/api/driveitem-copy?view=graph-rest-beta) scenario.</span></span>
<span data-ttu-id="419cd-115">В этом сценарии приложение запрашивает операцию копирования папки, в которой содержится большое количество данных.</span><span class="sxs-lookup"><span data-stu-id="419cd-115">In this scenario, your app requests to copy a folder that contains a large amount of data.</span></span>
<span data-ttu-id="419cd-116">На выполнение этого запроса, вероятно, потребуется несколько секунд, так как необходимо передать большой объем данных.</span><span class="sxs-lookup"><span data-stu-id="419cd-116">This request will likely take several seconds to complete since the amount of data is large.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="419cd-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="419cd-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "lro-copy-item-example", "scopes": "files.readwrite" } -->

```http
POST https://graph.microsoft.com/beta/me/drive/items/{folder-item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "Copy of LargeFolder1"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="419cd-118">C#</span><span class="sxs-lookup"><span data-stu-id="419cd-118">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/lro-copy-item-example-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="419cd-119">JavaScript</span><span class="sxs-lookup"><span data-stu-id="419cd-119">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/lro-copy-item-example-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="419cd-120">Цель — C</span><span class="sxs-lookup"><span data-stu-id="419cd-120">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/lro-copy-item-example-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="419cd-121">Java</span><span class="sxs-lookup"><span data-stu-id="419cd-121">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/lro-copy-item-example-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="419cd-122">API отправляет ответ о том, что действие принято, и URL-адрес для получения сведений о состоянии действия, выполняющегося длительное время.</span><span class="sxs-lookup"><span data-stu-id="419cd-122">The API responds that the action was accepted and the URL for retrieving the status of the long running action.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="419cd-123">**Примечание.** Возвращаемый URL-адрес расположения, возможно, не будет соответствовать конечной точке API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="419cd-123">**Note:** The location URL returned may not be on the Microsoft Graph API endpoint.</span></span>

<span data-ttu-id="419cd-124">Во многих случаях это может быть завершением запроса, так как действие копирования будет выполняться без каких-либо дополнительных действий со стороны приложения.</span><span class="sxs-lookup"><span data-stu-id="419cd-124">In many cases this may be the end of the request, since the copy action will complete without the app doing any additional work.</span></span>
<span data-ttu-id="419cd-125">Тем не менее если вашему приложению необходимо отображать состояние действия копирования или убедиться, что действие выполнено без ошибок, приложение может сделать это, используя URL-адрес для отслеживания.</span><span class="sxs-lookup"><span data-stu-id="419cd-125">However, if your app needs to show the status of the copy action or ensure that it completes without error, it can do so using the monitor URL.</span></span>

## <a name="retrieve-a-status-report-from-the-monitor-url"></a><span data-ttu-id="419cd-126">Получение отчета о состоянии с URL-адреса для отслеживания</span><span class="sxs-lookup"><span data-stu-id="419cd-126">Retrieve a status report from the monitor URL</span></span>

<span data-ttu-id="419cd-p105">Чтобы проверить состояние действия копирования, приложение отправляет запрос на URL-адрес, указанный в предыдущем ответе. *Примечание.* Для этого запроса не нужно выполнять аутентификацию, так как этот URL-адрес действует в течение небольшого времени и является уникальным для исходного вызывающего объекта.</span><span class="sxs-lookup"><span data-stu-id="419cd-p105">To check on the status of the copy action, the app makes a request to the URL provided in the previous response. *Note:* This request does not require authentication, since the URL is short-lived and unique to the original caller.</span></span> 

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="419cd-129">Служба возвращает ответ со сведениями о том, что действие, выполняющееся длительное время, еще не завершено:</span><span class="sxs-lookup"><span data-stu-id="419cd-129">The service responses with information that the long running action is still in progress:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
  "operation": "ItemCopy",
  "percentageComplete": 27.8,
  "status": "inProgress"
}
```

<span data-ttu-id="419cd-p106">Эти сведения можно использовать для обновления информации о ходе копирования для пользователя. Приложение может опрашивать URL-адрес для отслеживания и получать обновленные сведения о ходе выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="419cd-p106">This information can be used to provide an update to the user about the progress of the copy action. The app can continue to poll the monitor URL to request status updates and keep track of the progress of the action.</span></span>

## <a name="retrieve-a-completed-status-report-from-the-monitor-url"></a><span data-ttu-id="419cd-132">Получение отчета о выполнении действия с URL-адреса для отслеживания</span><span class="sxs-lookup"><span data-stu-id="419cd-132">Retrieve a completed status report from the monitor URL</span></span>

<span data-ttu-id="419cd-p107">Через несколько секунд операция копирования завершается. На этот раз, когда приложение отправляет запрос на URL-для отслеживания, ответом будет перенаправление на результат выполненного действия.</span><span class="sxs-lookup"><span data-stu-id="419cd-p107">After a few seconds the copy operation has completed. This time when the app makes a request to the monitor URL the response is a redirection to the finished result of the action.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="419cd-135">По завершении действия в отклике службы отслеживания будет возвращен идентификатор ресурса для результатов.</span><span class="sxs-lookup"><span data-stu-id="419cd-135">When the action has completed, the response from the monitor service will return the resourceId for the results.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
    "percentageComplete": 100.0,
    "resourceId": "01MOWKYVJML57KN2ANMBA3JZJS2MBGC7KM",
    "status": "completed"
}
```

## <a name="retrieve-the-results-of-the-completed-operation"></a><span data-ttu-id="419cd-136">Получение результатов выполненной операции</span><span class="sxs-lookup"><span data-stu-id="419cd-136">Retrieve the results of the completed operation</span></span>

<span data-ttu-id="419cd-137">После завершения задания URL-адрес для отслеживания возвращает идентификатор ресурса результата (в данном случае новую копию исходного элемента).</span><span class="sxs-lookup"><span data-stu-id="419cd-137">Once the job has completed, the monitor URL returns the resourceId of the result, in this case the new copy of the original item.</span></span>
<span data-ttu-id="419cd-138">Вы можете обратиться к этому новому элементу с использованием идентификатора ресурса, например:</span><span class="sxs-lookup"><span data-stu-id="419cd-138">You can address this new item using the resourceId, for example:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="419cd-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="419cd-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "lro-copy-item-example-complete",
  "scopes": "files.readwrite"
} -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="419cd-140">C#</span><span class="sxs-lookup"><span data-stu-id="419cd-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/lro-copy-item-example-complete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="419cd-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="419cd-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/lro-copy-item-example-complete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="419cd-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="419cd-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/lro-copy-item-example-complete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="419cd-143">Java</span><span class="sxs-lookup"><span data-stu-id="419cd-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/lro-copy-item-example-complete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "",
    "name": "Copy of LargeFolder1",
    "folder": { },
    "size": 12019
}
```

## <a name="supported-resources"></a><span data-ttu-id="419cd-144">Поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="419cd-144">Supported resources</span></span>

<span data-ttu-id="419cd-145">Действия, выполняющиеся длительное время, поддерживаются в указанных ниже методах API</span><span class="sxs-lookup"><span data-stu-id="419cd-145">Long running actions are supported on the following API methods</span></span>

| <span data-ttu-id="419cd-146">**Ресурс**</span><span class="sxs-lookup"><span data-stu-id="419cd-146">**Resource**</span></span> | <span data-ttu-id="419cd-147">**API**</span><span class="sxs-lookup"><span data-stu-id="419cd-147">**API**</span></span> |
|:------ | :------ |
| <span data-ttu-id="419cd-148">DriveItem</span><span class="sxs-lookup"><span data-stu-id="419cd-148">DriveItem</span></span> | [<span data-ttu-id="419cd-149">Copy</span><span class="sxs-lookup"><span data-stu-id="419cd-149">Copy</span></span>](/graph/api/driveitem-copy?view=graph-rest-beta) |

## <a name="prerequisites"></a><span data-ttu-id="419cd-150">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="419cd-150">Prerequisites</span></span>

<span data-ttu-id="419cd-151">Для запроса сведений о состоянии действия, выполняющегося длительное время, необходимы такие же [разрешения](./permissions-reference.md), что и для самого действия, выполняющегося длительное время.</span><span class="sxs-lookup"><span data-stu-id="419cd-151">The same [permissions](./permissions-reference.md) that are required to perform a long running action are also required to query the status of a long running action.</span></span>




<!-- {
  "type": "#page.annotation",
  "description": "Monitor the progress of long-running actions in the API.",
  "keywords": "monitor,long,running,operation,action",
  "section": "documentation",
  "suppressions": [
    "Error: lro-check-status:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus",
    "Error: lro-check-status-complete:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus"
  ],
  "tocPath": "Concepts/Long running actions"
} -->
