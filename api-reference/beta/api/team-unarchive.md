---
title: Распаковка объекта команды
description: Восстановление архивной команды. Это восстанавливает возможность пользователей отправлять сообщения и редактировать команду, абидинг по клиенту и параметрам группы. Архивация Teams выполняется с помощью API архива.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 0c39cac6a61f09c0531f1c337ff01e1b3c077b67
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536804"
---
# <a name="unarchive-team"></a><span data-ttu-id="f3c92-105">Распаковка объекта команды</span><span class="sxs-lookup"><span data-stu-id="f3c92-105">Unarchive team</span></span>



<span data-ttu-id="f3c92-106">Восстановление архивной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="f3c92-106">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="f3c92-107">Это восстанавливает возможность пользователей отправлять сообщения и редактировать команду, абидинг по клиенту и параметрам группы.</span><span class="sxs-lookup"><span data-stu-id="f3c92-107">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="f3c92-108">Архивация Teams выполняется с помощью API [архива](team-archive.md) .</span><span class="sxs-lookup"><span data-stu-id="f3c92-108">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="f3c92-109">Unarchivingя это асинхронная операция.</span><span class="sxs-lookup"><span data-stu-id="f3c92-109">Unarchiving is an async operation.</span></span> <span data-ttu-id="f3c92-110">Команда не архивируется после успешного завершения асинхронной операции, которая может произойти после ответа от этого API.</span><span class="sxs-lookup"><span data-stu-id="f3c92-110">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3c92-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3c92-111">Permissions</span></span>
<span data-ttu-id="f3c92-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3c92-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3c92-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3c92-114">Permission type</span></span>      | <span data-ttu-id="f3c92-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3c92-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3c92-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3c92-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f3c92-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3c92-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f3c92-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3c92-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3c92-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3c92-119">Not supported.</span></span>    |
|<span data-ttu-id="f3c92-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3c92-120">Application</span></span> | <span data-ttu-id="f3c92-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3c92-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="f3c92-122">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="f3c92-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f3c92-123">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="f3c92-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f3c92-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3c92-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="f3c92-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3c92-125">Request headers</span></span>
| <span data-ttu-id="f3c92-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3c92-126">Header</span></span>       | <span data-ttu-id="f3c92-127">Значение</span><span class="sxs-lookup"><span data-stu-id="f3c92-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f3c92-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3c92-128">Authorization</span></span>  | <span data-ttu-id="f3c92-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3c92-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f3c92-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3c92-131">Request body</span></span>
<span data-ttu-id="f3c92-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3c92-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3c92-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3c92-133">Response</span></span>

<span data-ttu-id="f3c92-134">В случае успешного запуска unarchivingи этот метод возвращает код `202 Accepted` отклика.</span><span class="sxs-lookup"><span data-stu-id="f3c92-134">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="f3c92-135">Ответ также будет содержать `Location` заголовок, который содержит расположение [теамсасинкоператион](../resources/teamsasyncoperation.md) , созданного для обработки отмененного архивирования команды.</span><span class="sxs-lookup"><span data-stu-id="f3c92-135">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="f3c92-136">Проверьте состояние операции расархивации, выполнив запрос GET к этому расположению.</span><span class="sxs-lookup"><span data-stu-id="f3c92-136">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="f3c92-137">Пример</span><span class="sxs-lookup"><span data-stu-id="f3c92-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f3c92-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3c92-138">Request</span></span>
<span data-ttu-id="f3c92-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3c92-139">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="f3c92-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3c92-140">Response</span></span>
<span data-ttu-id="f3c92-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f3c92-141">The following is an example of a response.</span></span>
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
