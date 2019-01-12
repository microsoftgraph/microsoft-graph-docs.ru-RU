---
title: Группа архива
description: 'Архивируйте указанной группы. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c5bfabb7fc6c57f79cf04b58e8b8196a00b284a7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947822"
---
# <a name="archive-team"></a><span data-ttu-id="8e046-103">Группа архива</span><span class="sxs-lookup"><span data-stu-id="8e046-103">Archive team</span></span>

> <span data-ttu-id="8e046-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8e046-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e046-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e046-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8e046-106">Архивируйте указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="8e046-106">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="8e046-107">При архивации группы, пользователи могут больше не отправлять или как сообщения на любом рабочих групп, изменить имя группы, описание или другие параметры или в целом изменять большинство в группу.</span><span class="sxs-lookup"><span data-stu-id="8e046-107">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="8e046-108">Изменения членства в группе продолжать разрешено.</span><span class="sxs-lookup"><span data-stu-id="8e046-108">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="8e046-109">Архивация — это асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="8e046-109">Archiving is an async operation.</span></span> <span data-ttu-id="8e046-110">Группа архивируется после асинхронного успешного завершения операции, которой может произойти после ответа от этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="8e046-110">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="8e046-111">Для архивации группы, группы и [группы](../resources/group.md) должен иметь владельца.</span><span class="sxs-lookup"><span data-stu-id="8e046-111">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="8e046-112">Чтобы восстановить группы из состояния архивных, используйте API-интерфейса [unarchive](team-unarchive.md).</span><span class="sxs-lookup"><span data-stu-id="8e046-112">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8e046-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e046-113">Permissions</span></span>
<span data-ttu-id="8e046-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e046-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e046-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e046-116">Permission type</span></span>      | <span data-ttu-id="8e046-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e046-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e046-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e046-118">Delegated (work or school account)</span></span> | <span data-ttu-id="8e046-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e046-119">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8e046-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e046-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e046-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e046-121">Not supported.</span></span>    |
|<span data-ttu-id="8e046-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e046-122">Application</span></span> | <span data-ttu-id="8e046-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e046-123">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="8e046-124">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="8e046-124">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8e046-125">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="8e046-125">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8e046-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e046-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="8e046-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e046-127">Request headers</span></span>
| <span data-ttu-id="8e046-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e046-128">Header</span></span>       | <span data-ttu-id="8e046-129">Значение</span><span class="sxs-lookup"><span data-stu-id="8e046-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8e046-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e046-130">Authorization</span></span>  | <span data-ttu-id="8e046-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e046-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e046-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8e046-133">Request body</span></span>
<span data-ttu-id="8e046-134">В запросе, можно _Дополнительно_ включить `shouldSetSpoSiteReadOnlyForMembers` параметр в формате JSON в body следующим образом.</span><span class="sxs-lookup"><span data-stu-id="8e046-134">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="8e046-135">Этот дополнительный параметр определяет, требуется ли задавать разрешения для членов группы только для чтения на сайте Sharepoint Online, связанный с группой.</span><span class="sxs-lookup"><span data-stu-id="8e046-135">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="8e046-136">Задать значение false или пропуск текста полностью приведет к этот шаг пропущен.</span><span class="sxs-lookup"><span data-stu-id="8e046-136">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="8e046-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e046-137">Response</span></span>

<span data-ttu-id="8e046-138">Если архивация запускается успешно, этот метод возвращает `202 Accepted` код ответа.</span><span class="sxs-lookup"><span data-stu-id="8e046-138">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="8e046-139">Ответ также будет содержать `Location` заголовок, который содержит расположение [teamsAsyncOperation](../resources/teamsasyncoperation.md) , который был создан для обработки архивации рабочей группы.</span><span class="sxs-lookup"><span data-stu-id="8e046-139">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="8e046-140">Проверьте состояние архивации операции, внесение запрос GET в этом расположении.</span><span class="sxs-lookup"><span data-stu-id="8e046-140">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="8e046-141">Пример</span><span class="sxs-lookup"><span data-stu-id="8e046-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8e046-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e046-142">Request</span></span>
<span data-ttu-id="8e046-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e046-143">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="8e046-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e046-144">Response</span></span>
<span data-ttu-id="8e046-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8e046-145">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
