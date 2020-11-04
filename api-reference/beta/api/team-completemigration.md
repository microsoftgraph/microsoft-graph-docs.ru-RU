---
title: 'команда: Комплетемигратион'
description: Завершите Перенос внешних сообщений, удалив из команды режим миграции.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0594d7da3dce01285829e9ad4e59e8143c41bfdf
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903606"
---
# <a name="team-completemigration"></a><span data-ttu-id="b5458-103">команда: Комплетемигратион</span><span class="sxs-lookup"><span data-stu-id="b5458-103">team: completeMigration</span></span>

<span data-ttu-id="b5458-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5458-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5458-105">Завершите процесс переноса сообщений, удалив `migration mode` из [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="b5458-105">Complete the message migration process by removing `migration mode` from a [team](../resources/team.md).</span></span> <span data-ttu-id="b5458-106">`Migration mode` — Это специальное состояние, в котором отменяются определенные операции, например операции отправки и участия в сообщениях во время процесса переноса данных.</span><span class="sxs-lookup"><span data-stu-id="b5458-106">`Migration mode` is a special state where certain operations are barred, like message POST and membership operations during the data migration process.</span></span>

<span data-ttu-id="b5458-107">После выполнения запроса **комплетемигратион** вы не можете импортировать в команду Дополнительные сообщения.</span><span class="sxs-lookup"><span data-stu-id="b5458-107">After a **completeMigration** request is made, you cannot import additional messages into the team.</span></span> <span data-ttu-id="b5458-108">Вы можете добавлять участников в команду после того, как запрос возвращает успешный ответ.</span><span class="sxs-lookup"><span data-stu-id="b5458-108">You can add members to the team after the request returns a successful response.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5458-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5458-109">Permissions</span></span>

<span data-ttu-id="b5458-110">Для вызова этого API требуется следующее разрешение.</span><span class="sxs-lookup"><span data-stu-id="b5458-110">The following permission is required to call this API.</span></span> <span data-ttu-id="b5458-111">Дополнительные сведения см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5458-111">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5458-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5458-112">Permission type</span></span>      | <span data-ttu-id="b5458-113">Разрешение</span><span class="sxs-lookup"><span data-stu-id="b5458-113">Permission</span></span>  |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="b5458-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5458-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="b5458-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5458-115">Not supported.</span></span>|
| <span data-ttu-id="b5458-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5458-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5458-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5458-117">Not supported.</span></span> |
|<span data-ttu-id="b5458-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5458-118">Application</span></span> | <span data-ttu-id="b5458-119">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="b5458-119">Teamwork.Migrate.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5458-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5458-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{teamId}/completeMigration
```

## <a name="request-headers"></a><span data-ttu-id="b5458-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5458-121">Request headers</span></span>

| <span data-ttu-id="b5458-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b5458-122">Header</span></span>       | <span data-ttu-id="b5458-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b5458-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b5458-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5458-124">Authorization</span></span>  | <span data-ttu-id="b5458-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5458-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b5458-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5458-127">Request body</span></span>

<span data-ttu-id="b5458-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5458-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5458-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5458-129">Response</span></span>

<span data-ttu-id="b5458-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b5458-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5458-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b5458-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5458-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5458-133">Request</span></span>

<span data-ttu-id="b5458-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5458-134">The following is an example of the request.</span></span>
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD022 -->


# <a name="http"></a>[<span data-ttu-id="b5458-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5458-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "completeMigration_team"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/completeMigration
```
# <a name="c"></a>[<span data-ttu-id="b5458-136">C#</span><span class="sxs-lookup"><span data-stu-id="b5458-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/completemigration-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5458-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5458-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/completemigration-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5458-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5458-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/completemigration-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="b5458-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5458-139">Response</span></span>

<span data-ttu-id="b5458-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b5458-140">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: d945a9a4-0e5b-11eb-adc1-0242ac120002
2020-10-14 20:22:11 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "completeMigration_ team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
