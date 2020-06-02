---
title: Архивация команды
description: 'Архивация указанной команды. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c62a8aca9e5c3c3838f9a4d9ec83fea0fd87f173
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491793"
---
# <a name="archive-team"></a><span data-ttu-id="80a82-103">Архивация команды</span><span class="sxs-lookup"><span data-stu-id="80a82-103">Archive team</span></span>

<span data-ttu-id="80a82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80a82-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="80a82-105">Архивация указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="80a82-105">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="80a82-106">При архивации команды пользователь больше не сможет отправлять сообщения в любой канал команды или присваивать сообщениям отметку "Нравится", изменять название команды, описание, другие параметры и в целом вносить большинство изменений в команду.</span><span class="sxs-lookup"><span data-stu-id="80a82-106">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="80a82-107">Изменение участия в команде по-прежнему допускается.</span><span class="sxs-lookup"><span data-stu-id="80a82-107">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="80a82-108">Архивация — это асинхронная операция.</span><span class="sxs-lookup"><span data-stu-id="80a82-108">Archiving is an async operation.</span></span> <span data-ttu-id="80a82-109">Команда архивируется после успешного завершения асинхронной операции, которая может выполняться после отклика этого API.</span><span class="sxs-lookup"><span data-stu-id="80a82-109">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="80a82-110">Чтобы архивировать команду, у команды и [группы](../resources/group.md) должен быть владелец.</span><span class="sxs-lookup"><span data-stu-id="80a82-110">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="80a82-111">Чтобы восстановить команду из архивированного состояния, используйте API для [распаковки](team-unarchive.md).</span><span class="sxs-lookup"><span data-stu-id="80a82-111">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="80a82-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80a82-112">Permissions</span></span>
<span data-ttu-id="80a82-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80a82-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80a82-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80a82-115">Permission type</span></span>      | <span data-ttu-id="80a82-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80a82-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80a82-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80a82-117">Delegated (work or school account)</span></span> | <span data-ttu-id="80a82-118">Теамсеттингс. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="80a82-118">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="80a82-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80a82-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80a82-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80a82-120">Not supported.</span></span>    |
|<span data-ttu-id="80a82-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80a82-121">Application</span></span> |<span data-ttu-id="80a82-122">Теамсеттингс. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="80a82-122">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="80a82-123">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="80a82-123">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="80a82-124">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="80a82-124">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="80a82-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80a82-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="80a82-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80a82-126">Request headers</span></span>
| <span data-ttu-id="80a82-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="80a82-127">Header</span></span>       | <span data-ttu-id="80a82-128">Значение</span><span class="sxs-lookup"><span data-stu-id="80a82-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="80a82-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80a82-129">Authorization</span></span>  | <span data-ttu-id="80a82-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80a82-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="80a82-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80a82-132">Request body</span></span>
<span data-ttu-id="80a82-133">В запросе можно _при необходимости_ включить параметр `shouldSetSpoSiteReadOnlyForMembers` в текст JSON следующим образом.</span><span class="sxs-lookup"><span data-stu-id="80a82-133">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="80a82-134">Этот необязательный параметр определяет, следует ли для участников команды задать разрешения только для чтения на сайте Sharepoint Online, связанном с командой.</span><span class="sxs-lookup"><span data-stu-id="80a82-134">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="80a82-135">Если присвоить ему значение false или не указать текст, этот этап будет пропущен.</span><span class="sxs-lookup"><span data-stu-id="80a82-135">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

>[!IMPORTANT]
><span data-ttu-id="80a82-136">Параметр `shouldSetSpoSiteReadOnlyForMembers` не поддерживается в контексте приложения.</span><span class="sxs-lookup"><span data-stu-id="80a82-136">The `shouldSetSpoSiteReadOnlyForMembers` parameter is not supported in the application context.</span></span>

## <a name="response"></a><span data-ttu-id="80a82-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="80a82-137">Response</span></span>

<span data-ttu-id="80a82-138">Если архивация начата успешно, этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="80a82-138">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="80a82-139">Отклик также будет содержать заголовок `Location`, в котором указывается расположение ресурса [teamsAsyncOperation](../resources/teamsasyncoperation.md), созданного для обработки архивации команды.</span><span class="sxs-lookup"><span data-stu-id="80a82-139">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="80a82-140">Проверьте состояние операции архивации, выполнив запрос GET для этого расположения.</span><span class="sxs-lookup"><span data-stu-id="80a82-140">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="80a82-141">Пример</span><span class="sxs-lookup"><span data-stu-id="80a82-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="80a82-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="80a82-142">Request</span></span>
<span data-ttu-id="80a82-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80a82-143">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="80a82-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="80a82-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/archive
```
# <a name="c"></a>[<span data-ttu-id="80a82-145">C#</span><span class="sxs-lookup"><span data-stu-id="80a82-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/archive-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80a82-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80a82-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/archive-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80a82-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80a82-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/archive-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80a82-148">Java</span><span class="sxs-lookup"><span data-stu-id="80a82-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/archive-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="80a82-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="80a82-149">Response</span></span>
<span data-ttu-id="80a82-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="80a82-150">The following is an example of a response.</span></span>

<!-- {
  "blockType": "response",
  "name": "archive_team"
}-->
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
