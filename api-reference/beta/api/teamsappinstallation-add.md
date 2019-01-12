---
title: Добавление приложения в группу
description: Пакет приложения для указанной группы.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3f52d54850d1046d837821de1501968965678e8b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990273"
---
# <a name="add-app-to-team"></a><span data-ttu-id="d5fd6-103">Добавление приложения в группу</span><span class="sxs-lookup"><span data-stu-id="d5fd6-103">Add app to team</span></span>

> <span data-ttu-id="d5fd6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d5fd6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5fd6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5fd6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d5fd6-106">Пакет [приложения](../resources/teamsapp.md) для указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="d5fd6-106">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5fd6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5fd6-107">Permissions</span></span>
<span data-ttu-id="d5fd6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5fd6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5fd6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5fd6-110">Permission type</span></span>      | <span data-ttu-id="d5fd6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5fd6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5fd6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5fd6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d5fd6-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5fd6-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d5fd6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5fd6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5fd6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5fd6-115">Not supported.</span></span>    |
|<span data-ttu-id="d5fd6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5fd6-116">Application</span></span> | <span data-ttu-id="d5fd6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5fd6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5fd6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5fd6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="d5fd6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5fd6-119">Request headers</span></span>
| <span data-ttu-id="d5fd6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5fd6-120">Header</span></span>       | <span data-ttu-id="d5fd6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d5fd6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d5fd6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5fd6-122">Authorization</span></span>  | <span data-ttu-id="d5fd6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5fd6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d5fd6-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d5fd6-125">Request body</span></span>

| <span data-ttu-id="d5fd6-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5fd6-126">Property</span></span>     | <span data-ttu-id="d5fd6-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d5fd6-127">Type</span></span>   |<span data-ttu-id="d5fd6-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d5fd6-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5fd6-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d5fd6-129">teamsApp</span></span>|<span data-ttu-id="d5fd6-130">String</span><span class="sxs-lookup"><span data-stu-id="d5fd6-130">String</span></span>|<span data-ttu-id="d5fd6-131">Идентификатор приложения для добавления.</span><span class="sxs-lookup"><span data-stu-id="d5fd6-131">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="d5fd6-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5fd6-132">Response</span></span>

<span data-ttu-id="d5fd6-133">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="d5fd6-133">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="d5fd6-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d5fd6-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d5fd6-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5fd6-135">Request</span></span>
<span data-ttu-id="d5fd6-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5fd6-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="d5fd6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5fd6-137">Response</span></span>
<span data-ttu-id="d5fd6-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d5fd6-138">The following is an example of the response.</span></span> <span data-ttu-id="d5fd6-139">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="d5fd6-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d5fd6-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5fd6-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="d5fd6-141">См. также</span><span class="sxs-lookup"><span data-stu-id="d5fd6-141">See also</span></span>

