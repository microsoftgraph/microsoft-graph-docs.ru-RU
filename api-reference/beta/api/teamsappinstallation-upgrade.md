---
title: Обновление приложения в команде
description: Обновление установки приложения в команде
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0ab151203e3b2ec3ee863bae34a8feed0c6d1064
ms.sourcegitcommit: 4e9acb8029aca36dfade509a25f1111e1bd0ec6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/16/2019
ms.locfileid: "30070808"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="d0766-103">Обновление приложения в команде</span><span class="sxs-lookup"><span data-stu-id="d0766-103">Upgrade an app in a team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0766-104">Обновляет [установку приложения](../resources/teamsappinstallation.md) в [команде](../resources/team.md) до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="d0766-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

><span data-ttu-id="d0766-105">**Примечание:** Если вы используете разрешения приложения, произойдет известная ошибка.</span><span class="sxs-lookup"><span data-stu-id="d0766-105">**Note:** If you're using application permissions, a known issue will occur.</span></span> <span data-ttu-id="d0766-106">Дополнительные сведения см. в статье [Известные проблемы](/graph/known-issues).</span><span class="sxs-lookup"><span data-stu-id="d0766-106">For details, see [known issues](/graph/known-issues).</span></span>

## <a name="permissions"></a><span data-ttu-id="d0766-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0766-107">Permissions</span></span>

<span data-ttu-id="d0766-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0766-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0766-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0766-110">Permission type</span></span>      | <span data-ttu-id="d0766-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0766-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0766-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0766-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d0766-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0766-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0766-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0766-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0766-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0766-115">Not supported.</span></span>    |
|<span data-ttu-id="d0766-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0766-116">Application</span></span> | <span data-ttu-id="d0766-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0766-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0766-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0766-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="d0766-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0766-119">Request headers</span></span>
| <span data-ttu-id="d0766-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0766-120">Header</span></span>       | <span data-ttu-id="d0766-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d0766-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d0766-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0766-122">Authorization</span></span>  | <span data-ttu-id="d0766-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0766-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d0766-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0766-125">Request body</span></span>
<span data-ttu-id="d0766-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d0766-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0766-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0766-127">Response</span></span>

<span data-ttu-id="d0766-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d0766-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0766-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d0766-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d0766-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0766-131">Request</span></span>
<span data-ttu-id="d0766-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0766-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="d0766-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0766-133">Response</span></span>
<span data-ttu-id="d0766-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d0766-134">The following is an example of the response.</span></span> 

><span data-ttu-id="d0766-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0766-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/teamsappinstallation-upgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
