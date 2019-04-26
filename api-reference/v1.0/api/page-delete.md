---
title: Удаление страницы
description: Удаление страницы OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 691ec8d4d2f6c95c217a9ddb99fbd4e8608483f9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556468"
---
# <a name="delete-page"></a><span data-ttu-id="38b2c-103">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="38b2c-103">Delete page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38b2c-104">Удаление страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="38b2c-104">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="38b2c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38b2c-105">Permissions</span></span>
<span data-ttu-id="38b2c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38b2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38b2c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38b2c-108">Permission type</span></span>      | <span data-ttu-id="38b2c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38b2c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38b2c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38b2c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="38b2c-111">Notes. ReadWrite, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="38b2c-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="38b2c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38b2c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38b2c-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="38b2c-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="38b2c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38b2c-114">Application</span></span> | <span data-ttu-id="38b2c-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38b2c-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38b2c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38b2c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="38b2c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38b2c-117">Request headers</span></span>
| <span data-ttu-id="38b2c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="38b2c-118">Name</span></span>       | <span data-ttu-id="38b2c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="38b2c-119">Type</span></span> | <span data-ttu-id="38b2c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="38b2c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="38b2c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="38b2c-121">Authorization</span></span>  | <span data-ttu-id="38b2c-122">string</span><span class="sxs-lookup"><span data-stu-id="38b2c-122">string</span></span>  | <span data-ttu-id="38b2c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38b2c-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="38b2c-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="38b2c-125">Response</span></span>

<span data-ttu-id="38b2c-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="38b2c-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38b2c-128">Пример</span><span class="sxs-lookup"><span data-stu-id="38b2c-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38b2c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="38b2c-129">Request</span></span>
<span data-ttu-id="38b2c-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38b2c-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="38b2c-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="38b2c-131">Response</span></span>
<span data-ttu-id="38b2c-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="38b2c-132">Here is an example of the response.</span></span>
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
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
