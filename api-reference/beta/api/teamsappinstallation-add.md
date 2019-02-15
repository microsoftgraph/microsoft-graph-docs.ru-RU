---
title: Добавление приложения в команду
description: Устанавливает приложение в указанную группу.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 35d2521d9bff37ea45f7496a825429762daaf8f7
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2019
ms.locfileid: "30056996"
---
# <a name="add-app-to-team"></a><span data-ttu-id="c4b0c-103">Добавление приложения в команду</span><span class="sxs-lookup"><span data-stu-id="c4b0c-103">Add app to team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4b0c-104">Устанавливает [приложение](../resources/teamsapp.md) в указанную [группу](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="c4b0c-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

><span data-ttu-id="c4b0c-105">**Примечание:** Если вы используете разрешения приложения, произойдет известная ошибка.</span><span class="sxs-lookup"><span data-stu-id="c4b0c-105">**Note:** If you're using application permissions, a known issue will occur.</span></span> <span data-ttu-id="c4b0c-106">Дополнительные сведения см. в статье [Известные проблемы](graph/concepts/known-issues.md).</span><span class="sxs-lookup"><span data-stu-id="c4b0c-106">For details, see [known issues](graph/concepts/known-issues.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4b0c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4b0c-107">Permissions</span></span>
<span data-ttu-id="c4b0c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4b0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4b0c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4b0c-110">Permission type</span></span>      | <span data-ttu-id="c4b0c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4b0c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4b0c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4b0c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c4b0c-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4b0c-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c4b0c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4b0c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4b0c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4b0c-115">Not supported.</span></span>    |
|<span data-ttu-id="c4b0c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4b0c-116">Application</span></span> | <span data-ttu-id="c4b0c-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4b0c-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4b0c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4b0c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="c4b0c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4b0c-119">Request headers</span></span>
| <span data-ttu-id="c4b0c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4b0c-120">Header</span></span>       | <span data-ttu-id="c4b0c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c4b0c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c4b0c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4b0c-122">Authorization</span></span>  | <span data-ttu-id="c4b0c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4b0c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c4b0c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4b0c-125">Request body</span></span>

| <span data-ttu-id="c4b0c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4b0c-126">Property</span></span>     | <span data-ttu-id="c4b0c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c4b0c-127">Type</span></span>   |<span data-ttu-id="c4b0c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c4b0c-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4b0c-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c4b0c-129">teamsApp</span></span>|<span data-ttu-id="c4b0c-130">String</span><span class="sxs-lookup"><span data-stu-id="c4b0c-130">String</span></span>|<span data-ttu-id="c4b0c-131">Идентификатор добавляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="c4b0c-131">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="c4b0c-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4b0c-132">Response</span></span>

<span data-ttu-id="c4b0c-133">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="c4b0c-133">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="c4b0c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="c4b0c-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c4b0c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4b0c-135">Request</span></span>
<span data-ttu-id="c4b0c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4b0c-136">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="c4b0c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4b0c-137">Response</span></span>
<span data-ttu-id="c4b0c-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c4b0c-138">The following is an example of the response.</span></span> <span data-ttu-id="c4b0c-139">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c4b0c-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c4b0c-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4b0c-140">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="c4b0c-141">См. также</span><span class="sxs-lookup"><span data-stu-id="c4b0c-141">See also</span></span>

