---
title: Добавление приложения в команду
description: Устанавливает приложение в указанную группу.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ca4110cb180860448fc7a6cf75d33d832e36a4a1
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409347"
---
# <a name="add-app-to-team"></a><span data-ttu-id="4a936-103">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="4a936-103">Add app to team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a936-104">Устанавливает [приложение](../resources/teamsapp.md) в указанную [группу](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="4a936-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a936-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a936-105">Permissions</span></span>

<span data-ttu-id="4a936-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a936-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a936-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a936-108">Permission type</span></span>      | <span data-ttu-id="4a936-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a936-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a936-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a936-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4a936-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a936-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4a936-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a936-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a936-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a936-113">Not supported.</span></span>    |
|<span data-ttu-id="4a936-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a936-114">Application</span></span> | <span data-ttu-id="4a936-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a936-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a936-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a936-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="4a936-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a936-117">Request headers</span></span>

| <span data-ttu-id="4a936-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a936-118">Header</span></span>       | <span data-ttu-id="4a936-119">Значение</span><span class="sxs-lookup"><span data-stu-id="4a936-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4a936-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a936-120">Authorization</span></span>  | <span data-ttu-id="4a936-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a936-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4a936-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4a936-123">Request body</span></span>

| <span data-ttu-id="4a936-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a936-124">Property</span></span>   | <span data-ttu-id="4a936-125">Тип</span><span class="sxs-lookup"><span data-stu-id="4a936-125">Type</span></span> |<span data-ttu-id="4a936-126">Описание</span><span class="sxs-lookup"><span data-stu-id="4a936-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a936-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="4a936-127">teamsApp</span></span>|<span data-ttu-id="4a936-128">String</span><span class="sxs-lookup"><span data-stu-id="4a936-128">String</span></span>|<span data-ttu-id="4a936-129">Идентификатор добавляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="4a936-129">The id of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="4a936-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a936-130">Response</span></span>

<span data-ttu-id="4a936-p103">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4a936-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a936-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4a936-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a936-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a936-134">Request</span></span>

<span data-ttu-id="4a936-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a936-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4a936-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a936-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4a936-137">C#</span><span class="sxs-lookup"><span data-stu-id="4a936-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a936-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a936-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4a936-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4a936-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4a936-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a936-140">Response</span></span>

<span data-ttu-id="4a936-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4a936-141">The following is an example of the response.</span></span>

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
