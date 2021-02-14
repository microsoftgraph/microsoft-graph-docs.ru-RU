---
title: Разрешения на удаление
description: Удаление объекта разрешений на сайте.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 09cfc0831230b3861f842728006b041a4f8e0261
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176928"
---
# <a name="delete-permission"></a><span data-ttu-id="8454d-103">Разрешения на удаление</span><span class="sxs-lookup"><span data-stu-id="8454d-103">Delete permission</span></span>
<span data-ttu-id="8454d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8454d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8454d-105">Удаление объекта [разрешений](../resources/permission.md) на сайте.</span><span class="sxs-lookup"><span data-stu-id="8454d-105">Delete a [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="8454d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8454d-106">Permissions</span></span>
<span data-ttu-id="8454d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8454d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8454d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8454d-109">Permission type</span></span>                        | <span data-ttu-id="8454d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8454d-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="8454d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8454d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8454d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8454d-112">Not supported.</span></span>
|<span data-ttu-id="8454d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8454d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8454d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8454d-114">Not supported.</span></span>
|<span data-ttu-id="8454d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8454d-115">Application</span></span>                            | <span data-ttu-id="8454d-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="8454d-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="8454d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8454d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /sites/{sitesId}/permissions/{permissionId}
```

## <a name="request-headers"></a><span data-ttu-id="8454d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8454d-118">Request headers</span></span>
|<span data-ttu-id="8454d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8454d-119">Name</span></span>|<span data-ttu-id="8454d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8454d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8454d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8454d-121">Authorization</span></span>|<span data-ttu-id="8454d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8454d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8454d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8454d-124">Request body</span></span>
<span data-ttu-id="8454d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8454d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8454d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8454d-126">Response</span></span>

<span data-ttu-id="8454d-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8454d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8454d-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="8454d-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8454d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8454d-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8454d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8454d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_permission"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/sites/{sitesId}/permissions/{permissionId}
```
# <a name="c"></a>[<span data-ttu-id="8454d-132">C#</span><span class="sxs-lookup"><span data-stu-id="8454d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8454d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8454d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8454d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8454d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8454d-135">Java</span><span class="sxs-lookup"><span data-stu-id="8454d-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8454d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8454d-136">Response</span></span>
<span data-ttu-id="8454d-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8454d-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Delete site permission"
} -->
