---
title: Unarchive группы
description: Восстановление архивированных группы. Это восстанавливает возможность отправлять сообщения и изменение группы, сотрудничает с параметры клиента и группы. Команды архивируются использования API архива.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: b5c64c9c04c7c3cc3549721747c27361680bd03a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977670"
---
# <a name="unarchive-team"></a><span data-ttu-id="839ec-105">Unarchive группы</span><span class="sxs-lookup"><span data-stu-id="839ec-105">Unarchive team</span></span>

> <span data-ttu-id="839ec-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="839ec-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="839ec-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="839ec-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="839ec-108">Восстановление архивированных [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="839ec-108">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="839ec-109">Это восстанавливает возможность отправлять сообщения и изменение группы, сотрудничает с параметры клиента и группы.</span><span class="sxs-lookup"><span data-stu-id="839ec-109">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="839ec-110">Команды, архивируются использования [архива](team-archive.md) API.</span><span class="sxs-lookup"><span data-stu-id="839ec-110">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="839ec-111">Unarchiving является асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="839ec-111">Unarchiving is an async operation.</span></span> <span data-ttu-id="839ec-112">Группа архиве после асинхронного успешного завершения операции, которой может произойти после ответа от этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="839ec-112">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="839ec-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="839ec-113">Permissions</span></span>
<span data-ttu-id="839ec-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="839ec-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="839ec-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="839ec-116">Permission type</span></span>      | <span data-ttu-id="839ec-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="839ec-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="839ec-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="839ec-118">Delegated (work or school account)</span></span> | <span data-ttu-id="839ec-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="839ec-119">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="839ec-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="839ec-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="839ec-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="839ec-121">Not supported.</span></span>    |
|<span data-ttu-id="839ec-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="839ec-122">Application</span></span> | <span data-ttu-id="839ec-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="839ec-123">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="839ec-124">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="839ec-124">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="839ec-125">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="839ec-125">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="839ec-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="839ec-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="839ec-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="839ec-127">Request headers</span></span>
| <span data-ttu-id="839ec-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="839ec-128">Header</span></span>       | <span data-ttu-id="839ec-129">Значение</span><span class="sxs-lookup"><span data-stu-id="839ec-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="839ec-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="839ec-130">Authorization</span></span>  | <span data-ttu-id="839ec-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="839ec-p107">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="839ec-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="839ec-133">Request body</span></span>
<span data-ttu-id="839ec-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="839ec-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="839ec-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="839ec-135">Response</span></span>

<span data-ttu-id="839ec-136">Если unarchiving запускается успешно, этот метод возвращает `202 Accepted` код ответа.</span><span class="sxs-lookup"><span data-stu-id="839ec-136">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="839ec-137">Ответ также будет содержать `Location` заголовок, который содержит расположение [teamsAsyncOperation](../resources/teamsasyncoperation.md) , который был создан для обработки unarchiving рабочей группы.</span><span class="sxs-lookup"><span data-stu-id="839ec-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="839ec-138">Проверьте состояние unarchiving операции, внесение запрос GET в этом расположении.</span><span class="sxs-lookup"><span data-stu-id="839ec-138">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="839ec-139">Пример</span><span class="sxs-lookup"><span data-stu-id="839ec-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="839ec-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="839ec-140">Request</span></span>
<span data-ttu-id="839ec-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="839ec-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="839ec-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="839ec-142">Response</span></span>
<span data-ttu-id="839ec-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="839ec-143">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
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
