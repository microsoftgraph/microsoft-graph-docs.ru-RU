---
title: Удаление категории Outlook
description: Удаление указанного объекта outlookCategory.
author: angelgolfer-ms
ms.openlocfilehash: 1654b0d67e61ea9f999495eb239eb1d837690159
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321240"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="85411-103">Удаление категории Outlook</span><span class="sxs-lookup"><span data-stu-id="85411-103">Delete Outlook category</span></span>

> <span data-ttu-id="85411-104">**Важно**: интерфейсы API в разделе версии /beta в Microsoft Graph в предварительной версии и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="85411-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85411-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85411-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85411-106">Удаление указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="85411-106">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="85411-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85411-107">Permissions</span></span>
<span data-ttu-id="85411-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85411-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85411-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85411-110">Permission type</span></span>      | <span data-ttu-id="85411-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85411-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85411-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85411-112">Delegated (work or school account)</span></span> | <span data-ttu-id="85411-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85411-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="85411-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85411-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85411-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85411-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="85411-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85411-116">Application</span></span> | <span data-ttu-id="85411-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85411-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="85411-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85411-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="85411-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="85411-119">Optional query parameters</span></span>
<span data-ttu-id="85411-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="85411-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85411-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85411-121">Request headers</span></span>
| <span data-ttu-id="85411-122">Имя</span><span class="sxs-lookup"><span data-stu-id="85411-122">Name</span></span>      |<span data-ttu-id="85411-123">Описание</span><span class="sxs-lookup"><span data-stu-id="85411-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="85411-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85411-124">Authorization</span></span>  | <span data-ttu-id="85411-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85411-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85411-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85411-127">Request body</span></span>
<span data-ttu-id="85411-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85411-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85411-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="85411-129">Response</span></span>

<span data-ttu-id="85411-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="85411-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85411-132">Пример</span><span class="sxs-lookup"><span data-stu-id="85411-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85411-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="85411-133">Request</span></span>
<span data-ttu-id="85411-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85411-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/masterCategories('4b1c2495-54c9-4a5e-90a2-0ab0b31987d8')
```
##### <a name="response"></a><span data-ttu-id="85411-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="85411-135">Response</span></span>
<span data-ttu-id="85411-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="85411-136">Here is an example of the response.</span></span>
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