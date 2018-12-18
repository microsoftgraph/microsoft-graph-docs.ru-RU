---
title: Удаление категории Outlook
description: Удаление указанного объекта outlookCategory.
author: angelgolfer-ms
ms.openlocfilehash: ded640425c30352cc83d4adaa02c76ed2bcfa170
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301038"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="a3389-103">Удаление категории Outlook</span><span class="sxs-lookup"><span data-stu-id="a3389-103">Delete Outlook category</span></span>


<span data-ttu-id="a3389-104">Удаление указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="a3389-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3389-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3389-105">Permissions</span></span>
<span data-ttu-id="a3389-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3389-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3389-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3389-108">Permission type</span></span>      | <span data-ttu-id="a3389-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3389-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3389-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3389-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a3389-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3389-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="a3389-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3389-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3389-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3389-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="a3389-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3389-114">Application</span></span> | <span data-ttu-id="a3389-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3389-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3389-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3389-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a3389-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a3389-117">Optional query parameters</span></span>
<span data-ttu-id="a3389-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a3389-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3389-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3389-119">Request headers</span></span>
| <span data-ttu-id="a3389-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a3389-120">Name</span></span>      |<span data-ttu-id="a3389-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a3389-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a3389-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3389-122">Authorization</span></span>  | <span data-ttu-id="a3389-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3389-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3389-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3389-125">Request body</span></span>
<span data-ttu-id="a3389-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3389-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3389-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3389-127">Response</span></span>

<span data-ttu-id="a3389-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a3389-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3389-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a3389-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3389-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3389-131">Request</span></span>
<span data-ttu-id="a3389-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3389-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"],
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
##### <a name="response"></a><span data-ttu-id="a3389-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3389-133">Response</span></span>
<span data-ttu-id="a3389-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a3389-134">Here is an example of the response.</span></span>
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