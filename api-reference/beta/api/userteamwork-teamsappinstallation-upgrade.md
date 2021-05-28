---
title: 'teamsAppInstallation: обновление'
description: Обновление установки приложения в личной области пользователя
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1dd9a390203658a2f7f284023a05ed0e166e5839
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696277"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="b2b46-103">teamsAppInstallation: обновление</span><span class="sxs-lookup"><span data-stu-id="b2b46-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="b2b46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2b46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2b46-105">Обновление [установки приложения](../resources/teamsappinstallation.md) в личном поле [](../resources/user.md) указанного пользователя до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="b2b46-105">Upgrade an [app installation](../resources/teamsappinstallation.md) in the personal scope of the specified [user](../resources/user.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2b46-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2b46-106">Permissions</span></span>

<span data-ttu-id="b2b46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2b46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2b46-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2b46-109">Permission type</span></span>      | <span data-ttu-id="b2b46-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2b46-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2b46-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2b46-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b2b46-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="b2b46-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="b2b46-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2b46-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2b46-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2b46-114">Not supported.</span></span>    |
|<span data-ttu-id="b2b46-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b2b46-115">Application</span></span> | <span data-ttu-id="b2b46-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span><span class="sxs-lookup"><span data-stu-id="b2b46-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2b46-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2b46-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{user-id | user-principal-name}/teamwork/installedApps/{app-installation-id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="b2b46-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2b46-118">Request headers</span></span>

| <span data-ttu-id="b2b46-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2b46-119">Header</span></span>       | <span data-ttu-id="b2b46-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b2b46-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b2b46-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2b46-121">Authorization</span></span>  | <span data-ttu-id="b2b46-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2b46-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b2b46-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2b46-124">Request body</span></span>

<span data-ttu-id="b2b46-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2b46-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2b46-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2b46-126">Response</span></span>

<span data-ttu-id="b2b46-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b2b46-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2b46-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b2b46-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2b46-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2b46-130">Request</span></span>

<span data-ttu-id="b2b46-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2b46-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b2b46-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2b46-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_upgrade_teamsApp"
}-->
```http
POST /users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk/upgrade
```
# <a name="c"></a>[<span data-ttu-id="b2b46-133">C#</span><span class="sxs-lookup"><span data-stu-id="b2b46-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2b46-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2b46-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2b46-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2b46-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2b46-136">Java</span><span class="sxs-lookup"><span data-stu-id="b2b46-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-upgrade-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b2b46-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2b46-137">Response</span></span>

<span data-ttu-id="b2b46-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b2b46-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "user_upgrade_teamsApp",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Upgrade teamsApp for user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


