---
title: Архивация команды
description: 'Архивация указанной команды. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8d7631524350c37a79913bbb4b37d0b6e9ee4651
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452609"
---
# <a name="archive-team"></a><span data-ttu-id="82cb1-103">Архивация команды</span><span class="sxs-lookup"><span data-stu-id="82cb1-103">Archive team</span></span>

<span data-ttu-id="82cb1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82cb1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82cb1-105">Архивация указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="82cb1-105">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="82cb1-106">При архивации команды пользователь больше не сможет отправлять сообщения в любой канал команды или присваивать сообщениям отметку "Нравится", изменять название команды, описание, другие параметры и в целом вносить большинство изменений в команду.</span><span class="sxs-lookup"><span data-stu-id="82cb1-106">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="82cb1-107">Изменение участия в команде по-прежнему допускается.</span><span class="sxs-lookup"><span data-stu-id="82cb1-107">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="82cb1-108">Архивация — это асинхронная операция.</span><span class="sxs-lookup"><span data-stu-id="82cb1-108">Archiving is an async operation.</span></span> <span data-ttu-id="82cb1-109">Команда архивируется после успешного завершения асинхронной операции, которая может выполняться после отклика этого API.</span><span class="sxs-lookup"><span data-stu-id="82cb1-109">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="82cb1-110">Чтобы архивировать команду, у команды и [группы](../resources/group.md) должен быть владелец.</span><span class="sxs-lookup"><span data-stu-id="82cb1-110">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="82cb1-111">Чтобы восстановить команду из архивированного состояния, используйте API для [распаковки](team-unarchive.md).</span><span class="sxs-lookup"><span data-stu-id="82cb1-111">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="82cb1-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82cb1-112">Permissions</span></span>
<span data-ttu-id="82cb1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82cb1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82cb1-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82cb1-115">Permission type</span></span>      | <span data-ttu-id="82cb1-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82cb1-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82cb1-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82cb1-117">Delegated (work or school account)</span></span> | <span data-ttu-id="82cb1-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82cb1-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="82cb1-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82cb1-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82cb1-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82cb1-120">Not supported.</span></span>    |
|<span data-ttu-id="82cb1-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82cb1-121">Application</span></span> | <span data-ttu-id="82cb1-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82cb1-122">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="82cb1-123">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="82cb1-123">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="82cb1-124">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="82cb1-124">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="82cb1-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82cb1-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="82cb1-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82cb1-126">Request headers</span></span>
| <span data-ttu-id="82cb1-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82cb1-127">Header</span></span>       | <span data-ttu-id="82cb1-128">Значение</span><span class="sxs-lookup"><span data-stu-id="82cb1-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="82cb1-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82cb1-129">Authorization</span></span>  | <span data-ttu-id="82cb1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82cb1-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="82cb1-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82cb1-132">Request body</span></span>
<span data-ttu-id="82cb1-133">В запросе можно _при необходимости_ включить параметр `shouldSetSpoSiteReadOnlyForMembers` в текст JSON следующим образом.</span><span class="sxs-lookup"><span data-stu-id="82cb1-133">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="82cb1-134">Этот необязательный параметр определяет, следует ли для участников команды задать разрешения только для чтения на сайте Sharepoint Online, связанном с командой.</span><span class="sxs-lookup"><span data-stu-id="82cb1-134">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="82cb1-135">Если присвоить ему значение false или не указать текст, этот этап будет пропущен.</span><span class="sxs-lookup"><span data-stu-id="82cb1-135">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="82cb1-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="82cb1-136">Response</span></span>

<span data-ttu-id="82cb1-137">Если архивация начата успешно, этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="82cb1-137">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="82cb1-138">Отклик также будет содержать заголовок `Location`, в котором указывается расположение ресурса [teamsAsyncOperation](../resources/teamsasyncoperation.md), созданного для обработки архивации команды.</span><span class="sxs-lookup"><span data-stu-id="82cb1-138">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="82cb1-139">Проверьте состояние операции архивации, выполнив запрос GET для этого расположения.</span><span class="sxs-lookup"><span data-stu-id="82cb1-139">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="82cb1-140">Пример</span><span class="sxs-lookup"><span data-stu-id="82cb1-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="82cb1-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="82cb1-141">Request</span></span>
<span data-ttu-id="82cb1-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82cb1-142">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="82cb1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="82cb1-143">Response</span></span>
<span data-ttu-id="82cb1-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="82cb1-144">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
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
  "suppressions": []
}
-->
