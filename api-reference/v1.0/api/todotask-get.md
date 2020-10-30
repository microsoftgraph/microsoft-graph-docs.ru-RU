---
title: Получение Тодотаск
description: Чтение свойств и связей объекта Тодотаск.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 58a3f1da44698d23bbfff1e0b31b5798929c17fa
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797345"
---
# <a name="get-todotask"></a><span data-ttu-id="a3446-103">Получение Тодотаск</span><span class="sxs-lookup"><span data-stu-id="a3446-103">Get todoTask</span></span>
<span data-ttu-id="a3446-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3446-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a3446-105">Чтение свойств и связей объекта [тодотаск](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="a3446-105">Read the properties and relationships of a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3446-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3446-106">Permissions</span></span>
<span data-ttu-id="a3446-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3446-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3446-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3446-109">Permission type</span></span>|<span data-ttu-id="a3446-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3446-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3446-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3446-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a3446-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3446-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="a3446-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3446-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3446-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3446-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="a3446-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3446-115">Application</span></span>|<span data-ttu-id="a3446-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3446-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3446-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3446-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3446-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a3446-118">Optional query parameters</span></span>
<span data-ttu-id="a3446-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a3446-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a3446-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a3446-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3446-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3446-121">Request headers</span></span>
|<span data-ttu-id="a3446-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a3446-122">Name</span></span>|<span data-ttu-id="a3446-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a3446-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a3446-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3446-124">Authorization</span></span>|<span data-ttu-id="a3446-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3446-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3446-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3446-127">Request body</span></span>
<span data-ttu-id="a3446-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3446-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3446-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3446-129">Response</span></span>

<span data-ttu-id="a3446-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тодотаск](../resources/todotask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a3446-130">If successful, this method returns a `200 OK` response code and a [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a3446-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="a3446-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a3446-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3446-132">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "get_todotask"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```


### <a name="response"></a><span data-ttu-id="a3446-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3446-133">Response</span></span>
<span data-ttu-id="a3446-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a3446-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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



