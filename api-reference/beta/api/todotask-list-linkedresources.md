---
title: Список Линкедресаурцес
description: Получение Линкедресаурцес из свойства навигации Линкедресаурцес.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0c2ea4db41b75a2ea7e4107741df97630d893cb7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058594"
---
# <a name="list-linkedresources"></a><span data-ttu-id="eb724-103">Список Линкедресаурцес</span><span class="sxs-lookup"><span data-stu-id="eb724-103">List linkedResources</span></span>
<span data-ttu-id="eb724-104">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="eb724-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="eb724-105">Получение Линкедресаурцес из свойства навигации Линкедресаурцес.</span><span class="sxs-lookup"><span data-stu-id="eb724-105">Get the linkedResources from the linkedResources navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb724-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb724-106">Permissions</span></span>
<span data-ttu-id="eb724-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb724-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb724-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb724-109">Permission type</span></span>|<span data-ttu-id="eb724-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb724-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb724-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb724-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eb724-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb724-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="eb724-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb724-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb724-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb724-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="eb724-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb724-115">Application</span></span>|<span data-ttu-id="eb724-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb724-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb724-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb724-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb724-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eb724-118">Optional query parameters</span></span>
<span data-ttu-id="eb724-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="eb724-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="eb724-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="eb724-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb724-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb724-121">Request headers</span></span>
|<span data-ttu-id="eb724-122">Имя</span><span class="sxs-lookup"><span data-stu-id="eb724-122">Name</span></span>|<span data-ttu-id="eb724-123">Описание</span><span class="sxs-lookup"><span data-stu-id="eb724-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eb724-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb724-124">Authorization</span></span>|<span data-ttu-id="eb724-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb724-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb724-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb724-127">Request body</span></span>
<span data-ttu-id="eb724-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eb724-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb724-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb724-129">Response</span></span>

<span data-ttu-id="eb724-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [линкедресаурце](../resources/linkedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eb724-130">If successful, this method returns a `200 OK` response code and a collection of [linkedResource](../resources/linkedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb724-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="eb724-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eb724-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb724-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="eb724-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb724-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
```
# <a name="c"></a>[<span data-ttu-id="eb724-134">C#</span><span class="sxs-lookup"><span data-stu-id="eb724-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb724-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb724-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb724-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb724-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="eb724-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb724-137">Response</span></span>
<span data-ttu-id="eb724-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="eb724-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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



