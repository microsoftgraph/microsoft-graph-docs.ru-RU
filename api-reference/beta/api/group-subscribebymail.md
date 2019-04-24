---
title: 'group: subscribeByMail'
description: С помощью этого метода можно разрешить текущему пользователю получать уведомления электронной почты о новых записях, событиях и файлов в этой группе. Поддерживается только для групп Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 0a334daa005947099da324aab31ccc2a1da6b6e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32501964"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="a397b-104">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="a397b-104">group: subscribeByMail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a397b-105">С помощью этого метода можно разрешить текущему пользователю получать уведомления электронной почты о новых записях, событиях и файлов в этой группе.</span><span class="sxs-lookup"><span data-stu-id="a397b-105">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="a397b-106">Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="a397b-106">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="a397b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a397b-107">Permissions</span></span>
<span data-ttu-id="a397b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a397b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a397b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a397b-110">Permission type</span></span>      | <span data-ttu-id="a397b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a397b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a397b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a397b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a397b-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a397b-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a397b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a397b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a397b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a397b-115">Not supported.</span></span>    |
|<span data-ttu-id="a397b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a397b-116">Application</span></span> | <span data-ttu-id="a397b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a397b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a397b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a397b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="a397b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a397b-119">Request headers</span></span>
| <span data-ttu-id="a397b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a397b-120">Header</span></span>       | <span data-ttu-id="a397b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a397b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a397b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a397b-122">Authorization</span></span>  | <span data-ttu-id="a397b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a397b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a397b-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="a397b-125">Prefer</span></span> | <span data-ttu-id="a397b-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="a397b-126">return=minimal.</span></span> <span data-ttu-id="a397b-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a397b-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="a397b-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a397b-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="a397b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a397b-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a397b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a397b-130">Response</span></span>
<span data-ttu-id="a397b-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a397b-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a397b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a397b-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a397b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a397b-134">Request</span></span>
<span data-ttu-id="a397b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a397b-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/subscribeByMail
```

#### <a name="response"></a><span data-ttu-id="a397b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a397b-136">Response</span></span>
<span data-ttu-id="a397b-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a397b-137">The following is an example of the response.</span></span> 
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
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-subscribebymail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
