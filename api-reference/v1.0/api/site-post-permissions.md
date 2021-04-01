---
title: Создание разрешений
description: Создание нового объекта разрешений.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c950085b9271b5c3f39eb32a69e93048b55b549f
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473621"
---
# <a name="create-permission"></a><span data-ttu-id="d5a5a-103">Создание разрешений</span><span class="sxs-lookup"><span data-stu-id="d5a5a-103">Create permission</span></span>
<span data-ttu-id="d5a5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5a5a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5a5a-105">Создание нового [объекта разрешений](../resources/permission.md) на сайте.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-105">Create a new [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5a5a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5a5a-106">Permissions</span></span>
<span data-ttu-id="d5a5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5a5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5a5a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5a5a-109">Permission type</span></span>                        | <span data-ttu-id="d5a5a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5a5a-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="d5a5a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5a5a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5a5a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-112">Not supported.</span></span>
|<span data-ttu-id="d5a5a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5a5a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5a5a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-114">Not supported.</span></span>
|<span data-ttu-id="d5a5a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5a5a-115">Application</span></span>                            | <span data-ttu-id="d5a5a-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="d5a5a-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d5a5a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5a5a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /sites/{sitesId}/permissions
```

## <a name="request-headers"></a><span data-ttu-id="d5a5a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5a5a-118">Request headers</span></span>
|<span data-ttu-id="d5a5a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d5a5a-119">Name</span></span>|<span data-ttu-id="d5a5a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d5a5a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d5a5a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5a5a-121">Authorization</span></span>|<span data-ttu-id="d5a5a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d5a5a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d5a5a-124">Content-Type</span></span>|<span data-ttu-id="d5a5a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5a5a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5a5a-127">Request body</span></span>
<span data-ttu-id="d5a5a-128">В теле запроса поставляем представление JSON объекта [разрешения.](../resources/permission.md)</span><span class="sxs-lookup"><span data-stu-id="d5a5a-128">In the request body, supply a JSON representation of the [permission](../resources/permission.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d5a5a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5a5a-129">Response</span></span>

<span data-ttu-id="d5a5a-130">В случае успешной работы этот метод возвращает код ответа и `201 Created` объект разрешения в тексте ответа. [](../resources/permission.md)</span><span class="sxs-lookup"><span data-stu-id="d5a5a-130">If successful, this method returns a `201 Created` response code and a [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d5a5a-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="d5a5a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d5a5a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5a5a-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d5a5a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5a5a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_permission_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/sites/{sitesId}/permissions
Content-Type: application/json

{
  "roles": ["write"],
  "grantedToIdentities": [{
    "application": {
      "id": "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
      "displayName": "Contoso Time Manager App"
    }
  }]
}
```
# <a name="c"></a>[<span data-ttu-id="d5a5a-134">C#</span><span class="sxs-lookup"><span data-stu-id="d5a5a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-permission-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5a5a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5a5a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-permission-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5a5a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5a5a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-permission-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d5a5a-137">Java</span><span class="sxs-lookup"><span data-stu-id="d5a5a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-permission-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d5a5a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5a5a-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "id": "1",
    "roles": ["write"],
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
  "tocPath": "Sites/Permissions/Create site permissions"
} -->
