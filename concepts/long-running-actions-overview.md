---
title: Работа с действиями, выполняющимися длительное время (бета-версия)
description: В этой статье описаны принципы работы с действиями, выполняющимися длительное время.
localization_priority: Normal
author: daspek
ms.openlocfilehash: 4512672ea44e944fd77e95249aa439f0ee9e84ba
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560783"
---
# <a name="working-with-long-running-actions-beta"></a><span data-ttu-id="127b4-103">Работа с действиями, выполняющимися длительное время (бета-версия)</span><span class="sxs-lookup"><span data-stu-id="127b4-103">Working with long running actions (beta)</span></span>


<span data-ttu-id="127b4-104">Для выполнения некоторых запросов API требуется неопределенное время.</span><span class="sxs-lookup"><span data-stu-id="127b4-104">Some API responses require indeterminate time to complete.</span></span>
<span data-ttu-id="127b4-105">Вместо того чтобы ожидать завершения действия перед возвращением ответа, Microsoft Graph может использовать шаблон действий, выполняющихся длительное время.</span><span class="sxs-lookup"><span data-stu-id="127b4-105">Instead of waiting until the action is complete before returning a response, Microsoft Graph may use a long running actions pattern.</span></span>
<span data-ttu-id="127b4-106">При использовании этого шаблона вашему приложению предоставляется время для выполнения опроса об изменениях состояния для действия, выполняющегося длительное время, и запросу не нужно ожидать завершения действия.</span><span class="sxs-lookup"><span data-stu-id="127b4-106">This pattern provides your app a wait to poll for status updates on a long running action, without any request waiting for the action to complete.</span></span>

<span data-ttu-id="127b4-107">В стандартном шаблоне выполняются следующие действия:</span><span class="sxs-lookup"><span data-stu-id="127b4-107">The general pattern follows these steps:</span></span>

1. <span data-ttu-id="127b4-108">Ваше приложение запрашивает действие, выполняющееся длительное время, через API.</span><span class="sxs-lookup"><span data-stu-id="127b4-108">Your app requests a long running action via the API.</span></span> <span data-ttu-id="127b4-109">API принимает действие и возвращает ответ `202 Accepted` вместе с заголовком Location для URL-адреса API, чтобы можно было получать отчеты о состоянии действия.</span><span class="sxs-lookup"><span data-stu-id="127b4-109">The API accepts the action and returns a `202 Accepted` response along with a Location header for the API URL to retrieve action status reports.</span></span>
2. <span data-ttu-id="127b4-110">Ваше приложение запрашивает URL-адрес отчета о состоянии действия и получает ответ [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) со сведениями о ходе выполнения действия, выполняющегося длительное время.</span><span class="sxs-lookup"><span data-stu-id="127b4-110">Your app requests the action status report URL and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response with the progress of the long running action.</span></span>
3. <span data-ttu-id="127b4-111">Действие, выполняющееся длительное время, завершается.</span><span class="sxs-lookup"><span data-stu-id="127b4-111">The long running action completes.</span></span> 
4. <span data-ttu-id="127b4-112">Приложение еще раз запрашивает URL-адрес отчета о состоянии действия и получает ответ [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta), в котором сообщается о завершении действия.</span><span class="sxs-lookup"><span data-stu-id="127b4-112">Your app requests the action status report URL again and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response showing the completion of the action.</span></span>

## <a name="initial-action-request"></a><span data-ttu-id="127b4-113">Начальный запрос действия</span><span class="sxs-lookup"><span data-stu-id="127b4-113">Initial action request</span></span>

