---
title: Удаление канала
description: Удаление канала.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 734df0a79881993f4e002562e5125305b624c4c7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525334"
---
# <a name="delete-channel"></a><span data-ttu-id="f146f-103">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="f146f-103">Delete channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f146f-104">Удаление [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="f146f-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="f146f-105">**Примечание**: существует известная проблема с разрешениями приложения и этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="f146f-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="f146f-106">Дополнительные сведения см [Известные проблемы списка](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="f146f-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="f146f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f146f-107">Permissions</span></span>
<span data-ttu-id="f146f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f146f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f146f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f146f-110">Permission type</span></span>      | <span data-ttu-id="f146f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f146f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f146f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f146f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f146f-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f146f-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f146f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f146f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f146f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f146f-115">Not supported.</span></span>    |
|<span data-ttu-id="f146f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f146f-116">Application</span></span> | <span data-ttu-id="f146f-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f146f-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="f146f-118">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="f146f-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f146f-119">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="f146f-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f146f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f146f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f146f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f146f-121">Request headers</span></span>
| <span data-ttu-id="f146f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f146f-122">Header</span></span>       | <span data-ttu-id="f146f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f146f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f146f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f146f-124">Authorization</span></span>  | <span data-ttu-id="f146f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f146f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f146f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f146f-127">Request body</span></span>
<span data-ttu-id="f146f-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f146f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f146f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f146f-129">Response</span></span>

<span data-ttu-id="f146f-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f146f-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f146f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f146f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f146f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f146f-133">Request</span></span>
<span data-ttu-id="f146f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f146f-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="f146f-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="f146f-135">Response</span></span>

<span data-ttu-id="f146f-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f146f-136">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
