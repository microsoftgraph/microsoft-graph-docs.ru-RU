---
title: Обновление приложения в группе
description: Обновляет установку приложения в группе
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 30398a21d1ba1d8d37932bf0933e454600f019b2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514679"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="82afe-103">Обновление приложения в группе</span><span class="sxs-lookup"><span data-stu-id="82afe-103">Upgrade an app in a team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82afe-104">Обновляет [установки приложения](../resources/teamsappinstallation.md) в [группы](../resources/team.md) до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="82afe-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="82afe-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82afe-105">Permissions</span></span>

<span data-ttu-id="82afe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82afe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82afe-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82afe-108">Permission type</span></span>      | <span data-ttu-id="82afe-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82afe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82afe-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82afe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="82afe-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82afe-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="82afe-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82afe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82afe-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82afe-113">Not supported.</span></span>    |
|<span data-ttu-id="82afe-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82afe-114">Application</span></span> | <span data-ttu-id="82afe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82afe-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82afe-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82afe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="82afe-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82afe-117">Request headers</span></span>
| <span data-ttu-id="82afe-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82afe-118">Header</span></span>       | <span data-ttu-id="82afe-119">Значение</span><span class="sxs-lookup"><span data-stu-id="82afe-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="82afe-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82afe-120">Authorization</span></span>  | <span data-ttu-id="82afe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82afe-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="82afe-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82afe-123">Request body</span></span>
<span data-ttu-id="82afe-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82afe-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82afe-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="82afe-125">Response</span></span>

<span data-ttu-id="82afe-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="82afe-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82afe-128">Пример</span><span class="sxs-lookup"><span data-stu-id="82afe-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="82afe-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="82afe-129">Request</span></span>
<span data-ttu-id="82afe-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82afe-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="82afe-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="82afe-131">Response</span></span>
<span data-ttu-id="82afe-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="82afe-132">The following is an example of the response.</span></span> 

><span data-ttu-id="82afe-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82afe-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
