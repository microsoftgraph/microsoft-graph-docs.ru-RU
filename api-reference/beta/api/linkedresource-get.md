---
title: Получение Линкедресаурце
description: Чтение свойств и связей объекта Линкедресаурце.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e041281a1922fce22f9e9b5ab8d38d1d0e572359
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873066"
---
# <a name="get-linkedresource"></a><span data-ttu-id="f6ed0-103">Получение Линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="f6ed0-103">Get linkedResource</span></span>
<span data-ttu-id="f6ed0-104">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="f6ed0-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="f6ed0-105">Чтение свойств и связей объекта [линкедресаурце](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="f6ed0-105">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6ed0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6ed0-106">Permissions</span></span>
<span data-ttu-id="f6ed0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6ed0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6ed0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6ed0-109">Permission type</span></span>|<span data-ttu-id="f6ed0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6ed0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6ed0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6ed0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f6ed0-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6ed0-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f6ed0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6ed0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6ed0-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6ed0-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f6ed0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6ed0-115">Application</span></span>|<span data-ttu-id="f6ed0-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f6ed0-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6ed0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6ed0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="f6ed0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6ed0-118">Request headers</span></span>
|<span data-ttu-id="f6ed0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f6ed0-119">Name</span></span>|<span data-ttu-id="f6ed0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f6ed0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f6ed0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6ed0-121">Authorization</span></span>|<span data-ttu-id="f6ed0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6ed0-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6ed0-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6ed0-124">Request body</span></span>
<span data-ttu-id="f6ed0-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6ed0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6ed0-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6ed0-126">Response</span></span>

<span data-ttu-id="f6ed0-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [линкедресаурце](../resources/linkedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6ed0-127">If successful, this method returns a `200 OK` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f6ed0-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="f6ed0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f6ed0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6ed0-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f6ed0-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6ed0-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
```
# <a name="c"></a>[<span data-ttu-id="f6ed0-131">C#</span><span class="sxs-lookup"><span data-stu-id="f6ed0-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6ed0-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6ed0-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6ed0-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6ed0-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f6ed0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6ed0-134">Response</span></span>
<span data-ttu-id="f6ed0-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f6ed0-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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
