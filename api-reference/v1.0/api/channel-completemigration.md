---
title: 'канал: completeMigration'
description: Завершите миграцию внешних сообщений, удалив режим миграции из канала.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 150bb921c87bcd0ea62d7218315f79e791a170fe
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51207580"
---
# <a name="channel-completemigration"></a><span data-ttu-id="3a3a5-103">канал: completeMigration</span><span class="sxs-lookup"><span data-stu-id="3a3a5-103">channel: completeMigration</span></span>

<span data-ttu-id="3a3a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a3a5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3a3a5-105">Завершите процесс миграции сообщений, `migration mode` удалив [канал](../resources/channel.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="3a3a5-105">Complete the message migration process by removing `migration mode` from a [channel](../resources/channel.md) in a team.</span></span> <span data-ttu-id="3a3a5-106">`Migration mode` это специальное состояние, которое предотвращает определенные операции, например отправку сообщений и добавление участников, во время процесса миграции данных.</span><span class="sxs-lookup"><span data-stu-id="3a3a5-106">`Migration mode` is a special state that prevents certain operations, like sending messages and adding members, during the data migration process.</span></span>

<span data-ttu-id="3a3a5-107">После выполнения **запроса completeMigration** вы не можете импортировать дополнительные сообщения в команду.</span><span class="sxs-lookup"><span data-stu-id="3a3a5-107">After a **completeMigration** request is made, you cannot import additional messages into the team.</span></span> <span data-ttu-id="3a3a5-108">Вы можете добавить членов в команду после успешного ответа на запрос.</span><span class="sxs-lookup"><span data-stu-id="3a3a5-108">You can add members to the team after the request returns a successful response.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a3a5-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a3a5-109">Permissions</span></span>

<span data-ttu-id="3a3a5-110">Для вызова этого API требуется следующее разрешение.</span><span class="sxs-lookup"><span data-stu-id="3a3a5-110">The following permission is required to call this API.</span></span> <span data-ttu-id="3a3a5-111">Дополнительные дополнительные новости *см. в см. в* ["Разрешениях".](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="3a3a5-111">To learn more, *see* [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a3a5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a3a5-112">Permission type</span></span>      | <span data-ttu-id="3a3a5-113">Разрешение</span><span class="sxs-lookup"><span data-stu-id="3a3a5-113">Permission</span></span>  |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="3a3a5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a3a5-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="3a3a5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a3a5-115">Not supported.</span></span>|
| <span data-ttu-id="3a3a5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a3a5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a3a5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a3a5-117">Not supported.</span></span> |
|<span data-ttu-id="3a3a5-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a3a5-118">Application</span></span> | <span data-ttu-id="3a3a5-119">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="3a3a5-119">Teamwork.Migrate.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a3a5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a3a5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/completeMigration
```

## <a name="request-headers"></a><span data-ttu-id="3a3a5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a3a5-121">Request headers</span></span>

| <span data-ttu-id="3a3a5-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a3a5-122">Header</span></span>       | <span data-ttu-id="3a3a5-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3a3a5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a3a5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a3a5-124">Authorization</span></span>  | <span data-ttu-id="3a3a5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a3a5-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a3a5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a3a5-127">Request body</span></span>

<span data-ttu-id="3a3a5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a3a5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a3a5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a3a5-129">Response</span></span>

<span data-ttu-id="3a3a5-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3a3a5-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a3a5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3a3a5-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a3a5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a3a5-133">Request</span></span>

<span data-ttu-id="3a3a5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a3a5-134">The following is an example of the request.</span></span>
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD022 -->


<!-- {
  "blockType": "request",
  "name": "completeMigration_channel"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/completeMigration
```


<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="3a3a5-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a3a5-135">Response</span></span>

<span data-ttu-id="3a3a5-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3a3a5-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 5793eec6-0e5a-11eb-adc1-0242ac120002
2020-10-14 20:22:11 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "completeMigration_ channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
