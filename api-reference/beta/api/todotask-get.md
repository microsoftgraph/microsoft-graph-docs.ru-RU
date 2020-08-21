---
title: Вывод задачи todoTask
description: Чтение свойств и связей объекта todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 41176f6e764cc1640eede00406208045f1e7e5f1
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46850068"
---
# <a name="get-todotask"></a><span data-ttu-id="8580b-103">Вывод задачи todoTask</span><span class="sxs-lookup"><span data-stu-id="8580b-103">Get todoTask</span></span>
<span data-ttu-id="8580b-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="8580b-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="8580b-105">Чтение свойств и связей объекта [todoTask.](../resources/todotask.md)</span><span class="sxs-lookup"><span data-stu-id="8580b-105">Read the properties and relationships of a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8580b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8580b-106">Permissions</span></span>
<span data-ttu-id="8580b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8580b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8580b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8580b-109">Permission type</span></span>|<span data-ttu-id="8580b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8580b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8580b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8580b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8580b-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8580b-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="8580b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8580b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8580b-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8580b-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="8580b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8580b-115">Application</span></span>|<span data-ttu-id="8580b-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8580b-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="8580b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8580b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8580b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8580b-118">Optional query parameters</span></span>
<span data-ttu-id="8580b-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8580b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8580b-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8580b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8580b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8580b-121">Request headers</span></span>
|<span data-ttu-id="8580b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8580b-122">Name</span></span>|<span data-ttu-id="8580b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8580b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8580b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8580b-124">Authorization</span></span>|<span data-ttu-id="8580b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8580b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8580b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8580b-127">Request body</span></span>
<span data-ttu-id="8580b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8580b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8580b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8580b-129">Response</span></span>

<span data-ttu-id="8580b-130">При успешном выполнении этот метод возвращает код `200 OK` ответа [и объект todoTask](../resources/todotask.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8580b-130">If successful, this method returns a `200 OK` response code and a [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8580b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="8580b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8580b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8580b-132">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "get_todotask"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```


### <a name="response"></a><span data-ttu-id="8580b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8580b-133">Response</span></span>
<span data-ttu-id="8580b-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8580b-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.todoTask"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tasks/$entity",
    "@odata.etag": "W/\"s8/ERWT3WEeFpBGD0bDgAA+TWq9g==\"",
    "importance": "low",
    "isReminderOn": false,
    "status": "notStarted",
    "title": "Shop for dinner",
    "createdDateTime": "2020-07-22T10:39:03.7937971Z",
    "lastModifiedDateTime": "2020-07-22T12:02:10.8835421Z",
    "id": "721a35e2-35e2-721a-e235-1a72e2351a72",
    "body": {
        "content": "",
        "contentType": "text"
    },
    "dueDateTime": {
        "dateTime": "2020-08-25T04:00:00.0000000",
        "timeZone": "UTC"
    }
}
```

