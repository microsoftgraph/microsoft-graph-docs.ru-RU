---
title: Список Линкедресаурцес
description: Получение Линкедресаурцес из свойства навигации Линкедресаурцес.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c3d780e05c71112ddabd1d5d6a64b22d6f771d40
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873260"
---
# <a name="list-linkedresources"></a><span data-ttu-id="a208b-103">Список Линкедресаурцес</span><span class="sxs-lookup"><span data-stu-id="a208b-103">List linkedResources</span></span>
<span data-ttu-id="a208b-104">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="a208b-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="a208b-105">Получение Линкедресаурцес из свойства навигации Линкедресаурцес.</span><span class="sxs-lookup"><span data-stu-id="a208b-105">Get the linkedResources from the linkedResources navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="a208b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a208b-106">Permissions</span></span>
<span data-ttu-id="a208b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a208b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a208b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a208b-109">Permission type</span></span>|<span data-ttu-id="a208b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a208b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a208b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a208b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a208b-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a208b-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="a208b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a208b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a208b-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a208b-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="a208b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a208b-115">Application</span></span>|<span data-ttu-id="a208b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a208b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a208b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a208b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a208b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a208b-118">Optional query parameters</span></span>
<span data-ttu-id="a208b-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a208b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a208b-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a208b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a208b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a208b-121">Request headers</span></span>
|<span data-ttu-id="a208b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a208b-122">Name</span></span>|<span data-ttu-id="a208b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a208b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a208b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a208b-124">Authorization</span></span>|<span data-ttu-id="a208b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a208b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a208b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a208b-127">Request body</span></span>
<span data-ttu-id="a208b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a208b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a208b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a208b-129">Response</span></span>

<span data-ttu-id="a208b-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [линкедресаурце](../resources/linkedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a208b-130">If successful, this method returns a `200 OK` response code and a collection of [linkedResource](../resources/linkedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a208b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="a208b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a208b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a208b-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a208b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a208b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
```
# <a name="c"></a>[<span data-ttu-id="a208b-134">C#</span><span class="sxs-lookup"><span data-stu-id="a208b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a208b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a208b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a208b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a208b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a208b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a208b-137">Response</span></span>
<span data-ttu-id="a208b-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a208b-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.linkedResource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.linkedResource",
      "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
      "webUrl": "http:://microsoft.com",
      "applicationName": "Microsoft",
      "displayName": "Microsoft",
      "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
    }
  ]
}
```

