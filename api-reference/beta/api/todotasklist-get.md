---
title: Get todoTaskList
description: Чтение свойств и связей объекта todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d617ac83bb5a6c42ac628fe4c23c9aa3701cb60f
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46850056"
---
# <a name="get-todotasklist"></a><span data-ttu-id="028fa-103">Get todoTaskList</span><span class="sxs-lookup"><span data-stu-id="028fa-103">Get todoTaskList</span></span>
<span data-ttu-id="028fa-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="028fa-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="028fa-105">Чтение свойств и связей объекта [todoTaskList.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="028fa-105">Read the properties and relationships of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="028fa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="028fa-106">Permissions</span></span>
<span data-ttu-id="028fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="028fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="028fa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="028fa-109">Permission type</span></span>|<span data-ttu-id="028fa-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="028fa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="028fa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="028fa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="028fa-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="028fa-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="028fa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="028fa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="028fa-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="028fa-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="028fa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="028fa-115">Application</span></span>|<span data-ttu-id="028fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="028fa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="028fa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="028fa-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="028fa-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="028fa-118">Optional query parameters</span></span>
<span data-ttu-id="028fa-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="028fa-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="028fa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="028fa-120">Request headers</span></span>
|<span data-ttu-id="028fa-121">Имя</span><span class="sxs-lookup"><span data-stu-id="028fa-121">Name</span></span>|<span data-ttu-id="028fa-122">Описание</span><span class="sxs-lookup"><span data-stu-id="028fa-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="028fa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="028fa-123">Authorization</span></span>|<span data-ttu-id="028fa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="028fa-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="028fa-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="028fa-126">Request body</span></span>
<span data-ttu-id="028fa-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="028fa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="028fa-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="028fa-128">Response</span></span>

<span data-ttu-id="028fa-129">При успешном выполнении этот метод возвращает код `200 OK` ответа [и объект todoTaskList](../resources/todotasklist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="028fa-129">If successful, this method returns a `200 OK` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="028fa-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="028fa-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="028fa-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="028fa-131">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAAABrJAAA="],
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/AAMkADIyAAAAABrJAAA=
```


### <a name="response"></a><span data-ttu-id="028fa-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="028fa-132">Response</span></span>
<span data-ttu-id="028fa-133">**Примечание.** Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="028fa-133">**Note:** Here is an example of the response.</span></span> <span data-ttu-id="028fa-134">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="028fa-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="028fa-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="028fa-135">All of the properties will be returned from an actual call..</span></span>
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

