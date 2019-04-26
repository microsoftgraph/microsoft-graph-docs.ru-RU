---
title: Удаление категории Outlook
description: Удаление указанного объекта outlookCategory.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5c909176634d64245d5ff5521c0da68b02e8777b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561371"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="11a62-103">Удаление категории Outlook</span><span class="sxs-lookup"><span data-stu-id="11a62-103">Delete Outlook category</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11a62-104">Удаление указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="11a62-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="11a62-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11a62-105">Permissions</span></span>
<span data-ttu-id="11a62-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11a62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11a62-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11a62-108">Permission type</span></span>      | <span data-ttu-id="11a62-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11a62-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11a62-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11a62-110">Delegated (work or school account)</span></span> | <span data-ttu-id="11a62-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11a62-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="11a62-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11a62-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11a62-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11a62-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="11a62-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11a62-114">Application</span></span> | <span data-ttu-id="11a62-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11a62-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="11a62-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11a62-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="11a62-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11a62-117">Request headers</span></span>
| <span data-ttu-id="11a62-118">Имя</span><span class="sxs-lookup"><span data-stu-id="11a62-118">Name</span></span>      |<span data-ttu-id="11a62-119">Описание</span><span class="sxs-lookup"><span data-stu-id="11a62-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="11a62-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11a62-120">Authorization</span></span>  | <span data-ttu-id="11a62-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11a62-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11a62-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11a62-123">Request body</span></span>
<span data-ttu-id="11a62-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="11a62-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11a62-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="11a62-125">Response</span></span>

<span data-ttu-id="11a62-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="11a62-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11a62-128">Пример</span><span class="sxs-lookup"><span data-stu-id="11a62-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11a62-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="11a62-129">Request</span></span>
<span data-ttu-id="11a62-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11a62-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
##### <a name="response"></a><span data-ttu-id="11a62-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="11a62-131">Response</span></span>
<span data-ttu-id="11a62-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="11a62-132">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