<span data-ttu-id="127b4-114">Давайте по шагам рассмотрим пример сценария [копирования ресурса DriveItem](/graph/api/driveitem-copy?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="127b4-114">Let's walk through the steps for an example [DriveItem Copy](/graph/api/driveitem-copy?view=graph-rest-beta) scenario.</span></span>
<span data-ttu-id="127b4-115">В этом сценарии приложение запрашивает операцию копирования папки, в которой содержится большое количество данных.</span><span class="sxs-lookup"><span data-stu-id="127b4-115">In this scenario, your app requests to copy a folder that contains a large amount of data.</span></span>
<span data-ttu-id="127b4-116">На выполнение этого запроса, вероятно, потребуется несколько секунд, так как необходимо передать большой объем данных.</span><span class="sxs-lookup"><span data-stu-id="127b4-116">This request will likely take several seconds to complete since the amount of data is large.</span></span>

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

<span data-ttu-id="127b4-117">API отправляет ответ о том, что действие принято, и URL-адрес для получения сведений о состоянии действия, выполняющегося длительное время.</span><span class="sxs-lookup"><span data-stu-id="127b4-117">The API responds that the action was accepted and the URL for retrieving the status of the long running action.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="127b4-118">**Примечание.** Возвращаемый URL-адрес расположения, возможно, не будет соответствовать конечной точке API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="127b4-118">**Note:** The location URL returned may not be on the Microsoft Graph API endpoint.</span></span>

<span data-ttu-id="127b4-119">Во многих случаях это может быть завершением запроса, так как действие копирования будет выполняться без каких-либо дополнительных действий со стороны приложения.</span><span class="sxs-lookup"><span data-stu-id="127b4-119">In many cases this may be the end of the request, since the copy action will complete without the app doing any additional work.</span></span>
<span data-ttu-id="127b4-120">Тем не менее если вашему приложению необходимо отображать состояние действия копирования или убедиться, что действие выполнено без ошибок, приложение может сделать это, используя URL-адрес для отслеживания.</span><span class="sxs-lookup"><span data-stu-id="127b4-120">However, if your app needs to show the status of the copy action or ensure that it completes without error, it can do so using the monitor URL.</span></span>

## <a name="retrieve-a-status-report-from-the-monitor-url"></a><span data-ttu-id="127b4-121">Получение отчета о состоянии с URL-адреса для отслеживания</span><span class="sxs-lookup"><span data-stu-id="127b4-121">Retrieve a status report from the monitor URL</span></span>

<span data-ttu-id="127b4-p105">Чтобы проверить состояние действия копирования, приложение отправляет запрос на URL-адрес, указанный в предыдущем ответе. *Примечание.* Для этого запроса не нужно выполнять аутентификацию, так как этот URL-адрес действует в течение небольшого времени и является уникальным для исходного вызывающего объекта.</span><span class="sxs-lookup"><span data-stu-id="127b4-p105">To check on the status of the copy action, the app makes a request to the URL provided in the previous response. *Note:* This request does not require authentication, since the URL is short-lived and unique to the original caller.</span></span> 

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="127b4-124">Служба возвращает ответ со сведениями о том, что действие, выполняющееся длительное время, еще не завершено:</span><span class="sxs-lookup"><span data-stu-id="127b4-124">The service responses with information that the long running action is still in progress:</span></span>

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

<span data-ttu-id="127b4-p106">Эти сведения можно использовать для обновления информации о ходе копирования для пользователя. Приложение может опрашивать URL-адрес для отслеживания и получать обновленные сведения о ходе выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="127b4-p106">This information can be used to provide an update to the user about the progress of the copy action. The app can continue to poll the monitor URL to request status updates and keep track of the progress of the action.</span></span>

## <a name="retrieve-a-completed-status-report-from-the-monitor-url"></a><span data-ttu-id="127b4-127">Получение отчета о выполнении действия с URL-адреса для отслеживания</span><span class="sxs-lookup"><span data-stu-id="127b4-127">Retrieve a completed status report from the monitor URL</span></span>

<span data-ttu-id="127b4-p107">Через несколько секунд операция копирования завершается. На этот раз, когда приложение отправляет запрос на URL-для отслеживания, ответом будет перенаправление на результат выполненного действия.</span><span class="sxs-lookup"><span data-stu-id="127b4-p107">After a few seconds the copy operation has completed. This time when the app makes a request to the monitor URL the response is a redirection to the finished result of the action.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="127b4-130">По завершении действия в отклике службы отслеживания будет возвращен идентификатор ресурса для результатов.</span><span class="sxs-lookup"><span data-stu-id="127b4-130">When the action has completed, the response from the monitor service will return the resourceId for the results.</span></span>

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

## <a name="retrieve-the-results-of-the-completed-operation"></a><span data-ttu-id="127b4-131">Получение результатов выполненной операции</span><span class="sxs-lookup"><span data-stu-id="127b4-131">Retrieve the results of the completed operation</span></span>

<span data-ttu-id="127b4-132">После завершения задания URL-адрес для отслеживания возвращает идентификатор ресурса результата (в данном случае новую копию исходного элемента).</span><span class="sxs-lookup"><span data-stu-id="127b4-132">Once the job has completed, the monitor URL returns the resourceId of the result, in this case the new copy of the original item.</span></span>
<span data-ttu-id="127b4-133">Вы можете обратиться к этому новому элементу с использованием идентификатора ресурса, например:</span><span class="sxs-lookup"><span data-stu-id="127b4-133">You can address this new item using the resourceId, for example:</span></span>

<!-- {
  "blockType": "request",
  "name": "lro-copy-item-example-complete",
  "scopes": "files.readwrite"
} -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}
```

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

## <a name="supported-resources"></a><span data-ttu-id="127b4-134">Поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="127b4-134">Supported resources</span></span>

<span data-ttu-id="127b4-135">Действия, выполняющиеся длительное время, поддерживаются в указанных ниже методах API</span><span class="sxs-lookup"><span data-stu-id="127b4-135">Long running actions are supported on the following API methods</span></span>

| <span data-ttu-id="127b4-136">**Ресурс**</span><span class="sxs-lookup"><span data-stu-id="127b4-136">**Resource**</span></span> | <span data-ttu-id="127b4-137">**API**</span><span class="sxs-lookup"><span data-stu-id="127b4-137">**API**</span></span> |
|:------ | :------ |
| <span data-ttu-id="127b4-138">DriveItem</span><span class="sxs-lookup"><span data-stu-id="127b4-138">DriveItem</span></span> | [<span data-ttu-id="127b4-139">Copy</span><span class="sxs-lookup"><span data-stu-id="127b4-139">Copy</span></span>](/graph/api/driveitem-copy?view=graph-rest-beta) |

## <a name="prerequisites"></a><span data-ttu-id="127b4-140">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="127b4-140">Prerequisites</span></span>

<span data-ttu-id="127b4-141">Для запроса сведений о состоянии действия, выполняющегося длительное время, необходимы такие же [разрешения](./permissions-reference.md), что и для самого действия, выполняющегося длительное время.</span><span class="sxs-lookup"><span data-stu-id="127b4-141">The same [permissions](./permissions-reference.md) that are required to perform a long running action are also required to query the status of a long running action.</span></span>




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
