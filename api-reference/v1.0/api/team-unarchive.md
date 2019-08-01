---
title: Распаковка объекта команды
description: Восстановление архивной команды. Это восстанавливает возможность пользователей отправлять сообщения и редактировать команду, абидинг по клиенту и параметрам группы. Архивация Teams выполняется с помощью API архива.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 011b68f2e85c041ccb0f654295dfaf1a42d5d237
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024226"
---
# <a name="unarchive-team"></a><span data-ttu-id="9fad3-105">Распаковка объекта команды</span><span class="sxs-lookup"><span data-stu-id="9fad3-105">Unarchive team</span></span>



<span data-ttu-id="9fad3-106">Восстановление архивной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="9fad3-106">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="9fad3-107">Это восстанавливает возможность пользователей отправлять сообщения и редактировать команду, абидинг по клиенту и параметрам группы.</span><span class="sxs-lookup"><span data-stu-id="9fad3-107">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="9fad3-108">Архивация Teams выполняется с помощью API [архива](team-archive.md) .</span><span class="sxs-lookup"><span data-stu-id="9fad3-108">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="9fad3-109">Unarchivingя это асинхронная операция.</span><span class="sxs-lookup"><span data-stu-id="9fad3-109">Unarchiving is an async operation.</span></span> <span data-ttu-id="9fad3-110">Команда не архивируется после успешного завершения асинхронной операции, которая может произойти после ответа от этого API.</span><span class="sxs-lookup"><span data-stu-id="9fad3-110">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fad3-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9fad3-111">Permissions</span></span>
<span data-ttu-id="9fad3-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fad3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fad3-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fad3-114">Permission type</span></span>      | <span data-ttu-id="9fad3-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fad3-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fad3-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fad3-116">Delegated (work or school account)</span></span> | <span data-ttu-id="9fad3-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fad3-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9fad3-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fad3-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fad3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fad3-119">Not supported.</span></span>    |
|<span data-ttu-id="9fad3-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9fad3-120">Application</span></span> | <span data-ttu-id="9fad3-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fad3-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="9fad3-122">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="9fad3-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9fad3-123">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="9fad3-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9fad3-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fad3-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="9fad3-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9fad3-125">Request headers</span></span>
| <span data-ttu-id="9fad3-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9fad3-126">Header</span></span>       | <span data-ttu-id="9fad3-127">Значение</span><span class="sxs-lookup"><span data-stu-id="9fad3-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9fad3-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9fad3-128">Authorization</span></span>  | <span data-ttu-id="9fad3-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fad3-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9fad3-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9fad3-131">Request body</span></span>
<span data-ttu-id="9fad3-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9fad3-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fad3-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="9fad3-133">Response</span></span>

<span data-ttu-id="9fad3-134">В случае успешного запуска unarchivingи этот метод возвращает код `202 Accepted` отклика.</span><span class="sxs-lookup"><span data-stu-id="9fad3-134">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="9fad3-135">Ответ также будет содержать `Location` заголовок, который содержит расположение [теамсасинкоператион](../resources/teamsasyncoperation.md) , созданного для обработки отмененного архивирования команды.</span><span class="sxs-lookup"><span data-stu-id="9fad3-135">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="9fad3-136">Проверьте состояние операции расархивации, выполнив запрос GET к этому расположению.</span><span class="sxs-lookup"><span data-stu-id="9fad3-136">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="9fad3-137">Пример</span><span class="sxs-lookup"><span data-stu-id="9fad3-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9fad3-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fad3-138">Request</span></span>
<span data-ttu-id="9fad3-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fad3-139">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="9fad3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fad3-140">Response</span></span>
<span data-ttu-id="9fad3-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9fad3-141">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 9a9bb83f-6f35-4426-bb04-73ca43ad6cc8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
