---
title: Распаковка объекта команды
description: Восстановление архивной команды. Это восстанавливает возможность пользователей отправлять сообщения и редактировать команду, абидинг по клиенту и параметрам группы. Архивация Teams выполняется с помощью API архива.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3529cfe38d6fa17b25df412b65ca9e2d42a18aff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509344"
---
# <a name="unarchive-team"></a><span data-ttu-id="91dbe-105">Распаковка объекта команды</span><span class="sxs-lookup"><span data-stu-id="91dbe-105">Unarchive team</span></span>

<span data-ttu-id="91dbe-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91dbe-106">Namespace: microsoft.graph</span></span>



<span data-ttu-id="91dbe-107">Восстановление архивной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="91dbe-107">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="91dbe-108">Это восстанавливает возможность пользователей отправлять сообщения и редактировать команду, абидинг по клиенту и параметрам группы.</span><span class="sxs-lookup"><span data-stu-id="91dbe-108">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="91dbe-109">Архивация Teams выполняется с помощью API [архива](team-archive.md) .</span><span class="sxs-lookup"><span data-stu-id="91dbe-109">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="91dbe-110">Unarchivingя это асинхронная операция.</span><span class="sxs-lookup"><span data-stu-id="91dbe-110">Unarchiving is an async operation.</span></span> <span data-ttu-id="91dbe-111">Команда не архивируется после успешного завершения асинхронной операции, которая может произойти после ответа от этого API.</span><span class="sxs-lookup"><span data-stu-id="91dbe-111">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="91dbe-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91dbe-112">Permissions</span></span>
<span data-ttu-id="91dbe-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91dbe-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91dbe-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91dbe-115">Permission type</span></span>      | <span data-ttu-id="91dbe-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91dbe-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91dbe-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91dbe-117">Delegated (work or school account)</span></span> | <span data-ttu-id="91dbe-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91dbe-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="91dbe-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91dbe-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91dbe-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91dbe-120">Not supported.</span></span>    |
|<span data-ttu-id="91dbe-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91dbe-121">Application</span></span> | <span data-ttu-id="91dbe-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91dbe-122">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="91dbe-123">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="91dbe-123">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="91dbe-124">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="91dbe-124">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="91dbe-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91dbe-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="91dbe-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91dbe-126">Request headers</span></span>
| <span data-ttu-id="91dbe-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91dbe-127">Header</span></span>       | <span data-ttu-id="91dbe-128">Значение</span><span class="sxs-lookup"><span data-stu-id="91dbe-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="91dbe-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91dbe-129">Authorization</span></span>  | <span data-ttu-id="91dbe-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91dbe-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="91dbe-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="91dbe-132">Request body</span></span>
<span data-ttu-id="91dbe-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91dbe-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91dbe-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="91dbe-134">Response</span></span>

<span data-ttu-id="91dbe-135">В случае успешного запуска unarchivingи этот метод возвращает код `202 Accepted` отклика.</span><span class="sxs-lookup"><span data-stu-id="91dbe-135">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="91dbe-136">Ответ также будет содержать `Location` заголовок, который содержит расположение [теамсасинкоператион](../resources/teamsasyncoperation.md) , созданного для обработки отмененного архивирования команды.</span><span class="sxs-lookup"><span data-stu-id="91dbe-136">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="91dbe-137">Проверьте состояние операции расархивации, выполнив запрос GET к этому расположению.</span><span class="sxs-lookup"><span data-stu-id="91dbe-137">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="91dbe-138">Пример</span><span class="sxs-lookup"><span data-stu-id="91dbe-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="91dbe-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="91dbe-139">Request</span></span>
<span data-ttu-id="91dbe-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91dbe-140">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="91dbe-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="91dbe-141">Response</span></span>
<span data-ttu-id="91dbe-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="91dbe-142">The following is an example of a response.</span></span>
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
