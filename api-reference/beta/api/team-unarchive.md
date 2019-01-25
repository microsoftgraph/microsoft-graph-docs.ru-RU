---
title: Unarchive группы
description: Восстановление архивированных группы. Это восстанавливает возможность отправлять сообщения и изменение группы, сотрудничает с параметры клиента и группы. Команды архивируются использования API архива.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: d21eb7d3531b69e148c0d420217fc309e0ea99ad
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518137"
---
# <a name="unarchive-team"></a><span data-ttu-id="f417c-105">Unarchive группы</span><span class="sxs-lookup"><span data-stu-id="f417c-105">Unarchive team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f417c-106">Восстановление архивированных [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="f417c-106">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="f417c-107">Это восстанавливает возможность отправлять сообщения и изменение группы, сотрудничает с параметры клиента и группы.</span><span class="sxs-lookup"><span data-stu-id="f417c-107">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="f417c-108">Команды, архивируются использования [архива](team-archive.md) API.</span><span class="sxs-lookup"><span data-stu-id="f417c-108">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="f417c-109">Unarchiving является асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="f417c-109">Unarchiving is an async operation.</span></span> <span data-ttu-id="f417c-110">Группа архиве после асинхронного успешного завершения операции, которой может произойти после ответа от этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="f417c-110">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="f417c-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f417c-111">Permissions</span></span>
<span data-ttu-id="f417c-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f417c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f417c-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f417c-114">Permission type</span></span>      | <span data-ttu-id="f417c-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f417c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f417c-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f417c-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f417c-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f417c-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f417c-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f417c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f417c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f417c-119">Not supported.</span></span>    |
|<span data-ttu-id="f417c-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f417c-120">Application</span></span> | <span data-ttu-id="f417c-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f417c-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="f417c-122">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="f417c-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f417c-123">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="f417c-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f417c-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f417c-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="f417c-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f417c-125">Request headers</span></span>
| <span data-ttu-id="f417c-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f417c-126">Header</span></span>       | <span data-ttu-id="f417c-127">Значение</span><span class="sxs-lookup"><span data-stu-id="f417c-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f417c-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f417c-128">Authorization</span></span>  | <span data-ttu-id="f417c-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f417c-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f417c-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f417c-131">Request body</span></span>
<span data-ttu-id="f417c-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f417c-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f417c-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="f417c-133">Response</span></span>

<span data-ttu-id="f417c-134">Если unarchiving запускается успешно, этот метод возвращает `202 Accepted` код ответа.</span><span class="sxs-lookup"><span data-stu-id="f417c-134">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="f417c-135">Ответ также будет содержать `Location` заголовок, который содержит расположение [teamsAsyncOperation](../resources/teamsasyncoperation.md) , который был создан для обработки unarchiving рабочей группы.</span><span class="sxs-lookup"><span data-stu-id="f417c-135">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="f417c-136">Проверьте состояние unarchiving операции, внесение запрос GET в этом расположении.</span><span class="sxs-lookup"><span data-stu-id="f417c-136">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="f417c-137">Пример</span><span class="sxs-lookup"><span data-stu-id="f417c-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f417c-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="f417c-138">Request</span></span>
<span data-ttu-id="f417c-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f417c-139">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="f417c-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="f417c-140">Response</span></span>
<span data-ttu-id="f417c-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f417c-141">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
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
  "suppressions": [
    "Error: /api-reference/beta/api/team-unarchive.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
