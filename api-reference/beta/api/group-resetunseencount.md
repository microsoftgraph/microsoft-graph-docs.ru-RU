---
title: 'group: resetUnseenCount'
description: Сброс свойства unseenCount всех записей, которые пользователь не просматривал со своего предыдущего посещения. Поддерживается только для групп Office 365.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: aa37261a536437d0e82195ecfaae06de9e1c6a3a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502010"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="ec67c-104">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="ec67c-104">group: resetUnseenCount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec67c-105">Сброс свойства unseenCount всех записей, которые пользователь не просматривал со своего предыдущего посещения.</span><span class="sxs-lookup"><span data-stu-id="ec67c-105">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="ec67c-106">Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="ec67c-106">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec67c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec67c-107">Permissions</span></span>
<span data-ttu-id="ec67c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec67c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec67c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec67c-110">Permission type</span></span>      | <span data-ttu-id="ec67c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec67c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec67c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec67c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ec67c-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec67c-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ec67c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec67c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec67c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec67c-115">Not supported.</span></span>    |
|<span data-ttu-id="ec67c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec67c-116">Application</span></span> | <span data-ttu-id="ec67c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec67c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec67c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec67c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="ec67c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec67c-119">Request headers</span></span>
| <span data-ttu-id="ec67c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ec67c-120">Header</span></span>       | <span data-ttu-id="ec67c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ec67c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ec67c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec67c-122">Authorization</span></span>  | <span data-ttu-id="ec67c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec67c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ec67c-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="ec67c-125">Prefer</span></span> | <span data-ttu-id="ec67c-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="ec67c-126">return=minimal.</span></span> <span data-ttu-id="ec67c-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ec67c-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="ec67c-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ec67c-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="ec67c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec67c-129">Request body</span></span>
<span data-ttu-id="ec67c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec67c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec67c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec67c-131">Response</span></span>
<span data-ttu-id="ec67c-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ec67c-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec67c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ec67c-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ec67c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec67c-135">Request</span></span>
<span data-ttu-id="ec67c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec67c-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/resetUnseenCount
```

#### <a name="response"></a><span data-ttu-id="ec67c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec67c-137">Response</span></span>
<span data-ttu-id="ec67c-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ec67c-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-resetunseencount.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
