---
title: Удаление приложения для пользователя
description: Удаление приложения из личной области указанного пользователя.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 175ab50057986a84dbfa4e962face3c05147a2c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968887"
---
# <a name="uninstall-app-for-user"></a><span data-ttu-id="0b4c6-103">Удаление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="0b4c6-103">Uninstall app for user</span></span>

<span data-ttu-id="0b4c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b4c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b4c6-105">Удаление [приложения](../resources/teamsappinstallation.md) из личной области указанного [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="0b4c6-105">Uninstall an [app](../resources/teamsappinstallation.md) from the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b4c6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b4c6-106">Permissions</span></span>

<span data-ttu-id="0b4c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b4c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b4c6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b4c6-109">Permission type</span></span>      | <span data-ttu-id="0b4c6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b4c6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b4c6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b4c6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0b4c6-112">TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="0b4c6-112">TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="0b4c6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b4c6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b4c6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b4c6-114">Not supported.</span></span>    |
|<span data-ttu-id="0b4c6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b4c6-115">Application</span></span> | <span data-ttu-id="0b4c6-116">TeamsAppInstallation.ReadWriteForUser.All</span><span class="sxs-lookup"><span data-stu-id="0b4c6-116">TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b4c6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b4c6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/teamwork/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0b4c6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b4c6-118">Request headers</span></span>

| <span data-ttu-id="0b4c6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b4c6-119">Header</span></span>       | <span data-ttu-id="0b4c6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0b4c6-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0b4c6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b4c6-121">Authorization</span></span>  | <span data-ttu-id="0b4c6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b4c6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0b4c6-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0b4c6-124">Request body</span></span>

<span data-ttu-id="0b4c6-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b4c6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b4c6-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b4c6-126">Response</span></span>

<span data-ttu-id="0b4c6-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0b4c6-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b4c6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0b4c6-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b4c6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b4c6-130">Request</span></span>

<span data-ttu-id="0b4c6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b4c6-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0b4c6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b4c6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delete_teamsApp"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps/{id}
```
# <a name="c"></a>[<span data-ttu-id="0b4c6-133">C#</span><span class="sxs-lookup"><span data-stu-id="0b4c6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b4c6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b4c6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b4c6-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b4c6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0b4c6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b4c6-136">Response</span></span>

<span data-ttu-id="0b4c6-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0b4c6-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User delete teamsAppInstallations,
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


