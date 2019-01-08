---
title: Удаление категории Outlook
description: Удаление указанного объекта outlookCategory.
author: angelgolfer-ms
ms.openlocfilehash: b82125c33c7b11274bfee80d9d1949ea776745c4
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748495"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="e97c5-103">Удаление категории Outlook</span><span class="sxs-lookup"><span data-stu-id="e97c5-103">Delete Outlook category</span></span>


<span data-ttu-id="e97c5-104">Удаление указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="e97c5-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e97c5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e97c5-105">Permissions</span></span>
<span data-ttu-id="e97c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e97c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e97c5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e97c5-108">Permission type</span></span>      | <span data-ttu-id="e97c5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e97c5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e97c5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e97c5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e97c5-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e97c5-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e97c5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e97c5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e97c5-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e97c5-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e97c5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e97c5-114">Application</span></span> | <span data-ttu-id="e97c5-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e97c5-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e97c5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e97c5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e97c5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e97c5-117">Request headers</span></span>
| <span data-ttu-id="e97c5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e97c5-118">Name</span></span>      |<span data-ttu-id="e97c5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e97c5-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e97c5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e97c5-120">Authorization</span></span>  | <span data-ttu-id="e97c5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e97c5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e97c5-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e97c5-123">Request body</span></span>
<span data-ttu-id="e97c5-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e97c5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e97c5-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="e97c5-125">Response</span></span>

<span data-ttu-id="e97c5-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e97c5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e97c5-128">Пример</span><span class="sxs-lookup"><span data-stu-id="e97c5-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e97c5-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e97c5-129">Request</span></span>
<span data-ttu-id="e97c5-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e97c5-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"],
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
##### <a name="response"></a><span data-ttu-id="e97c5-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e97c5-131">Response</span></span>
<span data-ttu-id="e97c5-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e97c5-132">Here is an example of the response.</span></span>
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