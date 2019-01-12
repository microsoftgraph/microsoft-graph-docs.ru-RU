---
title: Удаление категории Outlook
description: Удаление указанного объекта outlookCategory.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5c909176634d64245d5ff5521c0da68b02e8777b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972266"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="1c639-103">Удаление категории Outlook</span><span class="sxs-lookup"><span data-stu-id="1c639-103">Delete Outlook category</span></span>


<span data-ttu-id="1c639-104">Удаление указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="1c639-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c639-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c639-105">Permissions</span></span>
<span data-ttu-id="1c639-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c639-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c639-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c639-108">Permission type</span></span>      | <span data-ttu-id="1c639-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c639-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c639-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c639-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1c639-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c639-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1c639-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c639-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c639-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c639-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1c639-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c639-114">Application</span></span> | <span data-ttu-id="1c639-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c639-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c639-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c639-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1c639-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c639-117">Request headers</span></span>
| <span data-ttu-id="1c639-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1c639-118">Name</span></span>      |<span data-ttu-id="1c639-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1c639-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1c639-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c639-120">Authorization</span></span>  | <span data-ttu-id="1c639-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c639-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c639-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1c639-123">Request body</span></span>
<span data-ttu-id="1c639-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c639-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c639-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c639-125">Response</span></span>

<span data-ttu-id="1c639-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1c639-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c639-128">Пример</span><span class="sxs-lookup"><span data-stu-id="1c639-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c639-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c639-129">Request</span></span>
<span data-ttu-id="1c639-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c639-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"],
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
##### <a name="response"></a><span data-ttu-id="1c639-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c639-131">Response</span></span>
<span data-ttu-id="1c639-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1c639-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
