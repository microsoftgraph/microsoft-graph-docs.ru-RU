---
title: Получение Линкедресаурце
description: Чтение свойств и связей объекта Линкедресаурце.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d2c0ef4b2a10877aee0c9e956a43652bb42dc0ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999221"
---
# <a name="get-linkedresource"></a><span data-ttu-id="6c5ed-103">Получение Линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="6c5ed-103">Get linkedResource</span></span>
<span data-ttu-id="6c5ed-104">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="6c5ed-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="6c5ed-105">Чтение свойств и связей объекта [линкедресаурце](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="6c5ed-105">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c5ed-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c5ed-106">Permissions</span></span>
<span data-ttu-id="6c5ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c5ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c5ed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c5ed-109">Permission type</span></span>|<span data-ttu-id="6c5ed-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c5ed-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c5ed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c5ed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6c5ed-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c5ed-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="6c5ed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c5ed-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c5ed-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c5ed-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="6c5ed-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c5ed-115">Application</span></span>|<span data-ttu-id="6c5ed-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c5ed-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c5ed-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c5ed-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="6c5ed-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c5ed-118">Request headers</span></span>
|<span data-ttu-id="6c5ed-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6c5ed-119">Name</span></span>|<span data-ttu-id="6c5ed-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6c5ed-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6c5ed-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c5ed-121">Authorization</span></span>|<span data-ttu-id="6c5ed-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c5ed-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c5ed-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6c5ed-124">Request body</span></span>
<span data-ttu-id="6c5ed-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c5ed-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c5ed-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c5ed-126">Response</span></span>

<span data-ttu-id="6c5ed-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [линкедресаурце](../resources/linkedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c5ed-127">If successful, this method returns a `200 OK` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c5ed-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="6c5ed-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c5ed-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c5ed-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6c5ed-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c5ed-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
```
# <a name="c"></a>[<span data-ttu-id="6c5ed-131">C#</span><span class="sxs-lookup"><span data-stu-id="6c5ed-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c5ed-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c5ed-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c5ed-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c5ed-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6c5ed-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c5ed-134">Response</span></span>
<span data-ttu-id="6c5ed-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6c5ed-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.linkedResource"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
     "@odata.type": "#microsoft.graph.linkedResource",
      "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
      "webUrl": "http://microsoft.com",
      "applicationName": "Microsoft",
      "displayName": "Microsoft",
      "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
  }
}
```


