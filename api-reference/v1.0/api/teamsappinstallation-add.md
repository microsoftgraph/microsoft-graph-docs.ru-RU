---
title: Добавление приложения в команду
description: Установка приложения для указанной команды.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6198af51cd341898609b7b13b1a73384fef91c56
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383919"
---
# <a name="add-app-to-team"></a><span data-ttu-id="d9830-103">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="d9830-103">Add app to team</span></span>

<span data-ttu-id="d9830-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9830-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9830-105">Установка [приложения](../resources/teamsapp.md) для указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="d9830-105">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d9830-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9830-106">Permissions</span></span>

<span data-ttu-id="d9830-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9830-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9830-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9830-109">Permission type</span></span>      | <span data-ttu-id="d9830-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9830-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9830-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9830-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d9830-112">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9830-112">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="d9830-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9830-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9830-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9830-114">Not supported.</span></span>    |
|<span data-ttu-id="d9830-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9830-115">Application</span></span> | <span data-ttu-id="d9830-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9830-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9830-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9830-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="d9830-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9830-118">Request headers</span></span>

| <span data-ttu-id="d9830-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d9830-119">Header</span></span>       | <span data-ttu-id="d9830-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d9830-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d9830-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9830-121">Authorization</span></span>  | <span data-ttu-id="d9830-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9830-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d9830-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9830-124">Request body</span></span>

| <span data-ttu-id="d9830-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9830-125">Property</span></span>   | <span data-ttu-id="d9830-126">Тип</span><span class="sxs-lookup"><span data-stu-id="d9830-126">Type</span></span> |<span data-ttu-id="d9830-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d9830-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9830-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d9830-128">teamsApp</span></span>| [<span data-ttu-id="d9830-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d9830-129">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="d9830-130">Добавляемое приложение.</span><span class="sxs-lookup"><span data-stu-id="d9830-130">The app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="d9830-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9830-131">Response</span></span>

<span data-ttu-id="d9830-p103">При успешном выполнении этот метод возвращает код отклика `201 Created`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d9830-p103">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9830-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d9830-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9830-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9830-135">Request</span></span>

<span data-ttu-id="d9830-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9830-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d9830-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9830-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="c"></a>[<span data-ttu-id="d9830-138">C#</span><span class="sxs-lookup"><span data-stu-id="d9830-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9830-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9830-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9830-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9830-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9830-141">Java</span><span class="sxs-lookup"><span data-stu-id="d9830-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d9830-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9830-142">Response</span></span>

<span data-ttu-id="d9830-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d9830-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
