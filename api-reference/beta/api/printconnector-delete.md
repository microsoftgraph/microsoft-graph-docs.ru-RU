---
title: Удаление соединителя
description: Удаление (Отмена регистрации) соединителя.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 03a8e040a2254798eb140075b02fe181021fb8ec
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2020
ms.locfileid: "42948178"
---
# <a name="delete-connector"></a><span data-ttu-id="497f7-103">Удаление соединителя</span><span class="sxs-lookup"><span data-stu-id="497f7-103">Delete connector</span></span>

<span data-ttu-id="497f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="497f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="497f7-105">Удаление (Отмена регистрации) **принтконнектор**.</span><span class="sxs-lookup"><span data-stu-id="497f7-105">Delete (unregister) a **printConnector**.</span></span>

## <a name="permissions"></a><span data-ttu-id="497f7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="497f7-106">Permissions</span></span>
<span data-ttu-id="497f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="497f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="497f7-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="497f7-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="497f7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="497f7-110">Permission type</span></span> | <span data-ttu-id="497f7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="497f7-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="497f7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="497f7-112">Delegated (work or school account)</span></span>| <span data-ttu-id="497f7-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="497f7-113">Users.Read.All</span></span> |
|<span data-ttu-id="497f7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="497f7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="497f7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="497f7-115">Not Supported.</span></span>|
|<span data-ttu-id="497f7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="497f7-116">Application</span></span>|<span data-ttu-id="497f7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="497f7-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="497f7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="497f7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/connectors/{id}
```
## <a name="request-headers"></a><span data-ttu-id="497f7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="497f7-119">Request headers</span></span>
| <span data-ttu-id="497f7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="497f7-120">Name</span></span>          | <span data-ttu-id="497f7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="497f7-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="497f7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="497f7-122">Authorization</span></span> | <span data-ttu-id="497f7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="497f7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="497f7-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="497f7-125">Request body</span></span>
<span data-ttu-id="497f7-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="497f7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="497f7-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="497f7-127">Response</span></span>
<span data-ttu-id="497f7-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="497f7-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="error-conditions-and-messages"></a><span data-ttu-id="497f7-130">Условия и сообщения об ошибках</span><span class="sxs-lookup"><span data-stu-id="497f7-130">Error conditions and messages</span></span>

|<span data-ttu-id="497f7-131">Сценарий</span><span class="sxs-lookup"><span data-stu-id="497f7-131">Scenario</span></span>|<span data-ttu-id="497f7-132">Method</span><span class="sxs-lookup"><span data-stu-id="497f7-132">Method</span></span>|<span data-ttu-id="497f7-133">Код</span><span class="sxs-lookup"><span data-stu-id="497f7-133">Code</span></span>|<span data-ttu-id="497f7-134">Сообщение</span><span class="sxs-lookup"><span data-stu-id="497f7-134">Message</span></span>|
|--------|------|----|-------|
|<span data-ttu-id="497f7-135">Пользователь пытается удалить соединитель с одним или несколькими зарегистрированными принтерами</span><span class="sxs-lookup"><span data-stu-id="497f7-135">User attempts to delete a connector that has one or more printers registered</span></span>|<span data-ttu-id="497f7-136">DELETE</span><span class="sxs-lookup"><span data-stu-id="497f7-136">DELETE</span></span>|<span data-ttu-id="497f7-137">409</span><span class="sxs-lookup"><span data-stu-id="497f7-137">409</span></span>|<span data-ttu-id="497f7-138">Перед удалением соединителя отмените регистрацию связанных принтеров.</span><span class="sxs-lookup"><span data-stu-id="497f7-138">Before deleting the connector, please unregister the associated printers.</span></span>|

## <a name="example"></a><span data-ttu-id="497f7-139">Пример</span><span class="sxs-lookup"><span data-stu-id="497f7-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="497f7-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="497f7-140">Request</span></span>
<span data-ttu-id="497f7-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="497f7-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="497f7-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="497f7-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connector"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="497f7-143">C#</span><span class="sxs-lookup"><span data-stu-id="497f7-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="497f7-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="497f7-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="497f7-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="497f7-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="497f7-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="497f7-146">Response</span></span>
<span data-ttu-id="497f7-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="497f7-147">The following is an example of the response.</span></span>
><span data-ttu-id="497f7-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="497f7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
