---
title: Удаление элемента роли каталога
description: Удаление элемента из объекта directoryRole.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c45436660ed84476efd293095efb185757c01249
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526293"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="f56d6-103">Удаление элемента роли каталога</span><span class="sxs-lookup"><span data-stu-id="f56d6-103">Remove directory role member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f56d6-104">Удаление элемента из объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="f56d6-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="f56d6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f56d6-105">Permissions</span></span>

<span data-ttu-id="f56d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f56d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f56d6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f56d6-108">Permission type</span></span>      | <span data-ttu-id="f56d6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f56d6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f56d6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f56d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f56d6-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f56d6-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f56d6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f56d6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f56d6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f56d6-113">Not supported.</span></span>    |
|<span data-ttu-id="f56d6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f56d6-114">Application</span></span> | <span data-ttu-id="f56d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f56d6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f56d6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f56d6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f56d6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f56d6-117">Request headers</span></span>

| <span data-ttu-id="f56d6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f56d6-118">Name</span></span>       | <span data-ttu-id="f56d6-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f56d6-119">Type</span></span> | <span data-ttu-id="f56d6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f56d6-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f56d6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f56d6-121">Authorization</span></span>  | <span data-ttu-id="f56d6-122">string</span><span class="sxs-lookup"><span data-stu-id="f56d6-122">string</span></span>  | <span data-ttu-id="f56d6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f56d6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f56d6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f56d6-125">Request body</span></span>

<span data-ttu-id="f56d6-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f56d6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f56d6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f56d6-127">Response</span></span>

<span data-ttu-id="f56d6-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f56d6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f56d6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f56d6-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f56d6-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f56d6-131">Request</span></span>

<span data-ttu-id="f56d6-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f56d6-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="f56d6-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="f56d6-133">Response</span></span>

<span data-ttu-id="f56d6-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f56d6-134">Here is an example of the response.</span></span> 
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-delete-member.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
