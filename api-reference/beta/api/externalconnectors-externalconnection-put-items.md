---
title: Создание externalItem
description: Создание нового externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7939689cf113e709853e5da666d1479e600fe4cd
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467691"
---
# <a name="create-externalitem"></a><span data-ttu-id="d34c5-103">Создание externalItem</span><span class="sxs-lookup"><span data-stu-id="d34c5-103">Create externalItem</span></span>

<span data-ttu-id="d34c5-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="d34c5-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d34c5-105">Создание нового [externalItem](../resources/externalconnectors-externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="d34c5-105">Create a new [externalItem](../resources/externalconnectors-externalitem.md).</span></span>

<span data-ttu-id="d34c5-106">Этот API можно использовать для создания настраиваемой номенклатуры.</span><span class="sxs-lookup"><span data-stu-id="d34c5-106">This API can be used to create a custom item.</span></span> <span data-ttu-id="d34c5-107">Содержащая [externalConnection](../resources/externalconnectors-externalconnection.md) должна иметь [схему,](../resources/externalconnectors-schema.md) зарегистрированную соответствующего типа.</span><span class="sxs-lookup"><span data-stu-id="d34c5-107">The containing [externalConnection](../resources/externalconnectors-externalconnection.md) must have a [schema](../resources/externalconnectors-schema.md) registered of the corresponding type.</span></span>

## <a name="permissions"></a><span data-ttu-id="d34c5-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d34c5-108">Permissions</span></span>

<span data-ttu-id="d34c5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d34c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d34c5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d34c5-111">Permission type</span></span>                        | <span data-ttu-id="d34c5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d34c5-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d34c5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d34c5-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d34c5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d34c5-114">Not supported.</span></span> |
| <span data-ttu-id="d34c5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d34c5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d34c5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d34c5-116">Not supported.</span></span> |
| <span data-ttu-id="d34c5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d34c5-117">Application</span></span>                            | <span data-ttu-id="d34c5-118">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d34c5-118">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d34c5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d34c5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="d34c5-120">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="d34c5-120">Path parameters</span></span>

| <span data-ttu-id="d34c5-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="d34c5-121">Parameter</span></span>     | <span data-ttu-id="d34c5-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d34c5-122">Type</span></span>   | <span data-ttu-id="d34c5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d34c5-123">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="d34c5-124">connection-id</span><span class="sxs-lookup"><span data-stu-id="d34c5-124">connection-id</span></span> | <span data-ttu-id="d34c5-125">String</span><span class="sxs-lookup"><span data-stu-id="d34c5-125">string</span></span> | <span data-ttu-id="d34c5-126">`id`Свойствосодержащего [externalConnection](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="d34c5-126">The `id` property of the containing [externalConnection](../resources/externalconnectors-externalconnection.md)</span></span> |
| <span data-ttu-id="d34c5-127">item-id</span><span class="sxs-lookup"><span data-stu-id="d34c5-127">item-id</span></span>       | <span data-ttu-id="d34c5-128">String</span><span class="sxs-lookup"><span data-stu-id="d34c5-128">string</span></span> | <span data-ttu-id="d34c5-129">Свойство `id` [externalItem,](../resources/externalconnectors-externalitem.md)предоставленное разработчиком.</span><span class="sxs-lookup"><span data-stu-id="d34c5-129">The developer-provided `id` property of the [externalItem](../resources/externalconnectors-externalitem.md).</span></span> <span data-ttu-id="d34c5-130">Если с этим элементом уже не `id` существует, создается новый элемент.</span><span class="sxs-lookup"><span data-stu-id="d34c5-130">If no item already exists with this `id`, a new item is created.</span></span> <span data-ttu-id="d34c5-131">Если элемент уже существует с этим, он `id` перезаписывается объектом, отправленным в тело.</span><span class="sxs-lookup"><span data-stu-id="d34c5-131">If an item already exists with this `id`, it is overwritten by the object sent in the body.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d34c5-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d34c5-132">Request headers</span></span>

