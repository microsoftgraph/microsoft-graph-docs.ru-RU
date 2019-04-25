---
title: Удаление приложения из группы
description: Удаляет приложение из указанной команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 592f488ad73337cc89b92d5a57bd874664fba9cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536757"
---
# <a name="delete-app-from-team"></a><span data-ttu-id="4644c-103">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="4644c-103">Delete app from team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4644c-104">Удаляет [приложение](../resources/teamsappinstallation.md) из указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="4644c-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4644c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4644c-105">Permissions</span></span>
<span data-ttu-id="4644c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4644c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4644c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4644c-108">Permission type</span></span>      | <span data-ttu-id="4644c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4644c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4644c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4644c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4644c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4644c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4644c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4644c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4644c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4644c-113">Not supported.</span></span>    |
|<span data-ttu-id="4644c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4644c-114">Application</span></span> | <span data-ttu-id="4644c-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4644c-115">Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4644c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4644c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4644c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4644c-117">Request headers</span></span>
| <span data-ttu-id="4644c-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4644c-118">Header</span></span>       | <span data-ttu-id="4644c-119">Значение</span><span class="sxs-lookup"><span data-stu-id="4644c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4644c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4644c-120">Authorization</span></span>  | <span data-ttu-id="4644c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4644c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4644c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4644c-123">Request body</span></span>
<span data-ttu-id="4644c-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4644c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4644c-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="4644c-125">Response</span></span>

<span data-ttu-id="4644c-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4644c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4644c-128">Пример</span><span class="sxs-lookup"><span data-stu-id="4644c-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4644c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="4644c-129">Request</span></span>
<span data-ttu-id="4644c-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4644c-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="4644c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4644c-131">Response</span></span>
<span data-ttu-id="4644c-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4644c-132">The following is an example of the response.</span></span> <span data-ttu-id="4644c-133">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="4644c-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4644c-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4644c-134">All of the properties will be returned from an actual call.</span></span>
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
