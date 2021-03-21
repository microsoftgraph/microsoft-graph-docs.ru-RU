---
title: Список linkedResources
description: Получите linkedResources из свойства навигации linkedResources.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ab6f7984a7202ebe12cab0be465deb8e6797dee0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963452"
---
# <a name="list-linkedresources"></a><span data-ttu-id="ec2a4-103">Список linkedResources</span><span class="sxs-lookup"><span data-stu-id="ec2a4-103">List linkedResources</span></span>
<span data-ttu-id="ec2a4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec2a4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ec2a4-105">Получение сведений об одном или более элементов в партнерской заявке, на основе которой была создана [указанная](../resources/todotask.md) задача.</span><span class="sxs-lookup"><span data-stu-id="ec2a4-105">Get information of one or more items in a partner application, based on which a specified [task](../resources/todotask.md) was created.</span></span> <span data-ttu-id="ec2a4-106">Сведения представлены в [объекте linkedResource](../resources/linkedresource.md) для каждого элемента.</span><span class="sxs-lookup"><span data-stu-id="ec2a4-106">The information is represented in a [linkedResource](../resources/linkedresource.md) object for each item.</span></span> <span data-ttu-id="ec2a4-107">Он включает внешний ID для элемента в партнерской заявке и, если применимо, глубокую ссылку на этот элемент в приложении.</span><span class="sxs-lookup"><span data-stu-id="ec2a4-107">It includes an external ID for the item in the partner application, and if applicable, a deep link to that item in the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec2a4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec2a4-108">Permissions</span></span>
<span data-ttu-id="ec2a4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec2a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec2a4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec2a4-111">Permission type</span></span>|<span data-ttu-id="ec2a4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec2a4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec2a4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec2a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec2a4-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec2a4-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="ec2a4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec2a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec2a4-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec2a4-116">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="ec2a4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec2a4-117">Application</span></span>|<span data-ttu-id="ec2a4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec2a4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec2a4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec2a4-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec2a4-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ec2a4-120">Optional query parameters</span></span>
<span data-ttu-id="ec2a4-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ec2a4-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ec2a4-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ec2a4-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec2a4-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec2a4-123">Request headers</span></span>
|<span data-ttu-id="ec2a4-124">Имя</span><span class="sxs-lookup"><span data-stu-id="ec2a4-124">Name</span></span>|<span data-ttu-id="ec2a4-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ec2a4-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ec2a4-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec2a4-126">Authorization</span></span>|<span data-ttu-id="ec2a4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec2a4-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec2a4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec2a4-129">Request body</span></span>
<span data-ttu-id="ec2a4-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec2a4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec2a4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec2a4-131">Response</span></span>

<span data-ttu-id="ec2a4-132">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [linkedResource](../resources/linkedresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ec2a4-132">If successful, this method returns a `200 OK` response code and a collection of [linkedResource](../resources/linkedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ec2a4-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="ec2a4-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ec2a4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec2a4-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ec2a4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec2a4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "get_linkedresource_2"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
```
# <a name="c"></a>[<span data-ttu-id="ec2a4-136">C#</span><span class="sxs-lookup"><span data-stu-id="ec2a4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec2a4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec2a4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec2a4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec2a4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec2a4-139">Java</span><span class="sxs-lookup"><span data-stu-id="ec2a4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-linkedresource-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ec2a4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec2a4-140">Response</span></span>
<span data-ttu-id="ec2a4-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ec2a4-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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



