---
title: Удаление allowedGroup из принтераShare
description: Отзовет доступ указанной группы для отправки заданий печати в связанную долю принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: be6d50dad54ac5f9c7995c4dd9b39b49d5b5c1fe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777358"
---
# <a name="delete-allowedgroup-from-printershare"></a><span data-ttu-id="6225c-103">Удаление allowedGroup из принтераShare</span><span class="sxs-lookup"><span data-stu-id="6225c-103">Delete allowedGroup from printerShare</span></span>

<span data-ttu-id="6225c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6225c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6225c-105">Отзовет доступ указанной группы для отправки заданий печати в связанный [принтерShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="6225c-105">Revoke the specified group's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6225c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6225c-106">Permissions</span></span>
<span data-ttu-id="6225c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6225c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6225c-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="6225c-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="6225c-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="6225c-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="6225c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6225c-111">Permission type</span></span> | <span data-ttu-id="6225c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6225c-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="6225c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6225c-113">Delegated (work or school account)</span></span>| <span data-ttu-id="6225c-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6225c-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="6225c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6225c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6225c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6225c-116">Not Supported.</span></span>|
|<span data-ttu-id="6225c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6225c-117">Application</span></span>|<span data-ttu-id="6225c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6225c-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6225c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6225c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/shares/{id}/allowedGroups/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="6225c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6225c-120">Request headers</span></span>
| <span data-ttu-id="6225c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6225c-121">Name</span></span>          | <span data-ttu-id="6225c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6225c-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6225c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6225c-123">Authorization</span></span> | <span data-ttu-id="6225c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6225c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6225c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6225c-126">Request body</span></span>
<span data-ttu-id="6225c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6225c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6225c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6225c-128">Response</span></span>
<span data-ttu-id="6225c-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6225c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6225c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6225c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6225c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6225c-132">Request</span></span>
<span data-ttu-id="6225c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6225c-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6225c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6225c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_allowedgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/shares/{id}/allowedGroups/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="6225c-135">C#</span><span class="sxs-lookup"><span data-stu-id="6225c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-allowedgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6225c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6225c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-allowedgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6225c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6225c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-allowedgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6225c-138">Java</span><span class="sxs-lookup"><span data-stu-id="6225c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-allowedgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6225c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6225c-139">Response</span></span>
<span data-ttu-id="6225c-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6225c-140">The following is an example of the response.</span></span>
><span data-ttu-id="6225c-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6225c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
