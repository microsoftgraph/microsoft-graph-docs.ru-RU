---
title: Удаление объекта directoryObject
description: Удаление объекта directoryObject
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 63e9d4574c505158171c93fd7ac9dc51678c7d2b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507721"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="7b877-103">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="7b877-103">Delete directoryObject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b877-104">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="7b877-104">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="7b877-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b877-105">Permissions</span></span>
<span data-ttu-id="7b877-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b877-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7b877-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b877-108">Permission type</span></span>      | <span data-ttu-id="7b877-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b877-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b877-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b877-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7b877-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7b877-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7b877-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b877-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b877-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b877-113">Not supported.</span></span>    |
|<span data-ttu-id="7b877-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b877-114">Application</span></span> | <span data-ttu-id="7b877-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b877-115">Not supported.</span></span> |

<span data-ttu-id="7b877-116">**Примечание:** Пользователей, групп и контакты, типы объектов каталога.</span><span class="sxs-lookup"><span data-stu-id="7b877-116">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="7b877-117">В результате, если вам потребуется удалить пользователей, следующие разрешения можно и должен использоваться: User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b877-117">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="7b877-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b877-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="7b877-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b877-119">Request headers</span></span>
| <span data-ttu-id="7b877-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7b877-120">Name</span></span>       | <span data-ttu-id="7b877-121">Тип</span><span class="sxs-lookup"><span data-stu-id="7b877-121">Type</span></span> | <span data-ttu-id="7b877-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7b877-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7b877-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b877-123">Authorization</span></span>  | <span data-ttu-id="7b877-124">string</span><span class="sxs-lookup"><span data-stu-id="7b877-124">string</span></span>  | <span data-ttu-id="7b877-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b877-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b877-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b877-127">Request body</span></span>
<span data-ttu-id="7b877-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b877-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b877-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b877-129">Response</span></span>

<span data-ttu-id="7b877-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7b877-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b877-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7b877-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b877-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b877-133">Request</span></span>
<span data-ttu-id="7b877-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b877-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="7b877-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b877-135">Response</span></span>
<span data-ttu-id="7b877-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7b877-136">Here is an example of the response.</span></span> 
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
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
