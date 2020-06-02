---
title: Распаковка объекта команды
description: Восстановление архивной команды. Это восстанавливает возможность пользователей отправлять сообщения и редактировать команду, абидинг по клиенту и параметрам группы. Архивация Teams выполняется с помощью API архива.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cdf4ac0b7687836559614d2b51d04f831a9ff0f2
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491912"
---
# <a name="unarchive-team"></a><span data-ttu-id="937da-105">Распаковка объекта команды</span><span class="sxs-lookup"><span data-stu-id="937da-105">Unarchive team</span></span>

<span data-ttu-id="937da-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="937da-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="937da-107">Восстановление архивной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="937da-107">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="937da-108">Это восстанавливает возможность пользователей отправлять сообщения и редактировать команду, абидинг по клиенту и параметрам группы.</span><span class="sxs-lookup"><span data-stu-id="937da-108">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="937da-109">Архивация Teams выполняется с помощью API [архива](team-archive.md) .</span><span class="sxs-lookup"><span data-stu-id="937da-109">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="937da-110">Unarchivingя это асинхронная операция.</span><span class="sxs-lookup"><span data-stu-id="937da-110">Unarchiving is an async operation.</span></span> <span data-ttu-id="937da-111">Команда не архивируется после успешного завершения асинхронной операции, которая может произойти после ответа от этого API.</span><span class="sxs-lookup"><span data-stu-id="937da-111">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="937da-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="937da-112">Permissions</span></span>
<span data-ttu-id="937da-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="937da-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="937da-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="937da-115">Permission type</span></span>      | <span data-ttu-id="937da-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="937da-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="937da-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="937da-117">Delegated (work or school account)</span></span> | <span data-ttu-id="937da-118">Теамсеттингс. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="937da-118">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="937da-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="937da-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="937da-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="937da-120">Not supported.</span></span>    |
|<span data-ttu-id="937da-121">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="937da-121">Application</span></span> | <span data-ttu-id="937da-122">Теамсеттингс. Edit. Group \*, Теамсеттингс. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="937da-122">TeamSettings.Edit.Group\*, TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="937da-123">**Note**: разрешения, помеченные как \* использовать [согласие с определенным ресурсом](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="937da-123">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="937da-124">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="937da-124">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="937da-125">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="937da-125">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="937da-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="937da-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="937da-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="937da-127">Request headers</span></span>
| <span data-ttu-id="937da-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="937da-128">Header</span></span>       | <span data-ttu-id="937da-129">Значение</span><span class="sxs-lookup"><span data-stu-id="937da-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="937da-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="937da-130">Authorization</span></span>  | <span data-ttu-id="937da-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="937da-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="937da-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="937da-133">Request body</span></span>
<span data-ttu-id="937da-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="937da-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="937da-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="937da-135">Response</span></span>

<span data-ttu-id="937da-136">В случае успешного запуска unarchivingи этот метод возвращает `202 Accepted` код отклика.</span><span class="sxs-lookup"><span data-stu-id="937da-136">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="937da-137">Ответ также будет содержать `Location` заголовок, который содержит расположение [теамсасинкоператион](../resources/teamsasyncoperation.md) , созданного для обработки отмененного архивирования команды.</span><span class="sxs-lookup"><span data-stu-id="937da-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="937da-138">Проверьте состояние операции расархивации, выполнив запрос GET к этому расположению.</span><span class="sxs-lookup"><span data-stu-id="937da-138">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="937da-139">Пример</span><span class="sxs-lookup"><span data-stu-id="937da-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="937da-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="937da-140">Request</span></span>
<span data-ttu-id="937da-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="937da-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="937da-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="937da-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```
# <a name="c"></a>[<span data-ttu-id="937da-143">C#</span><span class="sxs-lookup"><span data-stu-id="937da-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unarchive-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="937da-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="937da-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unarchive-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="937da-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="937da-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unarchive-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="937da-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="937da-146">Response</span></span>
<span data-ttu-id="937da-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="937da-147">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "name": "unarchive_team"
}-->
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 9a9bb83f-6f35-4426-bb04-73ca43ad6cc8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
