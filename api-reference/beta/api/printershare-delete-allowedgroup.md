---
title: Удаление allowedGroup из принтераShare
description: Отзовет доступ указанной группы для отправки заданий печати в связанную долю принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: dce2a4d044b555116396953e926ef3c5d8c13fb0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051062"
---
# <a name="delete-allowedgroup-from-printershare"></a><span data-ttu-id="686a2-103">Удаление allowedGroup из принтераShare</span><span class="sxs-lookup"><span data-stu-id="686a2-103">Delete allowedGroup from printerShare</span></span>

<span data-ttu-id="686a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="686a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="686a2-105">Отзовет доступ указанной группы для отправки заданий печати в связанный [принтерShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="686a2-105">Revoke the specified group's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="686a2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="686a2-106">Permissions</span></span>
<span data-ttu-id="686a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="686a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="686a2-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="686a2-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="686a2-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="686a2-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="686a2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="686a2-111">Permission type</span></span> | <span data-ttu-id="686a2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="686a2-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="686a2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="686a2-113">Delegated (work or school account)</span></span>| <span data-ttu-id="686a2-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="686a2-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="686a2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="686a2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="686a2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="686a2-116">Not Supported.</span></span>|
|<span data-ttu-id="686a2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="686a2-117">Application</span></span>|<span data-ttu-id="686a2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="686a2-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="686a2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="686a2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/shares/{id}/allowedGroups/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="686a2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="686a2-120">Request headers</span></span>
| <span data-ttu-id="686a2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="686a2-121">Name</span></span>          | <span data-ttu-id="686a2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="686a2-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="686a2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="686a2-123">Authorization</span></span> | <span data-ttu-id="686a2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="686a2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="686a2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="686a2-126">Request body</span></span>
<span data-ttu-id="686a2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="686a2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="686a2-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="686a2-128">Response</span></span>
<span data-ttu-id="686a2-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="686a2-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="686a2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="686a2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="686a2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="686a2-132">Request</span></span>
<span data-ttu-id="686a2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="686a2-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="686a2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="686a2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_allowedgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/shares/{id}/allowedGroups/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="686a2-135">C#</span><span class="sxs-lookup"><span data-stu-id="686a2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-allowedgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="686a2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="686a2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-allowedgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="686a2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="686a2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-allowedgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="686a2-138">Java</span><span class="sxs-lookup"><span data-stu-id="686a2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-allowedgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="686a2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="686a2-139">Response</span></span>
<span data-ttu-id="686a2-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="686a2-140">The following is an example of the response.</span></span>
><span data-ttu-id="686a2-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="686a2-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete allowedGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
