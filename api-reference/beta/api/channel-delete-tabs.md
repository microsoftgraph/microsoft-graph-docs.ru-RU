---
title: Удаление вкладки из канала
description: 'Удаляет (открепит) вкладку из указанного канала в команде. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5afc43cd071a66c4e6312456e6ed40f674305ab1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047555"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="bcb3c-103">Удаление вкладки из канала</span><span class="sxs-lookup"><span data-stu-id="bcb3c-103">Delete tab from channel</span></span>

<span data-ttu-id="bcb3c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcb3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcb3c-105">Удаляет (открепит) вкладку из указанного [канала](../resources/channel.md) в [команде.](../resources/team.md)</span><span class="sxs-lookup"><span data-stu-id="bcb3c-105">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="bcb3c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bcb3c-106">Permissions</span></span>
<span data-ttu-id="bcb3c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcb3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcb3c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcb3c-109">Permission type</span></span>      | <span data-ttu-id="bcb3c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcb3c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcb3c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcb3c-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="bcb3c-112">TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcb3c-112">TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="bcb3c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcb3c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcb3c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcb3c-114">Not supported.</span></span>    |
|<span data-ttu-id="bcb3c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="bcb3c-115">Application</span></span> | <span data-ttu-id="bcb3c-116">TeamsTab.Delete.Group\*, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcb3c-116">TeamsTab.Delete.Group\*, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="bcb3c-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="bcb3c-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="bcb3c-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="bcb3c-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="bcb3c-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="bcb3c-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="bcb3c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcb3c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{team-id}/channels/{channel-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="bcb3c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcb3c-121">Request headers</span></span>
| <span data-ttu-id="bcb3c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bcb3c-122">Header</span></span>       | <span data-ttu-id="bcb3c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="bcb3c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bcb3c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bcb3c-124">Authorization</span></span>  | <span data-ttu-id="bcb3c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcb3c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bcb3c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bcb3c-127">Request body</span></span>
<span data-ttu-id="bcb3c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bcb3c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcb3c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcb3c-129">Response</span></span>

<span data-ttu-id="bcb3c-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bcb3c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcb3c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="bcb3c-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bcb3c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcb3c-133">Request</span></span>
<span data-ttu-id="bcb3c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcb3c-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="bcb3c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcb3c-135">Response</span></span>
<span data-ttu-id="bcb3c-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bcb3c-136">The following is an example of the response.</span></span> <span data-ttu-id="bcb3c-137">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bcb3c-137">Note: The response object shown here might be shortened for readability.</span></span>
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete tab from channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


