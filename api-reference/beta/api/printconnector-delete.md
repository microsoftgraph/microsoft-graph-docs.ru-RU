---
title: Удаление соединителя
description: Удаление (незарегистрированного) соединитетеля.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 99a8a4d0da5f3abb4beccfc1a196b8567f690303
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053617"
---
# <a name="delete-connector"></a><span data-ttu-id="0dc19-103">Удаление соединителя</span><span class="sxs-lookup"><span data-stu-id="0dc19-103">Delete connector</span></span>

<span data-ttu-id="0dc19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dc19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0dc19-105">Удаление (незарегистрированного) **printConnector**.</span><span class="sxs-lookup"><span data-stu-id="0dc19-105">Delete (unregister) a **printConnector**.</span></span>

## <a name="permissions"></a><span data-ttu-id="0dc19-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0dc19-106">Permissions</span></span>
<span data-ttu-id="0dc19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0dc19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0dc19-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="0dc19-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="0dc19-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="0dc19-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="0dc19-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0dc19-111">Permission type</span></span> | <span data-ttu-id="0dc19-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0dc19-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0dc19-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0dc19-113">Delegated (work or school account)</span></span>| <span data-ttu-id="0dc19-114">PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dc19-114">PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="0dc19-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0dc19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0dc19-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0dc19-116">Not Supported.</span></span>|
|<span data-ttu-id="0dc19-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0dc19-117">Application</span></span>|<span data-ttu-id="0dc19-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0dc19-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0dc19-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0dc19-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/connectors/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0dc19-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0dc19-120">Request headers</span></span>
| <span data-ttu-id="0dc19-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0dc19-121">Name</span></span>          | <span data-ttu-id="0dc19-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0dc19-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0dc19-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0dc19-123">Authorization</span></span> | <span data-ttu-id="0dc19-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0dc19-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0dc19-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0dc19-126">Request body</span></span>
<span data-ttu-id="0dc19-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0dc19-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0dc19-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0dc19-128">Response</span></span>
<span data-ttu-id="0dc19-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0dc19-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="error-conditions-and-messages"></a><span data-ttu-id="0dc19-131">Условия ошибки и сообщения</span><span class="sxs-lookup"><span data-stu-id="0dc19-131">Error conditions and messages</span></span>

|<span data-ttu-id="0dc19-132">Сценарий</span><span class="sxs-lookup"><span data-stu-id="0dc19-132">Scenario</span></span>|<span data-ttu-id="0dc19-133">Method</span><span class="sxs-lookup"><span data-stu-id="0dc19-133">Method</span></span>|<span data-ttu-id="0dc19-134">Код</span><span class="sxs-lookup"><span data-stu-id="0dc19-134">Code</span></span>|<span data-ttu-id="0dc19-135">Сообщение</span><span class="sxs-lookup"><span data-stu-id="0dc19-135">Message</span></span>|
|--------|------|----|-------|
|<span data-ttu-id="0dc19-136">Пользователь пытается удалить соединителя, который имеет один или несколько принтеров зарегистрированы</span><span class="sxs-lookup"><span data-stu-id="0dc19-136">User attempts to delete a connector that has one or more printers registered</span></span>|<span data-ttu-id="0dc19-137">DELETE</span><span class="sxs-lookup"><span data-stu-id="0dc19-137">DELETE</span></span>|<span data-ttu-id="0dc19-138">409</span><span class="sxs-lookup"><span data-stu-id="0dc19-138">409</span></span>|<span data-ttu-id="0dc19-139">Перед удалением соединителя удаляйте связанные принтеры.</span><span class="sxs-lookup"><span data-stu-id="0dc19-139">Before deleting the connector, please unregister the associated printers.</span></span>|

## <a name="example"></a><span data-ttu-id="0dc19-140">Пример</span><span class="sxs-lookup"><span data-stu-id="0dc19-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0dc19-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="0dc19-141">Request</span></span>
<span data-ttu-id="0dc19-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0dc19-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0dc19-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="0dc19-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connector"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="0dc19-144">C#</span><span class="sxs-lookup"><span data-stu-id="0dc19-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0dc19-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0dc19-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0dc19-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0dc19-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0dc19-147">Java</span><span class="sxs-lookup"><span data-stu-id="0dc19-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0dc19-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="0dc19-148">Response</span></span>
<span data-ttu-id="0dc19-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0dc19-149">The following is an example of the response.</span></span>
><span data-ttu-id="0dc19-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0dc19-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Delete connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
