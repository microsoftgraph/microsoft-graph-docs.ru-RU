---
title: 'команда: completeMigration'
description: Выполните миграцию внешних сообщений, удалив режим миграции из группы.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0d7599bb68479dba9aa03b4e6a56bac1cee50fc5
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51207586"
---
# <a name="team-completemigration"></a><span data-ttu-id="44bf2-103">команда: completeMigration</span><span class="sxs-lookup"><span data-stu-id="44bf2-103">team: completeMigration</span></span>

<span data-ttu-id="44bf2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44bf2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="44bf2-105">Завершите процесс миграции сообщений, `migration mode` удалив его из [группы.](../resources/team.md)</span><span class="sxs-lookup"><span data-stu-id="44bf2-105">Complete the message migration process by removing `migration mode` from a [team](../resources/team.md).</span></span> <span data-ttu-id="44bf2-106">`Migration mode` это специальное состояние, в котором определенные операции запрещены, например post сообщения и операции членства во время процесса миграции данных.</span><span class="sxs-lookup"><span data-stu-id="44bf2-106">`Migration mode` is a special state where certain operations are barred, like message POST and membership operations during the data migration process.</span></span>

<span data-ttu-id="44bf2-107">После выполнения **запроса completeMigration** вы не можете импортировать дополнительные сообщения в команду.</span><span class="sxs-lookup"><span data-stu-id="44bf2-107">After a **completeMigration** request is made, you cannot import additional messages into the team.</span></span> <span data-ttu-id="44bf2-108">Вы можете добавить членов в команду после успешного ответа на запрос.</span><span class="sxs-lookup"><span data-stu-id="44bf2-108">You can add members to the team after the request returns a successful response.</span></span>

## <a name="permissions"></a><span data-ttu-id="44bf2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44bf2-109">Permissions</span></span>

<span data-ttu-id="44bf2-110">Для вызова этого API требуется следующее разрешение.</span><span class="sxs-lookup"><span data-stu-id="44bf2-110">The following permission is required to call this API.</span></span> <span data-ttu-id="44bf2-111">Дополнительные сведения см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44bf2-111">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44bf2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44bf2-112">Permission type</span></span>      | <span data-ttu-id="44bf2-113">Разрешение</span><span class="sxs-lookup"><span data-stu-id="44bf2-113">Permission</span></span>  |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="44bf2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44bf2-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="44bf2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44bf2-115">Not supported.</span></span>|
| <span data-ttu-id="44bf2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44bf2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44bf2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44bf2-117">Not supported.</span></span> |
|<span data-ttu-id="44bf2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44bf2-118">Application</span></span> | <span data-ttu-id="44bf2-119">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="44bf2-119">Teamwork.Migrate.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44bf2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44bf2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/completeMigration
```

## <a name="request-headers"></a><span data-ttu-id="44bf2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44bf2-121">Request headers</span></span>

| <span data-ttu-id="44bf2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44bf2-122">Header</span></span>       | <span data-ttu-id="44bf2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="44bf2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="44bf2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44bf2-124">Authorization</span></span>  | <span data-ttu-id="44bf2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44bf2-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="44bf2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44bf2-127">Request body</span></span>

<span data-ttu-id="44bf2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44bf2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44bf2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="44bf2-129">Response</span></span>

<span data-ttu-id="44bf2-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="44bf2-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44bf2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="44bf2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="44bf2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="44bf2-133">Request</span></span>

<span data-ttu-id="44bf2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44bf2-134">The following is an example of the request.</span></span>
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD022 -->


<!-- {
  "blockType": "request",
  "name": "completeMigration_team"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/completeMigration
```


<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="44bf2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="44bf2-135">Response</span></span>

<span data-ttu-id="44bf2-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="44bf2-136">The following is an example of the response.</span></span>
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
