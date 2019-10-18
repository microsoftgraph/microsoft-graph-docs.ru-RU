---
title: Архивация команды
description: 'Архивация указанной команды. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cb2a6ca3962804ae9fc4ae85d1b8db93ead9bac6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021167"
---
# <a name="archive-team"></a><span data-ttu-id="416af-103">Архивация команды</span><span class="sxs-lookup"><span data-stu-id="416af-103">Archive team</span></span>



<span data-ttu-id="416af-104">Архивация указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="416af-104">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="416af-105">При архивации команды пользователь больше не сможет отправлять сообщения в любой канал команды или присваивать сообщениям отметку "Нравится", изменять название команды, описание, другие параметры и в целом вносить большинство изменений в команду.</span><span class="sxs-lookup"><span data-stu-id="416af-105">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="416af-106">Изменение участия в команде по-прежнему допускается.</span><span class="sxs-lookup"><span data-stu-id="416af-106">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="416af-107">Архивация — это асинхронная операция.</span><span class="sxs-lookup"><span data-stu-id="416af-107">Archiving is an async operation.</span></span> <span data-ttu-id="416af-108">Команда архивируется после успешного завершения асинхронной операции, которая может выполняться после отклика этого API.</span><span class="sxs-lookup"><span data-stu-id="416af-108">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="416af-109">Чтобы архивировать команду, у команды и [группы](../resources/group.md) должен быть владелец.</span><span class="sxs-lookup"><span data-stu-id="416af-109">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="416af-110">Чтобы восстановить команду из архивированного состояния, используйте API для [распаковки](team-unarchive.md).</span><span class="sxs-lookup"><span data-stu-id="416af-110">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="416af-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="416af-111">Permissions</span></span>
<span data-ttu-id="416af-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="416af-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="416af-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="416af-114">Permission type</span></span>      | <span data-ttu-id="416af-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="416af-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="416af-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="416af-116">Delegated (work or school account)</span></span> | <span data-ttu-id="416af-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="416af-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="416af-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="416af-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="416af-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="416af-119">Not supported.</span></span>    |
|<span data-ttu-id="416af-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="416af-120">Application</span></span> | <span data-ttu-id="416af-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="416af-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="416af-122">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="416af-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="416af-123">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="416af-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="416af-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="416af-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="416af-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="416af-125">Request headers</span></span>
| <span data-ttu-id="416af-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="416af-126">Header</span></span>       | <span data-ttu-id="416af-127">Значение</span><span class="sxs-lookup"><span data-stu-id="416af-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="416af-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="416af-128">Authorization</span></span>  | <span data-ttu-id="416af-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="416af-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="416af-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="416af-131">Request body</span></span>
<span data-ttu-id="416af-132">В запросе можно _при необходимости_ включить параметр `shouldSetSpoSiteReadOnlyForMembers` в текст JSON следующим образом.</span><span class="sxs-lookup"><span data-stu-id="416af-132">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="416af-133">Этот необязательный параметр определяет, следует ли для участников команды задать разрешения только для чтения на сайте Sharepoint Online, связанном с командой.</span><span class="sxs-lookup"><span data-stu-id="416af-133">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="416af-134">Если присвоить ему значение false или не указать текст, этот этап будет пропущен.</span><span class="sxs-lookup"><span data-stu-id="416af-134">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="416af-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="416af-135">Response</span></span>

<span data-ttu-id="416af-136">Если архивация начата успешно, этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="416af-136">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="416af-137">Отклик также будет содержать заголовок `Location`, в котором указывается расположение ресурса [teamsAsyncOperation](../resources/teamsasyncoperation.md), созданного для обработки архивации команды.</span><span class="sxs-lookup"><span data-stu-id="416af-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="416af-138">Проверьте состояние операции архивации, выполнив запрос GET для этого расположения.</span><span class="sxs-lookup"><span data-stu-id="416af-138">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="416af-139">Пример</span><span class="sxs-lookup"><span data-stu-id="416af-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="416af-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="416af-140">Request</span></span>
<span data-ttu-id="416af-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="416af-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="416af-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="416af-142">Response</span></span>
<span data-ttu-id="416af-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="416af-143">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
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
