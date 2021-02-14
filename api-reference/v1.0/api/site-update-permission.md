---
title: Обновление разрешения
description: Обновление объекта разрешений на сайте.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 98a8b0b85577a4843664e7440978837563f44e23
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176742"
---
# <a name="update-permission"></a><span data-ttu-id="f1dd6-103">Обновление разрешения</span><span class="sxs-lookup"><span data-stu-id="f1dd6-103">Update permission</span></span>
<span data-ttu-id="f1dd6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1dd6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f1dd6-105">Обновление объекта [разрешений](../resources/permission.md) на сайте.</span><span class="sxs-lookup"><span data-stu-id="f1dd6-105">Update the [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1dd6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1dd6-106">Permissions</span></span>
<span data-ttu-id="f1dd6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1dd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1dd6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1dd6-109">Permission type</span></span>                        | <span data-ttu-id="f1dd6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1dd6-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="f1dd6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1dd6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1dd6-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1dd6-112">Not supported.</span></span>
|<span data-ttu-id="f1dd6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1dd6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1dd6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1dd6-114">Not supported.</span></span>
|<span data-ttu-id="f1dd6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1dd6-115">Application</span></span>                            | <span data-ttu-id="f1dd6-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f1dd6-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f1dd6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1dd6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /sites/{sitesId}/permissions/{permissionId}
```

## <a name="request-headers"></a><span data-ttu-id="f1dd6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1dd6-118">Request headers</span></span>
|<span data-ttu-id="f1dd6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f1dd6-119">Name</span></span>|<span data-ttu-id="f1dd6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f1dd6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f1dd6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1dd6-121">Authorization</span></span>|<span data-ttu-id="f1dd6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1dd6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f1dd6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f1dd6-124">Content-Type</span></span>|<span data-ttu-id="f1dd6-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1dd6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1dd6-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1dd6-127">Request body</span></span>
<span data-ttu-id="f1dd6-128">В теле запроса укажу представление объекта разрешений в [JSON.](../resources/permission.md)</span><span class="sxs-lookup"><span data-stu-id="f1dd6-128">In the request body, supply a JSON representation of the [permission](../resources/permission.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f1dd6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1dd6-129">Response</span></span>

<span data-ttu-id="f1dd6-130">В случае успеха этот метод возвращает код отклика и `200 OK` объект [разрешения](../resources/permission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1dd6-130">If successful, this method returns a `200 OK` response code and a [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f1dd6-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f1dd6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f1dd6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1dd6-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f1dd6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1dd6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_permission_from_"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/sites/{sitesId}/permissions/{permissionId}
Content-Type: application/json

{
  "roles": ["read"]
}
```
# <a name="c"></a>[<span data-ttu-id="f1dd6-134">C#</span><span class="sxs-lookup"><span data-stu-id="f1dd6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permission-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1dd6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1dd6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permission-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1dd6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1dd6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permission-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f1dd6-137">Java</span><span class="sxs-lookup"><span data-stu-id="f1dd6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permission-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f1dd6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1dd6-138">Response</span></span>

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
    "id": "2",
    "roles": ["read"],
    "grantedToIdentities": [{
      "application": {
        "id": "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
        "displayName": "Bar App"
      }
    }]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Update site permission",
  "suppressions": [
  ]
} -->
