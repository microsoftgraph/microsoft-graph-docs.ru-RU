---
title: Удаление вкладки из канала
description: 'Удаляет (открепляет) вкладку из указанного канала в команде. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a5cb2334c250c63d0644c8fab3f97d35c481a515
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521779"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="2d784-103">Удаление вкладки из канала</span><span class="sxs-lookup"><span data-stu-id="2d784-103">Delete tab from channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d784-104">Удаляет (открепляет) вкладку из указанного [канала](../resources/channel.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="2d784-104">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="2d784-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d784-105">Permissions</span></span>
<span data-ttu-id="2d784-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d784-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d784-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d784-108">Permission type</span></span>      | <span data-ttu-id="2d784-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d784-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d784-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d784-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2d784-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d784-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2d784-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d784-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d784-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d784-113">Not supported.</span></span>    |
|<span data-ttu-id="2d784-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d784-114">Application</span></span> | <span data-ttu-id="2d784-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d784-115">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="2d784-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="2d784-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2d784-117">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="2d784-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2d784-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d784-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2d784-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d784-119">Request headers</span></span>
| <span data-ttu-id="2d784-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2d784-120">Header</span></span>       | <span data-ttu-id="2d784-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2d784-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2d784-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d784-122">Authorization</span></span>  | <span data-ttu-id="2d784-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d784-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2d784-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d784-125">Request body</span></span>
<span data-ttu-id="2d784-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2d784-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d784-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d784-127">Response</span></span>

<span data-ttu-id="2d784-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2d784-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d784-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2d784-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2d784-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d784-131">Request</span></span>
<span data-ttu-id="2d784-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d784-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="2d784-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d784-133">Response</span></span>
<span data-ttu-id="2d784-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2d784-134">The following is an example of the response.</span></span> <span data-ttu-id="2d784-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="2d784-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2d784-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d784-136">All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/teamstab-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
