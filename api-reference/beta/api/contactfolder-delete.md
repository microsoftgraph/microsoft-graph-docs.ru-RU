---
title: Удаление объекта contactFolder
description: Удаление любого объекта contactFolder, кроме объекта contactFolder по умолчанию.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 01b8303723c4a59b8fdc4ac3f5d7d4f6cb491fd1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523920"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="d4a9c-103">Удаление объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="d4a9c-103">Delete contactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4a9c-104">Удаление любого объекта contactFolder, кроме объекта contactFolder по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d4a9c-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="d4a9c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4a9c-105">Permissions</span></span>
<span data-ttu-id="d4a9c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4a9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4a9c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4a9c-108">Permission type</span></span>      | <span data-ttu-id="d4a9c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4a9c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4a9c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4a9c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d4a9c-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4a9c-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d4a9c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4a9c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4a9c-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4a9c-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d4a9c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4a9c-114">Application</span></span> | <span data-ttu-id="d4a9c-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4a9c-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4a9c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4a9c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d4a9c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4a9c-117">Request headers</span></span>
| <span data-ttu-id="d4a9c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d4a9c-118">Name</span></span>       | <span data-ttu-id="d4a9c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="d4a9c-119">Type</span></span> | <span data-ttu-id="d4a9c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d4a9c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d4a9c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4a9c-121">Authorization</span></span>  | <span data-ttu-id="d4a9c-122">string</span><span class="sxs-lookup"><span data-stu-id="d4a9c-122">string</span></span>  | <span data-ttu-id="d4a9c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4a9c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4a9c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4a9c-125">Request body</span></span>
<span data-ttu-id="d4a9c-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4a9c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4a9c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4a9c-127">Response</span></span>

<span data-ttu-id="d4a9c-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d4a9c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4a9c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d4a9c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d4a9c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4a9c-131">Request</span></span>
<span data-ttu-id="d4a9c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4a9c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="d4a9c-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4a9c-133">Response</span></span>
<span data-ttu-id="d4a9c-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d4a9c-134">Here is an example of the response.</span></span> 
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
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
