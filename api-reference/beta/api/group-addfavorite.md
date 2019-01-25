---
title: 'group: addFavorite'
description: Добавление группы в список избранных групп текущего пользователя. Поддерживается только для групп Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 09bebe58349e4d040fb185c59d5158e9e39ec832
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512887"
---
# <a name="group-addfavorite"></a><span data-ttu-id="22252-104">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="22252-104">group: addFavorite</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22252-p102">Добавление группы в список избранных групп текущего пользователя. Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="22252-p102">Add the group to the list of the current user's favorite groups. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="22252-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22252-107">Permissions</span></span>
<span data-ttu-id="22252-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22252-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22252-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22252-110">Permission type</span></span>      | <span data-ttu-id="22252-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22252-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22252-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22252-112">Delegated (work or school account)</span></span> | <span data-ttu-id="22252-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22252-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="22252-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22252-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22252-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22252-115">Not supported.</span></span>    |
|<span data-ttu-id="22252-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22252-116">Application</span></span> | <span data-ttu-id="22252-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22252-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22252-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22252-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```

## <a name="request-headers"></a><span data-ttu-id="22252-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22252-119">Request headers</span></span>
| <span data-ttu-id="22252-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22252-120">Header</span></span>       | <span data-ttu-id="22252-121">Значение</span><span class="sxs-lookup"><span data-stu-id="22252-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="22252-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22252-122">Authorization</span></span>  | <span data-ttu-id="22252-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22252-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="22252-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="22252-125">Prefer</span></span> | <span data-ttu-id="22252-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="22252-126">return=minimal.</span></span> <span data-ttu-id="22252-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="22252-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="22252-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="22252-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="22252-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="22252-129">Request body</span></span>
<span data-ttu-id="22252-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22252-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22252-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="22252-131">Response</span></span>
<span data-ttu-id="22252-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="22252-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22252-134">Пример</span><span class="sxs-lookup"><span data-stu-id="22252-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="22252-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="22252-135">Request</span></span>
<span data-ttu-id="22252-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22252-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/addFavorite
```

#### <a name="response"></a><span data-ttu-id="22252-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="22252-137">Response</span></span>
<span data-ttu-id="22252-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22252-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: addFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-addfavorite.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
