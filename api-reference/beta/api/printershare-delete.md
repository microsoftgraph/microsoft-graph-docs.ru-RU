---
title: Удаление printerShare
description: Удаление общего принтера (отменяйте общий доступ к связанному принтеру). Это действие невозможно отменить. Если к принтеру предоставлен общий доступ в будущем, все пользователи Windows, на которых ранее устанавливался принтер, должны обнаружить и повторно установить его.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: b500be46b0667326e62426fb7ff50ec076e47631
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979767"
---
# <a name="delete-printershare"></a><span data-ttu-id="0aded-105">Удаление printerShare</span><span class="sxs-lookup"><span data-stu-id="0aded-105">Delete printerShare</span></span>

<span data-ttu-id="0aded-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0aded-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0aded-107">Удаление общего принтера (отменяйте общий доступ к связанному [принтеру](../resources/printer.md)).</span><span class="sxs-lookup"><span data-stu-id="0aded-107">Delete a printer share (unshare the associated [printer](../resources/printer.md)).</span></span> <span data-ttu-id="0aded-108">Это действие невозможно отменить.</span><span class="sxs-lookup"><span data-stu-id="0aded-108">This action cannot be undone.</span></span> <span data-ttu-id="0aded-109">Если к [принтеру](../resources/printer.md) предоставлен общий доступ в будущем, все пользователи Windows, на которых ранее устанавливался [принтер](../resources/printer.md) , должны обнаружить и переустановить его.</span><span class="sxs-lookup"><span data-stu-id="0aded-109">If the [printer](../resources/printer.md) is shared again in the future, any Windows users who had previously installed the [printer](../resources/printer.md) will need to discover and reinstall it.</span></span>

## <a name="permissions"></a><span data-ttu-id="0aded-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0aded-110">Permissions</span></span>
<span data-ttu-id="0aded-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0aded-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0aded-113">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="0aded-113">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="0aded-114">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="0aded-114">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="0aded-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0aded-115">Permission type</span></span> | <span data-ttu-id="0aded-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0aded-116">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0aded-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0aded-117">Delegated (work or school account)</span></span>| <span data-ttu-id="0aded-118">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0aded-118">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="0aded-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0aded-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0aded-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0aded-120">Not Supported.</span></span>|
|<span data-ttu-id="0aded-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0aded-121">Application</span></span>|<span data-ttu-id="0aded-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0aded-122">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0aded-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0aded-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/shares/{id}
DELETE /print/printers/{id}/share
```
## <a name="request-headers"></a><span data-ttu-id="0aded-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0aded-124">Request headers</span></span>
| <span data-ttu-id="0aded-125">Имя</span><span class="sxs-lookup"><span data-stu-id="0aded-125">Name</span></span>          | <span data-ttu-id="0aded-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0aded-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0aded-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0aded-127">Authorization</span></span> | <span data-ttu-id="0aded-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0aded-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0aded-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0aded-130">Request body</span></span>
<span data-ttu-id="0aded-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0aded-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0aded-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0aded-132">Response</span></span>
<span data-ttu-id="0aded-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0aded-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aded-135">Пример</span><span class="sxs-lookup"><span data-stu-id="0aded-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0aded-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="0aded-136">Request</span></span>
<span data-ttu-id="0aded-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0aded-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0aded-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="0aded-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printershare"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/shares/{id}
```
# <a name="c"></a>[<span data-ttu-id="0aded-139">C#</span><span class="sxs-lookup"><span data-stu-id="0aded-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0aded-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0aded-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0aded-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0aded-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0aded-142">Java</span><span class="sxs-lookup"><span data-stu-id="0aded-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0aded-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0aded-143">Response</span></span>
<span data-ttu-id="0aded-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0aded-144">The following is an example of the response.</span></span>
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
  "description": "Delete printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