| <span data-ttu-id="d34c5-133">Имя</span><span class="sxs-lookup"><span data-stu-id="d34c5-133">Name</span></span>          | <span data-ttu-id="d34c5-134">Описание</span><span class="sxs-lookup"><span data-stu-id="d34c5-134">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="d34c5-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d34c5-135">Authorization</span></span> | <span data-ttu-id="d34c5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d34c5-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d34c5-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d34c5-138">Content-Type</span></span>  | <span data-ttu-id="d34c5-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d34c5-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d34c5-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d34c5-141">Request body</span></span>

<span data-ttu-id="d34c5-142">В теле запроса поставляем представление JSON объекта [externalItem.](../resources/externalconnectors-externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="d34c5-142">In the request body, supply a JSON representation of an [externalItem](../resources/externalconnectors-externalitem.md) object.</span></span> <span data-ttu-id="d34c5-143">Нагрузка ограничена 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="d34c5-143">The payload is limited to 4 MB.</span></span>

### <a name="creating-an-externalitem"></a><span data-ttu-id="d34c5-144">Создание externalItem</span><span class="sxs-lookup"><span data-stu-id="d34c5-144">Creating an externalItem</span></span>

<span data-ttu-id="d34c5-145">При создании поля требуются следующие `externalItem` поля: `acl` и `properties` .</span><span class="sxs-lookup"><span data-stu-id="d34c5-145">When creating an `externalItem`, the following fields are required: `acl`, and `properties`.</span></span> <span data-ttu-id="d34c5-146">Объект `properties` должен содержать по крайней мере одно свойство.</span><span class="sxs-lookup"><span data-stu-id="d34c5-146">The `properties` object must contain at least one property.</span></span>

<span data-ttu-id="d34c5-147">Все `DateTime` свойства типа должны быть в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="d34c5-147">All `DateTime` type properties must be in ISO 8601 format.</span></span>

<span data-ttu-id="d34c5-148">Свойства на объекте должны использовать указанные типы в полезной `externalItem` нагрузке в следующих сценариях:</span><span class="sxs-lookup"><span data-stu-id="d34c5-148">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="d34c5-149">Для `String` свойств типа, если значение содержит символы, не относимые к ASCII.</span><span class="sxs-lookup"><span data-stu-id="d34c5-149">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="d34c5-150">Для всех типов коллекций.</span><span class="sxs-lookup"><span data-stu-id="d34c5-150">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="d34c5-151">При включаем свойстве типа `Collection(DateTime)` необходимо использовать указанный `Collection(DateTimeOffset)` тип.</span><span class="sxs-lookup"><span data-stu-id="d34c5-151">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

## <a name="response"></a><span data-ttu-id="d34c5-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="d34c5-152">Response</span></span>

<span data-ttu-id="d34c5-153">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="d34c5-153">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d34c5-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="d34c5-154">Examples</span></span>

### <a name="example-create-a-custom-item"></a><span data-ttu-id="d34c5-155">Пример: Создание настраиваемой номенклатуры</span><span class="sxs-lookup"><span data-stu-id="d34c5-155">Example: Create a custom item</span></span>

#### <a name="request"></a><span data-ttu-id="d34c5-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="d34c5-156">Request</span></span>

<span data-ttu-id="d34c5-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d34c5-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d34c5-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="d34c5-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_connections",
  "@odata.type": "microsoft.graph.externalConnectors.externalItem"
}-->

```http
PUT https://graph.microsoft.com/beta/external/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "acl": [
    {
      "type": "user",
      "value": "e811976d-83df-4cbd-8b9b-5215b18aa874",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    },
    {
      "type": "group",
      "value": "14m1b9c38qe647f6a",
      "accessType": "deny",
      "identitySource": "external"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "value": "Error in payment gateway...",
    "type": "text"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="d34c5-159">C#</span><span class="sxs-lookup"><span data-stu-id="d34c5-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d34c5-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d34c5-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d34c5-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d34c5-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="d34c5-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="d34c5-162">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="d34c5-163">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d34c5-163">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
