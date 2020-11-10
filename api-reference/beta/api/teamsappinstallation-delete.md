---
title: Удаление приложения из группы
description: Удаляет приложение из указанной команды.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bc49bb62536ec68c7a37331d37e3d9b9bbe329d1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967292"
---
# <a name="remove-app-from-team"></a><span data-ttu-id="59ed4-103">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="59ed4-103">Remove app from team</span></span>

<span data-ttu-id="59ed4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59ed4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59ed4-105">Удаляет [приложение](../resources/teamsappinstallation.md) из указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="59ed4-105">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="59ed4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59ed4-106">Permissions</span></span>

<span data-ttu-id="59ed4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59ed4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59ed4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59ed4-109">Permission type</span></span>      | <span data-ttu-id="59ed4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59ed4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59ed4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59ed4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="59ed4-112">Теамсаппинсталлатион. Реадвритефортеам, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="59ed4-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="59ed4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59ed4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59ed4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59ed4-114">Not supported.</span></span>    |
|<span data-ttu-id="59ed4-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="59ed4-115">Application</span></span> | <span data-ttu-id="59ed4-116">Теамсаппинсталлатион. Реадвритефортеам. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="59ed4-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59ed4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59ed4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="59ed4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59ed4-118">Request headers</span></span>

| <span data-ttu-id="59ed4-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59ed4-119">Header</span></span>       | <span data-ttu-id="59ed4-120">Значение</span><span class="sxs-lookup"><span data-stu-id="59ed4-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="59ed4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59ed4-121">Authorization</span></span>  | <span data-ttu-id="59ed4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59ed4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="59ed4-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59ed4-124">Request body</span></span>

<span data-ttu-id="59ed4-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="59ed4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59ed4-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="59ed4-126">Response</span></span>

<span data-ttu-id="59ed4-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="59ed4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59ed4-129">Пример</span><span class="sxs-lookup"><span data-stu-id="59ed4-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="59ed4-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="59ed4-130">Request</span></span>

<span data-ttu-id="59ed4-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59ed4-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="59ed4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="59ed4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "uninstall_teamsapp"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
# <a name="c"></a>[<span data-ttu-id="59ed4-133">C#</span><span class="sxs-lookup"><span data-stu-id="59ed4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/uninstall-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59ed4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59ed4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/uninstall-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59ed4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59ed4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/uninstall-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59ed4-136">Java</span><span class="sxs-lookup"><span data-stu-id="59ed4-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/uninstall-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="59ed4-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="59ed4-137">Response</span></span>

<span data-ttu-id="59ed4-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="59ed4-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "uninstall_teamsapp",
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
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


