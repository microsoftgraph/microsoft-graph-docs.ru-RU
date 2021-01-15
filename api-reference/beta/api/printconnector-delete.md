---
title: Удаление соединителя
description: Удалите (отрегистрите) соединители.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: f7b19cf15e7b08ae1d4c34011c8b5b4f5a41b178
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873565"
---
# <a name="delete-connector"></a><span data-ttu-id="27067-103">Удаление соединителя</span><span class="sxs-lookup"><span data-stu-id="27067-103">Delete connector</span></span>

<span data-ttu-id="27067-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27067-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27067-105">Удалите (отключите регистрацию) **printConnector.**</span><span class="sxs-lookup"><span data-stu-id="27067-105">Delete (unregister) a **printConnector**.</span></span>

## <a name="permissions"></a><span data-ttu-id="27067-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27067-106">Permissions</span></span>
<span data-ttu-id="27067-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27067-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="27067-109">Чтобы использовать службу универсальной печати, у пользователя или клиента приложения должна быть активная подписка универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="27067-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="27067-110">Пользователь, выписав его, должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="27067-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="27067-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27067-111">Permission type</span></span> | <span data-ttu-id="27067-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27067-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="27067-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27067-113">Delegated (work or school account)</span></span>| <span data-ttu-id="27067-114">PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27067-114">PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="27067-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27067-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27067-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27067-116">Not Supported.</span></span>|
|<span data-ttu-id="27067-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="27067-117">Application</span></span>|<span data-ttu-id="27067-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27067-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27067-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27067-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/connectors/{id}
```
## <a name="request-headers"></a><span data-ttu-id="27067-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27067-120">Request headers</span></span>
| <span data-ttu-id="27067-121">Имя</span><span class="sxs-lookup"><span data-stu-id="27067-121">Name</span></span>          | <span data-ttu-id="27067-122">Описание</span><span class="sxs-lookup"><span data-stu-id="27067-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="27067-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27067-123">Authorization</span></span> | <span data-ttu-id="27067-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27067-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27067-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27067-126">Request body</span></span>
<span data-ttu-id="27067-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27067-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27067-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="27067-128">Response</span></span>
<span data-ttu-id="27067-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="27067-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="error-conditions-and-messages"></a><span data-ttu-id="27067-131">Условия и сообщения об ошибках</span><span class="sxs-lookup"><span data-stu-id="27067-131">Error conditions and messages</span></span>

|<span data-ttu-id="27067-132">Сценарий</span><span class="sxs-lookup"><span data-stu-id="27067-132">Scenario</span></span>|<span data-ttu-id="27067-133">Метод</span><span class="sxs-lookup"><span data-stu-id="27067-133">Method</span></span>|<span data-ttu-id="27067-134">Код</span><span class="sxs-lookup"><span data-stu-id="27067-134">Code</span></span>|<span data-ttu-id="27067-135">Сообщение</span><span class="sxs-lookup"><span data-stu-id="27067-135">Message</span></span>|
|--------|------|----|-------|
|<span data-ttu-id="27067-136">Пользователь пытается удалить соединители с одним или более зарегистрированными принтерами</span><span class="sxs-lookup"><span data-stu-id="27067-136">User attempts to delete a connector that has one or more printers registered</span></span>|<span data-ttu-id="27067-137">DELETE</span><span class="sxs-lookup"><span data-stu-id="27067-137">DELETE</span></span>|<span data-ttu-id="27067-138">409</span><span class="sxs-lookup"><span data-stu-id="27067-138">409</span></span>|<span data-ttu-id="27067-139">Перед удалением соединителя отрегистрируются связанные принтеры.</span><span class="sxs-lookup"><span data-stu-id="27067-139">Before deleting the connector, please unregister the associated printers.</span></span>|

## <a name="example"></a><span data-ttu-id="27067-140">Пример</span><span class="sxs-lookup"><span data-stu-id="27067-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27067-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="27067-141">Request</span></span>
<span data-ttu-id="27067-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27067-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="27067-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="27067-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connector"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="27067-144">C#</span><span class="sxs-lookup"><span data-stu-id="27067-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27067-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27067-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27067-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27067-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27067-147">Java</span><span class="sxs-lookup"><span data-stu-id="27067-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="27067-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="27067-148">Response</span></span>
<span data-ttu-id="27067-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27067-149">The following is an example of the response.</span></span>
><span data-ttu-id="27067-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27067-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
