---
title: Архивация команды
description: 'Архивация указанной команды. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: da0d836eb6eea664cbc8a6bf2814a13dc33c4d03
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290358"
---
# <a name="archive-team"></a><span data-ttu-id="37a34-103">Архивация команды</span><span class="sxs-lookup"><span data-stu-id="37a34-103">Archive team</span></span>

<span data-ttu-id="37a34-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37a34-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37a34-105">Архивация указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="37a34-105">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="37a34-106">При архивации команды пользователь больше не сможет отправлять сообщения в любой канал команды или присваивать сообщениям отметку "Нравится", изменять название команды, описание, другие параметры и в целом вносить большинство изменений в команду.</span><span class="sxs-lookup"><span data-stu-id="37a34-106">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="37a34-107">Изменение участия в команде по-прежнему допускается.</span><span class="sxs-lookup"><span data-stu-id="37a34-107">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="37a34-108">Архивация — это асинхронная операция.</span><span class="sxs-lookup"><span data-stu-id="37a34-108">Archiving is an async operation.</span></span> <span data-ttu-id="37a34-109">Команда архивируется после успешного завершения асинхронной операции, которая может выполняться после отклика этого API.</span><span class="sxs-lookup"><span data-stu-id="37a34-109">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="37a34-110">Чтобы архивировать команду, у команды и [группы](../resources/group.md) должен быть владелец.</span><span class="sxs-lookup"><span data-stu-id="37a34-110">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="37a34-111">Чтобы восстановить команду из архивированного состояния, используйте API для [распаковки](team-unarchive.md).</span><span class="sxs-lookup"><span data-stu-id="37a34-111">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="37a34-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37a34-112">Permissions</span></span>
<span data-ttu-id="37a34-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37a34-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37a34-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37a34-115">Permission type</span></span>      | <span data-ttu-id="37a34-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37a34-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37a34-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37a34-117">Delegated (work or school account)</span></span> | <span data-ttu-id="37a34-118">Теамсеттингс. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="37a34-118">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="37a34-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37a34-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37a34-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37a34-120">Not supported.</span></span>    |
|<span data-ttu-id="37a34-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37a34-121">Application</span></span> | <span data-ttu-id="37a34-122">Теамсеттингс. Edit. Group ([RSC](https://aka.ms/teams-rsc)), Теамсеттингс. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="37a34-122">TeamSettings.Edit.Group ([RSC](https://aka.ms/teams-rsc)), TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="37a34-123">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="37a34-123">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="37a34-124">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="37a34-124">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="37a34-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37a34-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="37a34-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37a34-126">Request headers</span></span>
| <span data-ttu-id="37a34-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37a34-127">Header</span></span>       | <span data-ttu-id="37a34-128">Значение</span><span class="sxs-lookup"><span data-stu-id="37a34-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="37a34-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37a34-129">Authorization</span></span>  | <span data-ttu-id="37a34-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37a34-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="37a34-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37a34-132">Request body</span></span>
<span data-ttu-id="37a34-133">В запросе можно _при необходимости_ включить параметр `shouldSetSpoSiteReadOnlyForMembers` в текст JSON следующим образом.</span><span class="sxs-lookup"><span data-stu-id="37a34-133">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="37a34-134">Этот необязательный параметр определяет, следует ли для участников команды задать разрешения только для чтения на сайте Sharepoint Online, связанном с командой.</span><span class="sxs-lookup"><span data-stu-id="37a34-134">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="37a34-135">Если присвоить ему значение false или не указать текст, этот этап будет пропущен.</span><span class="sxs-lookup"><span data-stu-id="37a34-135">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

>[!IMPORTANT]
><span data-ttu-id="37a34-136">Параметр `shouldSetSpoSiteReadOnlyForMembers` не поддерживается в контексте приложения.</span><span class="sxs-lookup"><span data-stu-id="37a34-136">The `shouldSetSpoSiteReadOnlyForMembers` parameter is not supported in the application context.</span></span>

## <a name="response"></a><span data-ttu-id="37a34-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="37a34-137">Response</span></span>

<span data-ttu-id="37a34-138">Если архивация начата успешно, этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="37a34-138">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="37a34-139">Отклик также будет содержать заголовок `Location`, в котором указывается расположение ресурса [teamsAsyncOperation](../resources/teamsasyncoperation.md), созданного для обработки архивации команды.</span><span class="sxs-lookup"><span data-stu-id="37a34-139">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="37a34-140">Проверьте состояние операции архивации, выполнив запрос GET для этого расположения.</span><span class="sxs-lookup"><span data-stu-id="37a34-140">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="37a34-141">Пример</span><span class="sxs-lookup"><span data-stu-id="37a34-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="37a34-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="37a34-142">Request</span></span>
<span data-ttu-id="37a34-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37a34-143">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="37a34-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="37a34-144">Response</span></span>
<span data-ttu-id="37a34-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="37a34-145">The following is an example of a response.</span></span>
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
