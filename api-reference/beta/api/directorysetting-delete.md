---
title: Удаление параметров каталога
description: Удалите параметр каталога.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c66335ec863460c9b2167e25a7e78850846e105c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515827"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="09440-103">Удаление параметров каталога</span><span class="sxs-lookup"><span data-stu-id="09440-103">Delete a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09440-104">Удалите параметр каталога.</span><span class="sxs-lookup"><span data-stu-id="09440-104">Delete a directory setting.</span></span>

> <span data-ttu-id="09440-105">**Примечание**: версия /beta этот интерфейс API является только относится к группам.</span><span class="sxs-lookup"><span data-stu-id="09440-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="09440-106">Для *удаления groupSettings*переименован версии /v1.0 этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="09440-106">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="09440-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09440-107">Permissions</span></span>
<span data-ttu-id="09440-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09440-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09440-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09440-110">Permission type</span></span>      | <span data-ttu-id="09440-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09440-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09440-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09440-112">Delegated (work or school account)</span></span> | <span data-ttu-id="09440-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09440-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="09440-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09440-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09440-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09440-115">Not supported.</span></span>    |
|<span data-ttu-id="09440-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09440-116">Application</span></span> | <span data-ttu-id="09440-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09440-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09440-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09440-118">HTTP request</span></span>
<span data-ttu-id="09440-119"><!-- { "blockType": "ignored" } -->Удаление конкретных всей клиента или параметр групповой</span><span class="sxs-lookup"><span data-stu-id="09440-119"><!-- { "blockType": "ignored" } --> Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="09440-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09440-120">Request headers</span></span>
| <span data-ttu-id="09440-121">Имя</span><span class="sxs-lookup"><span data-stu-id="09440-121">Name</span></span>       | <span data-ttu-id="09440-122">Описание</span><span class="sxs-lookup"><span data-stu-id="09440-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="09440-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09440-123">Authorization</span></span>  | <span data-ttu-id="09440-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09440-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09440-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09440-126">Request body</span></span>
<span data-ttu-id="09440-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="09440-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09440-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="09440-128">Response</span></span>

<span data-ttu-id="09440-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="09440-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09440-131">Пример</span><span class="sxs-lookup"><span data-stu-id="09440-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09440-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="09440-132">Request</span></span>
<span data-ttu-id="09440-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09440-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="09440-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="09440-134">Response</span></span>
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
  "description": "Delete directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
