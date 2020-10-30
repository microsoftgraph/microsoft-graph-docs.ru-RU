---
title: Получение Тодотасклист
description: Чтение свойств и связей объекта Тодотасклист.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f7aced0d3e023eacfde6faaecc8c63836bbb44b7
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797381"
---
# <a name="get-todotasklist"></a><span data-ttu-id="e3b42-103">Получение Тодотасклист</span><span class="sxs-lookup"><span data-stu-id="e3b42-103">Get todoTaskList</span></span>
<span data-ttu-id="e3b42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3b42-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3b42-105">Чтение свойств и связей объекта [тодотасклист](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="e3b42-105">Read the properties and relationships of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3b42-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3b42-106">Permissions</span></span>
<span data-ttu-id="e3b42-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3b42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3b42-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3b42-109">Permission type</span></span>|<span data-ttu-id="e3b42-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3b42-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3b42-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3b42-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3b42-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3b42-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="e3b42-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3b42-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3b42-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3b42-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="e3b42-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3b42-115">Application</span></span>|<span data-ttu-id="e3b42-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3b42-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3b42-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3b42-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3b42-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e3b42-118">Optional query parameters</span></span>
<span data-ttu-id="e3b42-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e3b42-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3b42-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3b42-120">Request headers</span></span>
|<span data-ttu-id="e3b42-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e3b42-121">Name</span></span>|<span data-ttu-id="e3b42-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e3b42-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e3b42-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3b42-123">Authorization</span></span>|<span data-ttu-id="e3b42-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3b42-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3b42-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3b42-126">Request body</span></span>
<span data-ttu-id="e3b42-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3b42-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3b42-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3b42-128">Response</span></span>

<span data-ttu-id="e3b42-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тодотасклист](../resources/todotasklist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e3b42-129">If successful, this method returns a `200 OK` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3b42-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="e3b42-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e3b42-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3b42-131">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAAABrJAAA="],
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADIyAAAAABrJAAA=
```


### <a name="response"></a><span data-ttu-id="e3b42-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3b42-132">Response</span></span>
><span data-ttu-id="e3b42-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e3b42-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.todoTaskList"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.todoTaskList",
    "id": "5daae1ed-e1ed-5daa-ede1-aa5dede1aa5d",
    "displayName": "Monthly tasks",
    "isOwner": "true",
    "isShared": "false",
    "wellknownListName": "defaultList"
  }
}
```



