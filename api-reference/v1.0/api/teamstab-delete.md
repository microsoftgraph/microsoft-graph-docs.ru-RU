---
title: Удаление вкладки из канала
description: 'Удаляет (открепляет) вкладку из указанного канала в команде. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a927ce5300f9e5b983bb9b0027f4a1ffcc305d13
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44287705"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="3324b-103">Удаление вкладки из канала</span><span class="sxs-lookup"><span data-stu-id="3324b-103">Delete tab from channel</span></span>

<span data-ttu-id="3324b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3324b-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="3324b-105">Удаляет (открепляет) вкладку из указанного [канала](../resources/channel.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="3324b-105">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="3324b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3324b-106">Permissions</span></span>
<span data-ttu-id="3324b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3324b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3324b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3324b-109">Permission type</span></span>      | <span data-ttu-id="3324b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3324b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3324b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3324b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3324b-112">TeamsTab. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3324b-112">TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="3324b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3324b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3324b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3324b-114">Not supported.</span></span>    |
|<span data-ttu-id="3324b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3324b-115">Application</span></span> | <span data-ttu-id="3324b-116">TeamsTab. Delete. Group ([RSC](https://aka.ms/teams-rsc)), TeamsTab. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3324b-116">TeamsTab.Delete.Group ([RSC](https://aka.ms/teams-rsc)), TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="3324b-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="3324b-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3324b-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="3324b-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3324b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3324b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3324b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3324b-120">Request headers</span></span>
| <span data-ttu-id="3324b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3324b-121">Header</span></span>       | <span data-ttu-id="3324b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3324b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3324b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3324b-123">Authorization</span></span>  | <span data-ttu-id="3324b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3324b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3324b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3324b-126">Request body</span></span>
<span data-ttu-id="3324b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3324b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3324b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3324b-128">Response</span></span>

<span data-ttu-id="3324b-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3324b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3324b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3324b-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3324b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3324b-132">Request</span></span>
<span data-ttu-id="3324b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3324b-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="3324b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3324b-134">Response</span></span>
<span data-ttu-id="3324b-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3324b-135">The following is an example of the response.</span></span> <span data-ttu-id="3324b-136">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="3324b-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3324b-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3324b-137">All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}
-->
