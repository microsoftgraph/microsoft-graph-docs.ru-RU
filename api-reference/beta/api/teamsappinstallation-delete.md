---
title: Удаление приложения из группы
description: Удаляет приложение из указанной команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a4857a5e56a16eb9ee0989108fcfe3b185bb5f0c
ms.sourcegitcommit: 4e9acb8029aca36dfade509a25f1111e1bd0ec6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/16/2019
ms.locfileid: "30070822"
---
# <a name="delete-app-from-team"></a><span data-ttu-id="febe3-103">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="febe3-103">Delete app from team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="febe3-104">Удаляет [приложение](../resources/teamsappinstallation.md) из указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="febe3-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

><span data-ttu-id="febe3-105">**Примечание:** Если вы используете разрешения приложения, произойдет известная ошибка.</span><span class="sxs-lookup"><span data-stu-id="febe3-105">**Note:** If you're using application permissions, a known issue will occur.</span></span> <span data-ttu-id="febe3-106">Дополнительные сведения см. в статье [Известные проблемы](/graph/known-issues).</span><span class="sxs-lookup"><span data-stu-id="febe3-106">For details, see [known issues](/graph/known-issues).</span></span>

## <a name="permissions"></a><span data-ttu-id="febe3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="febe3-107">Permissions</span></span>
<span data-ttu-id="febe3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="febe3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="febe3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="febe3-110">Permission type</span></span>      | <span data-ttu-id="febe3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="febe3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="febe3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="febe3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="febe3-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="febe3-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="febe3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="febe3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="febe3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="febe3-115">Not supported.</span></span>    |
|<span data-ttu-id="febe3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="febe3-116">Application</span></span> | <span data-ttu-id="febe3-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="febe3-117">Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="febe3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="febe3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="febe3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="febe3-119">Request headers</span></span>
| <span data-ttu-id="febe3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="febe3-120">Header</span></span>       | <span data-ttu-id="febe3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="febe3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="febe3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="febe3-122">Authorization</span></span>  | <span data-ttu-id="febe3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="febe3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="febe3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="febe3-125">Request body</span></span>
<span data-ttu-id="febe3-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="febe3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="febe3-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="febe3-127">Response</span></span>

<span data-ttu-id="febe3-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="febe3-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="febe3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="febe3-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="febe3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="febe3-131">Request</span></span>
<span data-ttu-id="febe3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="febe3-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="febe3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="febe3-133">Response</span></span>
<span data-ttu-id="febe3-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="febe3-134">The following is an example of the response.</span></span> <span data-ttu-id="febe3-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="febe3-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="febe3-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="febe3-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
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
    "Error: /api-reference/beta/api/teamsappinstallation-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
