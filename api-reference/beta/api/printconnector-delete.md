---
title: Удаление соединителя
description: Удаление (Отмена регистрации) соединителя.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7740f8d9976db1f6bc7f2daf300342f4cab98c98
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674318"
---
# <a name="delete-connector"></a><span data-ttu-id="f07ff-103">Удаление соединителя</span><span class="sxs-lookup"><span data-stu-id="f07ff-103">Delete connector</span></span>

<span data-ttu-id="f07ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f07ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f07ff-105">Удаление (Отмена регистрации) **принтконнектор**.</span><span class="sxs-lookup"><span data-stu-id="f07ff-105">Delete (unregister) a **printConnector**.</span></span>

## <a name="permissions"></a><span data-ttu-id="f07ff-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f07ff-106">Permissions</span></span>
<span data-ttu-id="f07ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f07ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f07ff-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="f07ff-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="f07ff-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="f07ff-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="f07ff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f07ff-111">Permission type</span></span> | <span data-ttu-id="f07ff-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f07ff-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f07ff-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f07ff-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f07ff-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="f07ff-114">User.Read</span></span> |
|<span data-ttu-id="f07ff-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f07ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f07ff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f07ff-116">Not Supported.</span></span>|
|<span data-ttu-id="f07ff-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f07ff-117">Application</span></span>|<span data-ttu-id="f07ff-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f07ff-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f07ff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f07ff-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/connectors/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f07ff-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f07ff-120">Request headers</span></span>
| <span data-ttu-id="f07ff-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f07ff-121">Name</span></span>          | <span data-ttu-id="f07ff-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f07ff-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f07ff-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f07ff-123">Authorization</span></span> | <span data-ttu-id="f07ff-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f07ff-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f07ff-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f07ff-126">Request body</span></span>
<span data-ttu-id="f07ff-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f07ff-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f07ff-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f07ff-128">Response</span></span>
<span data-ttu-id="f07ff-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f07ff-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="error-conditions-and-messages"></a><span data-ttu-id="f07ff-131">Условия и сообщения об ошибках</span><span class="sxs-lookup"><span data-stu-id="f07ff-131">Error conditions and messages</span></span>

|<span data-ttu-id="f07ff-132">Сценарий</span><span class="sxs-lookup"><span data-stu-id="f07ff-132">Scenario</span></span>|<span data-ttu-id="f07ff-133">Метод</span><span class="sxs-lookup"><span data-stu-id="f07ff-133">Method</span></span>|<span data-ttu-id="f07ff-134">Код</span><span class="sxs-lookup"><span data-stu-id="f07ff-134">Code</span></span>|<span data-ttu-id="f07ff-135">Сообщение</span><span class="sxs-lookup"><span data-stu-id="f07ff-135">Message</span></span>|
|--------|------|----|-------|
|<span data-ttu-id="f07ff-136">Пользователь пытается удалить соединитель с одним или несколькими зарегистрированными принтерами</span><span class="sxs-lookup"><span data-stu-id="f07ff-136">User attempts to delete a connector that has one or more printers registered</span></span>|<span data-ttu-id="f07ff-137">DELETE</span><span class="sxs-lookup"><span data-stu-id="f07ff-137">DELETE</span></span>|<span data-ttu-id="f07ff-138">409</span><span class="sxs-lookup"><span data-stu-id="f07ff-138">409</span></span>|<span data-ttu-id="f07ff-139">Перед удалением соединителя отмените регистрацию связанных принтеров.</span><span class="sxs-lookup"><span data-stu-id="f07ff-139">Before deleting the connector, please unregister the associated printers.</span></span>|

## <a name="example"></a><span data-ttu-id="f07ff-140">Пример</span><span class="sxs-lookup"><span data-stu-id="f07ff-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f07ff-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="f07ff-141">Request</span></span>
<span data-ttu-id="f07ff-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f07ff-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f07ff-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="f07ff-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connector"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="f07ff-144">C#</span><span class="sxs-lookup"><span data-stu-id="f07ff-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f07ff-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f07ff-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f07ff-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f07ff-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f07ff-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="f07ff-147">Response</span></span>
<span data-ttu-id="f07ff-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f07ff-148">The following is an example of the response.</span></span>
><span data-ttu-id="f07ff-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f07ff-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
