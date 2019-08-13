---
title: Добавление приложения в команду
description: Устанавливает приложение в указанную группу.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c20b53c3647edf4d6c3b03db94d20fc49193d951
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362852"
---
# <a name="add-app-to-team"></a><span data-ttu-id="0f455-103">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="0f455-103">Add app to team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f455-104">Устанавливает [приложение](../resources/teamsapp.md) в указанную [группу](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="0f455-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0f455-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f455-105">Permissions</span></span>

<span data-ttu-id="0f455-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f455-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f455-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f455-108">Permission type</span></span>      | <span data-ttu-id="0f455-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f455-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f455-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f455-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0f455-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f455-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0f455-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f455-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f455-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f455-113">Not supported.</span></span>    |
|<span data-ttu-id="0f455-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f455-114">Application</span></span> | <span data-ttu-id="0f455-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f455-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f455-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f455-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="0f455-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f455-117">Request headers</span></span>

| <span data-ttu-id="0f455-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0f455-118">Header</span></span>       | <span data-ttu-id="0f455-119">Значение</span><span class="sxs-lookup"><span data-stu-id="0f455-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0f455-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f455-120">Authorization</span></span>  | <span data-ttu-id="0f455-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f455-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0f455-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0f455-123">Request body</span></span>

| <span data-ttu-id="0f455-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f455-124">Property</span></span>   | <span data-ttu-id="0f455-125">Тип</span><span class="sxs-lookup"><span data-stu-id="0f455-125">Type</span></span> |<span data-ttu-id="0f455-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0f455-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f455-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0f455-127">teamsApp</span></span>|<span data-ttu-id="0f455-128">String</span><span class="sxs-lookup"><span data-stu-id="0f455-128">String</span></span>|<span data-ttu-id="0f455-129">Идентификатор добавляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="0f455-129">The id of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="0f455-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f455-130">Response</span></span>

<span data-ttu-id="0f455-p103">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0f455-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f455-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0f455-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f455-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f455-134">Request</span></span>

<span data-ttu-id="0f455-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f455-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0f455-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f455-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_teamsApp"
}-->
```http
POST /teams/87654321-0abc-zqf0-321456789q/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0f455-137">C#</span><span class="sxs-lookup"><span data-stu-id="0f455-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0f455-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f455-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0f455-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0f455-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0f455-140">Java</span><span class="sxs-lookup"><span data-stu-id="0f455-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0f455-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f455-141">Response</span></span>

<span data-ttu-id="0f455-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0f455-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add teamsApp",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
