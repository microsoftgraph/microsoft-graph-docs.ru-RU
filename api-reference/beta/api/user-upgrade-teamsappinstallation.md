---
title: 'Теамсаппинсталлатион: обновление'
description: Обновление установки приложения в личной области пользователя
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e0de5b95f8da705b6209cdaa5350f71d629a48f7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362056"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="e55b9-103">Теамсаппинсталлатион: обновление</span><span class="sxs-lookup"><span data-stu-id="e55b9-103">teamsAppInstallation: upgrade</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e55b9-104">Обновление [установки приложения](../resources/teamsappinstallation.md) в личной области указанного [пользователя](../resources/user.md) до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="e55b9-104">Upgrade an [app installation](../resources/teamsappinstallation.md) in the personal scope of the specified [user](../resources/user.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="e55b9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e55b9-105">Permissions</span></span>

<span data-ttu-id="e55b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e55b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e55b9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e55b9-108">Permission type</span></span>      | <span data-ttu-id="e55b9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e55b9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e55b9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e55b9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e55b9-111">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e55b9-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="e55b9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e55b9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e55b9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e55b9-113">Not supported.</span></span>    |
|<span data-ttu-id="e55b9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e55b9-114">Application</span></span> | <span data-ttu-id="e55b9-115">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e55b9-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e55b9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e55b9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="e55b9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e55b9-117">Request headers</span></span>

| <span data-ttu-id="e55b9-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e55b9-118">Header</span></span>       | <span data-ttu-id="e55b9-119">Значение</span><span class="sxs-lookup"><span data-stu-id="e55b9-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e55b9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e55b9-120">Authorization</span></span>  | <span data-ttu-id="e55b9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e55b9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e55b9-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e55b9-123">Request body</span></span>

<span data-ttu-id="e55b9-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e55b9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e55b9-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="e55b9-125">Response</span></span>

<span data-ttu-id="e55b9-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e55b9-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e55b9-128">Пример</span><span class="sxs-lookup"><span data-stu-id="e55b9-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="e55b9-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e55b9-129">Request</span></span>

<span data-ttu-id="e55b9-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e55b9-130">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e55b9-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e55b9-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_upgrade_teamsApp"
}-->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e55b9-132">C#</span><span class="sxs-lookup"><span data-stu-id="e55b9-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e55b9-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e55b9-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e55b9-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e55b9-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e55b9-135">Java</span><span class="sxs-lookup"><span data-stu-id="e55b9-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-upgrade-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e55b9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e55b9-136">Response</span></span>

<span data-ttu-id="e55b9-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e55b9-137">The following is an example of the response.</span></span>

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
