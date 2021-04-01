---
title: Получение разрешения
description: Извлечение свойств и связей объекта разрешений на сайте.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 65284bfb79121c49ed9323eef005f0276e8d0d20
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473719"
---
# <a name="get-permission"></a><span data-ttu-id="d62ad-103">Получение разрешения</span><span class="sxs-lookup"><span data-stu-id="d62ad-103">Get permission</span></span>
<span data-ttu-id="d62ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d62ad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d62ad-105">Извлечение свойств и связей объекта [разрешений](../resources/permission.md) на сайте.</span><span class="sxs-lookup"><span data-stu-id="d62ad-105">Retrieve the properties and relationships of a [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="d62ad-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d62ad-106">Permissions</span></span>
<span data-ttu-id="d62ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d62ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d62ad-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d62ad-109">Permission type</span></span>                        | <span data-ttu-id="d62ad-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d62ad-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="d62ad-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d62ad-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d62ad-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d62ad-112">Not supported.</span></span>
|<span data-ttu-id="d62ad-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d62ad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d62ad-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d62ad-114">Not supported.</span></span>
|<span data-ttu-id="d62ad-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d62ad-115">Application</span></span>                            | <span data-ttu-id="d62ad-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="d62ad-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d62ad-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d62ad-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /sites/{sitesId}/permissions/{permissionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d62ad-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d62ad-118">Optional query parameters</span></span>
<span data-ttu-id="d62ad-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d62ad-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d62ad-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d62ad-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d62ad-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d62ad-121">Request headers</span></span>
|<span data-ttu-id="d62ad-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d62ad-122">Name</span></span>|<span data-ttu-id="d62ad-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d62ad-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d62ad-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d62ad-124">Authorization</span></span>|<span data-ttu-id="d62ad-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d62ad-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d62ad-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d62ad-127">Request body</span></span>
<span data-ttu-id="d62ad-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d62ad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d62ad-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d62ad-129">Response</span></span>

<span data-ttu-id="d62ad-130">В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [разрешения](../resources/permission.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d62ad-130">If successful, this method returns a `200 OK` response code and the [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d62ad-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="d62ad-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d62ad-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d62ad-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d62ad-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d62ad-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_permission"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/sites/{sitesId}/permissions/{permissionId}
```
# <a name="c"></a>[<span data-ttu-id="d62ad-134">C#</span><span class="sxs-lookup"><span data-stu-id="d62ad-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d62ad-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d62ad-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d62ad-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d62ad-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d62ad-137">Java</span><span class="sxs-lookup"><span data-stu-id="d62ad-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d62ad-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d62ad-138">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "1",
  "roles": ["read"],
  "grantedToIdentities": [{
    "application": {
      "id": "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
      "displayName": "Contoso Time Manager App"
    }
  }]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Get site permission",
} -->
