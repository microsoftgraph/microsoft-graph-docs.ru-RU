---
title: Удаление приложения из группы
description: Удаляет приложение из указанной команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: aa75f72375432609afb748959cb82ff63fa1b721
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057024"
---
# <a name="delete-app-from-team"></a><span data-ttu-id="cc38d-103">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="cc38d-103">Delete app from team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc38d-104">Удаляет [приложение](../resources/teamsappinstallation.md) из указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="cc38d-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

><span data-ttu-id="cc38d-105">**Примечание:** Если вы используете разрешения приложения, произойдет известная ошибка.</span><span class="sxs-lookup"><span data-stu-id="cc38d-105">**Note:** If you're using application permissions, a known issue will occur.</span></span> <span data-ttu-id="cc38d-106">Дополнительные сведения см. в статье [Известные проблемы](graph/concepts/known-issues.md).</span><span class="sxs-lookup"><span data-stu-id="cc38d-106">For details, see [known issues](graph/concepts/known-issues.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cc38d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc38d-107">Permissions</span></span>
<span data-ttu-id="cc38d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc38d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc38d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc38d-110">Permission type</span></span>      | <span data-ttu-id="cc38d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc38d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc38d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc38d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cc38d-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc38d-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc38d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc38d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc38d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc38d-115">Not supported.</span></span>    |
|<span data-ttu-id="cc38d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc38d-116">Application</span></span> | <span data-ttu-id="cc38d-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc38d-117">Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="cc38d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc38d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cc38d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc38d-119">Request headers</span></span>
| <span data-ttu-id="cc38d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc38d-120">Header</span></span>       | <span data-ttu-id="cc38d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cc38d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc38d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc38d-122">Authorization</span></span>  | <span data-ttu-id="cc38d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc38d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc38d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc38d-125">Request body</span></span>
<span data-ttu-id="cc38d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cc38d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc38d-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="cc38d-127">Response</span></span>

<span data-ttu-id="cc38d-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cc38d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc38d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cc38d-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cc38d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc38d-131">Request</span></span>
<span data-ttu-id="cc38d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc38d-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="cc38d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc38d-133">Response</span></span>
<span data-ttu-id="cc38d-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc38d-134">The following is an example of the response.</span></span> <span data-ttu-id="cc38d-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="cc38d-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cc38d-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc38d-136">All of the properties will be returned from an actual call.</span></span>
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
