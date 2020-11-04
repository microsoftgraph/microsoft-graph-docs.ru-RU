---
title: Список Линкедресаурцес
description: Получение Линкедресаурцес из свойства навигации Линкедресаурцес.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: aa016742bad1535332ee9e5d78585467fc7a6af0
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904359"
---
# <a name="list-linkedresources"></a><span data-ttu-id="f4276-103">Список Линкедресаурцес</span><span class="sxs-lookup"><span data-stu-id="f4276-103">List linkedResources</span></span>
<span data-ttu-id="f4276-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4276-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f4276-105">Получение сведений об одном или нескольких элементах партнерского приложения, на основе которого была создана указанная [задача](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="f4276-105">Get information of one or more items in a partner application, based on which a specified [task](../resources/todotask.md) was created.</span></span> <span data-ttu-id="f4276-106">Сведения представлены в объекте [линкедресаурце](../resources/linkedresource.md) для каждого элемента.</span><span class="sxs-lookup"><span data-stu-id="f4276-106">The information is represented in a [linkedResource](../resources/linkedresource.md) object for each item.</span></span> <span data-ttu-id="f4276-107">Он включает внешний идентификатор элемента в партнерской приложении и, если это возможно, глубокая ссылка на этот элемент в приложении.</span><span class="sxs-lookup"><span data-stu-id="f4276-107">It includes an external ID for the item in the partner application, and if applicable, a deep link to that item in the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4276-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4276-108">Permissions</span></span>
<span data-ttu-id="f4276-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4276-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4276-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4276-111">Permission type</span></span>|<span data-ttu-id="f4276-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4276-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4276-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4276-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4276-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4276-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f4276-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4276-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4276-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4276-116">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f4276-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4276-117">Application</span></span>|<span data-ttu-id="f4276-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4276-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4276-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4276-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4276-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f4276-120">Optional query parameters</span></span>
<span data-ttu-id="f4276-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f4276-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f4276-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f4276-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4276-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4276-123">Request headers</span></span>
|<span data-ttu-id="f4276-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f4276-124">Name</span></span>|<span data-ttu-id="f4276-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f4276-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f4276-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4276-126">Authorization</span></span>|<span data-ttu-id="f4276-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4276-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4276-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4276-129">Request body</span></span>
<span data-ttu-id="f4276-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4276-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4276-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4276-131">Response</span></span>

<span data-ttu-id="f4276-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [линкедресаурце](../resources/linkedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4276-132">If successful, this method returns a `200 OK` response code and a collection of [linkedResource](../resources/linkedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f4276-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="f4276-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f4276-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4276-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f4276-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4276-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
```
# <a name="c"></a>[<span data-ttu-id="f4276-136">C#</span><span class="sxs-lookup"><span data-stu-id="f4276-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4276-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4276-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4276-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4276-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4276-139">Java</span><span class="sxs-lookup"><span data-stu-id="f4276-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-linkedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f4276-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4276-140">Response</span></span>
<span data-ttu-id="f4276-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f4276-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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



