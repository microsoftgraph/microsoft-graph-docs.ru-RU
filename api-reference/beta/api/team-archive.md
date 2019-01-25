---
title: Группа архива
description: 'Архивируйте указанной группы. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1f60ffc8526d40bc373045e207a4877fb91f694d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507826"
---
# <a name="archive-team"></a><span data-ttu-id="d6500-103">Группа архива</span><span class="sxs-lookup"><span data-stu-id="d6500-103">Archive team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6500-104">Архивируйте указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="d6500-104">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="d6500-105">При архивации группы, пользователи могут больше не отправлять или как сообщения на любом рабочих групп, изменить имя группы, описание или другие параметры или в целом изменять большинство в группу.</span><span class="sxs-lookup"><span data-stu-id="d6500-105">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="d6500-106">Изменения членства в группе продолжать разрешено.</span><span class="sxs-lookup"><span data-stu-id="d6500-106">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="d6500-107">Архивация — это асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="d6500-107">Archiving is an async operation.</span></span> <span data-ttu-id="d6500-108">Группа архивируется после асинхронного успешного завершения операции, которой может произойти после ответа от этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="d6500-108">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="d6500-109">Для архивации группы, группы и [группы](../resources/group.md) должен иметь владельца.</span><span class="sxs-lookup"><span data-stu-id="d6500-109">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="d6500-110">Чтобы восстановить группы из состояния архивных, используйте API-интерфейса [unarchive](team-unarchive.md).</span><span class="sxs-lookup"><span data-stu-id="d6500-110">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d6500-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6500-111">Permissions</span></span>
<span data-ttu-id="d6500-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6500-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6500-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6500-114">Permission type</span></span>      | <span data-ttu-id="d6500-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6500-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6500-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6500-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d6500-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6500-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d6500-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6500-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6500-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6500-119">Not supported.</span></span>    |
|<span data-ttu-id="d6500-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6500-120">Application</span></span> | <span data-ttu-id="d6500-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6500-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="d6500-122">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="d6500-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d6500-123">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="d6500-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d6500-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6500-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="d6500-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6500-125">Request headers</span></span>
| <span data-ttu-id="d6500-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6500-126">Header</span></span>       | <span data-ttu-id="d6500-127">Значение</span><span class="sxs-lookup"><span data-stu-id="d6500-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d6500-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6500-128">Authorization</span></span>  | <span data-ttu-id="d6500-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6500-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d6500-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6500-131">Request body</span></span>
<span data-ttu-id="d6500-132">В запросе, можно _Дополнительно_ включить `shouldSetSpoSiteReadOnlyForMembers` параметр в формате JSON в body следующим образом.</span><span class="sxs-lookup"><span data-stu-id="d6500-132">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="d6500-133">Этот дополнительный параметр определяет, требуется ли задавать разрешения для членов группы только для чтения на сайте Sharepoint Online, связанный с группой.</span><span class="sxs-lookup"><span data-stu-id="d6500-133">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="d6500-134">Задать значение false или пропуск текста полностью приведет к этот шаг пропущен.</span><span class="sxs-lookup"><span data-stu-id="d6500-134">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="d6500-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6500-135">Response</span></span>

<span data-ttu-id="d6500-136">Если архивация запускается успешно, этот метод возвращает `202 Accepted` код ответа.</span><span class="sxs-lookup"><span data-stu-id="d6500-136">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="d6500-137">Ответ также будет содержать `Location` заголовок, который содержит расположение [teamsAsyncOperation](../resources/teamsasyncoperation.md) , который был создан для обработки архивации рабочей группы.</span><span class="sxs-lookup"><span data-stu-id="d6500-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="d6500-138">Проверьте состояние архивации операции, внесение запрос GET в этом расположении.</span><span class="sxs-lookup"><span data-stu-id="d6500-138">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="d6500-139">Пример</span><span class="sxs-lookup"><span data-stu-id="d6500-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d6500-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6500-140">Request</span></span>
<span data-ttu-id="d6500-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6500-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="d6500-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6500-142">Response</span></span>
<span data-ttu-id="d6500-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d6500-143">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/team-archive.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
