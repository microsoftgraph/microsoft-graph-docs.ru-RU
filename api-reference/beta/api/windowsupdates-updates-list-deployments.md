---
title: Развертывание списков
description: Получите список объектов развертывания и их свойств.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 4eda89bc8f9bbdd2ec65f6701347f79989cdebff
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239192"
---
# <a name="list-deployments"></a><span data-ttu-id="5f715-103">Развертывание списков</span><span class="sxs-lookup"><span data-stu-id="5f715-103">List deployments</span></span>
<span data-ttu-id="5f715-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="5f715-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f715-105">Получите список объектов [развертывания](../resources/windowsupdates-deployment.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="5f715-105">Get a list of [deployment](../resources/windowsupdates-deployment.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f715-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f715-106">Permissions</span></span>
<span data-ttu-id="5f715-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f715-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f715-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f715-109">Permission type</span></span>|<span data-ttu-id="5f715-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f715-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f715-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f715-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5f715-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f715-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="5f715-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f715-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f715-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f715-114">Not supported.</span></span>|
|<span data-ttu-id="5f715-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f715-115">Application</span></span>|<span data-ttu-id="5f715-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f715-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f715-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f715-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/deployments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f715-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5f715-118">Optional query parameters</span></span>
<span data-ttu-id="5f715-119">Этот метод поддерживает некоторые параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$count` , , , , , и `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="5f715-119">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f715-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f715-120">Request headers</span></span>
|<span data-ttu-id="5f715-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5f715-121">Name</span></span>|<span data-ttu-id="5f715-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5f715-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5f715-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f715-123">Authorization</span></span>|<span data-ttu-id="5f715-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f715-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f715-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f715-126">Request body</span></span>
<span data-ttu-id="5f715-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f715-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f715-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f715-128">Response</span></span>

<span data-ttu-id="5f715-129">В случае успешного применения этот метод возвращает код ответа и коллекцию объектов `200 OK` развертывания в тексте отклика. [](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="5f715-129">If successful, this method returns a `200 OK` response code and a collection of [deployment](../resources/windowsupdates-deployment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f715-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="5f715-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5f715-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f715-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5f715-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f715-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_deployment"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments
```
# <a name="c"></a>[<span data-ttu-id="5f715-133">C#</span><span class="sxs-lookup"><span data-stu-id="5f715-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-deployment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f715-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f715-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-deployment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f715-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f715-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-deployment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f715-136">Java</span><span class="sxs-lookup"><span data-stu-id="5f715-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-deployment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5f715-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f715-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.deployment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
      "id": "b5171742-1742-b517-4217-17b5421717b5",
      "state": {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
      },
      "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.deployableContent"
      },
      "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentSettings"
      },
      "createdDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)"
    }
  ]
}
```

