---
title: Разрешения списка
description: Получите ресурсы разрешений из свойства навигации разрешений на сайте.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 33085513c2a6279a9c765fe43fa9eb8a025d1057
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473703"
---
# <a name="list-permissions"></a><span data-ttu-id="585a6-103">Разрешения списка</span><span class="sxs-lookup"><span data-stu-id="585a6-103">List permissions</span></span>
<span data-ttu-id="585a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="585a6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="585a6-105">Получите ресурсы [разрешений](../resources/permission.md) из свойства навигации разрешений на сайте.</span><span class="sxs-lookup"><span data-stu-id="585a6-105">Get the [permission](../resources/permission.md) resources from the permissions navigation property on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="585a6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="585a6-106">Permissions</span></span>
<span data-ttu-id="585a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="585a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="585a6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="585a6-109">Permission type</span></span>                        | <span data-ttu-id="585a6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="585a6-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="585a6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="585a6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="585a6-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="585a6-112">Not supported.</span></span>
|<span data-ttu-id="585a6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="585a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="585a6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="585a6-114">Not supported.</span></span>
|<span data-ttu-id="585a6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="585a6-115">Application</span></span>                            | <span data-ttu-id="585a6-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="585a6-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="585a6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="585a6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /sites/{sitesId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="585a6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="585a6-118">Optional query parameters</span></span>
<span data-ttu-id="585a6-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="585a6-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="585a6-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="585a6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="585a6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="585a6-121">Request headers</span></span>
|<span data-ttu-id="585a6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="585a6-122">Name</span></span>|<span data-ttu-id="585a6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="585a6-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="585a6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="585a6-124">Authorization</span></span>|<span data-ttu-id="585a6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="585a6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="585a6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="585a6-127">Request body</span></span>
<span data-ttu-id="585a6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="585a6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="585a6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="585a6-129">Response</span></span>

<span data-ttu-id="585a6-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` разрешений в [](../resources/permission.md) тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="585a6-130">If successful, this method returns a `200 OK` response code and a collection of [permission](../resources/permission.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="585a6-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="585a6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="585a6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="585a6-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="585a6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="585a6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_permission"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/sites/{sitesId}/permissions
```
# <a name="c"></a>[<span data-ttu-id="585a6-134">C#</span><span class="sxs-lookup"><span data-stu-id="585a6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="585a6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="585a6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="585a6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="585a6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="585a6-137">Java</span><span class="sxs-lookup"><span data-stu-id="585a6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="585a6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="585a6-138">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.permission)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["read"],
      "grantedToIdentities": [{
        "application": {
          "id": "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
          "displayName": "Contoso Time Manager App"
        }
      }]
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedToIdentities": [{
        "application": {
          "id": "22f09bb7-dd29-403e-bec2-ab5cde52c2b3",
          "displayName": "Fabrikam Dashboard App"
        }
      }]
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/List site permission",
} -->
