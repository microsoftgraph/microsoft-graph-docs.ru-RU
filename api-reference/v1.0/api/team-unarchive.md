---
title: Распаковка объекта команды
description: Восстановление архивной команды. Это восстанавливает возможность пользователей отправлять сообщения и редактировать команду, абидинг по клиенту и параметрам группы. Архивация Teams выполняется с помощью API архива.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 77cd2decf1250d6d189aba20df1db172475ab806
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576425"
---
# <a name="unarchive-team"></a><span data-ttu-id="23116-105">Распаковка объекта команды</span><span class="sxs-lookup"><span data-stu-id="23116-105">Unarchive team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23116-106">Восстановление архивной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="23116-106">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="23116-107">Это восстанавливает возможность пользователей отправлять сообщения и редактировать команду, абидинг по клиенту и параметрам группы.</span><span class="sxs-lookup"><span data-stu-id="23116-107">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="23116-108">Архивация Teams выполняется с помощью API [архива](team-archive.md) .</span><span class="sxs-lookup"><span data-stu-id="23116-108">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="23116-109">Unarchivingя это асинхронная операция.</span><span class="sxs-lookup"><span data-stu-id="23116-109">Unarchiving is an async operation.</span></span> <span data-ttu-id="23116-110">Команда не архивируется после успешного завершения асинхронной операции, которая может произойти после ответа от этого API.</span><span class="sxs-lookup"><span data-stu-id="23116-110">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="23116-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23116-111">Permissions</span></span>
<span data-ttu-id="23116-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23116-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23116-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23116-114">Permission type</span></span>      | <span data-ttu-id="23116-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23116-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23116-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23116-116">Delegated (work or school account)</span></span> | <span data-ttu-id="23116-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23116-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="23116-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23116-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23116-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23116-119">Not supported.</span></span>    |
|<span data-ttu-id="23116-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23116-120">Application</span></span> | <span data-ttu-id="23116-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23116-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="23116-122">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="23116-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="23116-123">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="23116-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="23116-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23116-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="23116-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23116-125">Request headers</span></span>
| <span data-ttu-id="23116-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23116-126">Header</span></span>       | <span data-ttu-id="23116-127">Значение</span><span class="sxs-lookup"><span data-stu-id="23116-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="23116-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23116-128">Authorization</span></span>  | <span data-ttu-id="23116-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23116-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="23116-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23116-131">Request body</span></span>
<span data-ttu-id="23116-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23116-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23116-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="23116-133">Response</span></span>

<span data-ttu-id="23116-134">В случае успешного запуска unarchivingи этот метод возвращает код `202 Accepted` отклика.</span><span class="sxs-lookup"><span data-stu-id="23116-134">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="23116-135">Ответ также будет содержать `Location` заголовок, который содержит расположение [теамсасинкоператион](../resources/teamsasyncoperation.md) , созданного для обработки отмененного архивирования команды.</span><span class="sxs-lookup"><span data-stu-id="23116-135">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="23116-136">Проверьте состояние операции расархивации, выполнив запрос GET к этому расположению.</span><span class="sxs-lookup"><span data-stu-id="23116-136">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="23116-137">Пример</span><span class="sxs-lookup"><span data-stu-id="23116-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="23116-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="23116-138">Request</span></span>
<span data-ttu-id="23116-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23116-139">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="23116-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="23116-140">Response</span></span>
<span data-ttu-id="23116-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23116-141">The following is an example of a response.</span></span>
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
