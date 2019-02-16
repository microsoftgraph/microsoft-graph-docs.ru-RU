---
title: Добавление приложения в команду
description: Устанавливает приложение в указанную группу.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 261d186e23b516e58a428ecfdd2883f7a3bc111d
ms.sourcegitcommit: 4e9acb8029aca36dfade509a25f1111e1bd0ec6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/16/2019
ms.locfileid: "30070829"
---
# <a name="add-app-to-team"></a><span data-ttu-id="cc7fe-103">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="cc7fe-103">Add app to team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc7fe-104">Устанавливает [приложение](../resources/teamsapp.md) в указанную [группу](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="cc7fe-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

><span data-ttu-id="cc7fe-105">**Примечание:** Если вы используете разрешения приложения, произойдет известная ошибка.</span><span class="sxs-lookup"><span data-stu-id="cc7fe-105">**Note:** If you're using application permissions, a known issue will occur.</span></span> <span data-ttu-id="cc7fe-106">Дополнительные сведения см. в статье [Известные проблемы](/graph/known-issues).</span><span class="sxs-lookup"><span data-stu-id="cc7fe-106">For details, see [known issues](/graph/known-issues).</span></span>

## <a name="permissions"></a><span data-ttu-id="cc7fe-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc7fe-107">Permissions</span></span>
<span data-ttu-id="cc7fe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc7fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc7fe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc7fe-110">Permission type</span></span>      | <span data-ttu-id="cc7fe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc7fe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc7fe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc7fe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cc7fe-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc7fe-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc7fe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc7fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc7fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc7fe-115">Not supported.</span></span>    |
|<span data-ttu-id="cc7fe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc7fe-116">Application</span></span> | <span data-ttu-id="cc7fe-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc7fe-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc7fe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc7fe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="cc7fe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc7fe-119">Request headers</span></span>
| <span data-ttu-id="cc7fe-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc7fe-120">Header</span></span>       | <span data-ttu-id="cc7fe-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cc7fe-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc7fe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc7fe-122">Authorization</span></span>  | <span data-ttu-id="cc7fe-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc7fe-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc7fe-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc7fe-125">Request body</span></span>

| <span data-ttu-id="cc7fe-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc7fe-126">Property</span></span>     | <span data-ttu-id="cc7fe-127">Тип</span><span class="sxs-lookup"><span data-stu-id="cc7fe-127">Type</span></span>   |<span data-ttu-id="cc7fe-128">Описание</span><span class="sxs-lookup"><span data-stu-id="cc7fe-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc7fe-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cc7fe-129">teamsApp</span></span>|<span data-ttu-id="cc7fe-130">String</span><span class="sxs-lookup"><span data-stu-id="cc7fe-130">String</span></span>|<span data-ttu-id="cc7fe-131">Идентификатор добавляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="cc7fe-131">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="cc7fe-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="cc7fe-132">Response</span></span>

<span data-ttu-id="cc7fe-133">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="cc7fe-133">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="cc7fe-134">Пример</span><span class="sxs-lookup"><span data-stu-id="cc7fe-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cc7fe-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc7fe-135">Request</span></span>
<span data-ttu-id="cc7fe-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc7fe-136">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="cc7fe-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc7fe-137">Response</span></span>
<span data-ttu-id="cc7fe-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc7fe-138">The following is an example of the response.</span></span> <span data-ttu-id="cc7fe-139">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="cc7fe-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cc7fe-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc7fe-140">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsappinstallation-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="cc7fe-141">См. также</span><span class="sxs-lookup"><span data-stu-id="cc7fe-141">See also</span></span>

