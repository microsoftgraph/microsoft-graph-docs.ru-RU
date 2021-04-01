---
title: Создание externalItem
description: Создание нового externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b4617596a10a85a4378b1e7ad4c4ca94fb16ffac
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491011"
---
# <a name="create-externalitem"></a><span data-ttu-id="661d5-103">Создание externalItem</span><span class="sxs-lookup"><span data-stu-id="661d5-103">Create externalItem</span></span>

<span data-ttu-id="661d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="661d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="661d5-105">Создание нового [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="661d5-105">Create a new [externalItem](../resources/externalitem.md).</span></span>

<span data-ttu-id="661d5-106">Этот API можно использовать для создания настраиваемой номенклатуры.</span><span class="sxs-lookup"><span data-stu-id="661d5-106">This API can be used to create a custom item.</span></span> <span data-ttu-id="661d5-107">Укажите тип, который вы создаете, включив `@odata.type` свойство в тело JSON.</span><span class="sxs-lookup"><span data-stu-id="661d5-107">Specify the type you are creating by including the `@odata.type` property in the JSON body.</span></span> <span data-ttu-id="661d5-108">Содержащая [externalConnection](../resources/externalconnection.md) должна иметь [схему,](../resources/schema.md) зарегистрированную соответствующего типа.</span><span class="sxs-lookup"><span data-stu-id="661d5-108">The containing [externalConnection](../resources/externalconnection.md) must have a [schema](../resources/schema.md) registered of the corresponding type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="661d5-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="661d5-109">Permissions</span></span>

<span data-ttu-id="661d5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="661d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="661d5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="661d5-112">Permission type</span></span>                        | <span data-ttu-id="661d5-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="661d5-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="661d5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="661d5-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="661d5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="661d5-115">Not supported.</span></span> |
| <span data-ttu-id="661d5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="661d5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="661d5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="661d5-117">Not supported.</span></span> |
| <span data-ttu-id="661d5-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="661d5-118">Application</span></span>                            | <span data-ttu-id="661d5-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="661d5-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="661d5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="661d5-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="661d5-121">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="661d5-121">Path parameters</span></span>

| <span data-ttu-id="661d5-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="661d5-122">Parameter</span></span>     | <span data-ttu-id="661d5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="661d5-123">Type</span></span>   | <span data-ttu-id="661d5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="661d5-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="661d5-125">connection-id</span><span class="sxs-lookup"><span data-stu-id="661d5-125">connection-id</span></span> | <span data-ttu-id="661d5-126">string</span><span class="sxs-lookup"><span data-stu-id="661d5-126">string</span></span> | <span data-ttu-id="661d5-127">`id`Свойствосодержащего [externalConnection](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="661d5-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="661d5-128">item-id</span><span class="sxs-lookup"><span data-stu-id="661d5-128">item-id</span></span>       | <span data-ttu-id="661d5-129">string</span><span class="sxs-lookup"><span data-stu-id="661d5-129">string</span></span> | <span data-ttu-id="661d5-130">Свойство `id` [externalItem,](../resources/externalitem.md)предоставленное разработчиком.</span><span class="sxs-lookup"><span data-stu-id="661d5-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> <span data-ttu-id="661d5-131">Если с этим элементом уже не `id` существует, создается новый элемент.</span><span class="sxs-lookup"><span data-stu-id="661d5-131">If no item already exists with this `id`, a new item is created.</span></span> <span data-ttu-id="661d5-132">Если элемент уже существует с этим, он `id` перезаписывается объектом, отправленным в тело.</span><span class="sxs-lookup"><span data-stu-id="661d5-132">If an item already exists with this `id`, it is overwritten by the object sent in the body.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="661d5-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="661d5-133">Request headers</span></span>

| <span data-ttu-id="661d5-134">Имя</span><span class="sxs-lookup"><span data-stu-id="661d5-134">Name</span></span>          | <span data-ttu-id="661d5-135">Описание</span><span class="sxs-lookup"><span data-stu-id="661d5-135">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="661d5-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="661d5-136">Authorization</span></span> | <span data-ttu-id="661d5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="661d5-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="661d5-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="661d5-139">Content-Type</span></span>  | <span data-ttu-id="661d5-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="661d5-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="661d5-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="661d5-142">Request body</span></span>

<span data-ttu-id="661d5-143">В теле запроса поставляем представление JSON объекта [externalItem.](../resources/externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="661d5-143">In the request body, supply a JSON representation of an [externalItem](../resources/externalitem.md) object.</span></span> <span data-ttu-id="661d5-144">Нагрузка ограничена 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="661d5-144">The payload is limited to 4 MB.</span></span>

### <a name="creating-an-externalitem"></a><span data-ttu-id="661d5-145">Создание externalItem</span><span class="sxs-lookup"><span data-stu-id="661d5-145">Creating an externalItem</span></span>

<span data-ttu-id="661d5-146">При создании поля требуются следующие `externalItem` поля: `@odata.type` и `acl` `properties` .</span><span class="sxs-lookup"><span data-stu-id="661d5-146">When creating an `externalItem`, the following fields are required: `@odata.type`, `acl`, and `properties`.</span></span> <span data-ttu-id="661d5-147">Объект `properties` должен содержать по крайней мере одно свойство.</span><span class="sxs-lookup"><span data-stu-id="661d5-147">The `properties` object must contain at least one property.</span></span>

<span data-ttu-id="661d5-148">Все `DateTime` свойства типа должны быть в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="661d5-148">All `DateTime` type properties must be in ISO 8601 format.</span></span>

<span data-ttu-id="661d5-149">Свойства на объекте должны использовать указанные типы в полезной `externalItem` нагрузке в следующих сценариях:</span><span class="sxs-lookup"><span data-stu-id="661d5-149">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="661d5-150">Для `String` свойств типа, если значение содержит символы, не относимые к ASCII.</span><span class="sxs-lookup"><span data-stu-id="661d5-150">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="661d5-151">Для всех типов коллекций.</span><span class="sxs-lookup"><span data-stu-id="661d5-151">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="661d5-152">При включаем свойстве типа `Collection(DateTime)` необходимо использовать указанный `Collection(DateTimeOffset)` тип.</span><span class="sxs-lookup"><span data-stu-id="661d5-152">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

## <a name="response"></a><span data-ttu-id="661d5-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="661d5-153">Response</span></span>

<span data-ttu-id="661d5-154">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="661d5-154">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="661d5-155">Примеры</span><span class="sxs-lookup"><span data-stu-id="661d5-155">Examples</span></span>

### <a name="example-create-a-custom-item"></a><span data-ttu-id="661d5-156">Пример: Создание настраиваемой номенклатуры</span><span class="sxs-lookup"><span data-stu-id="661d5-156">Example: Create a custom item</span></span>

#### <a name="request"></a><span data-ttu-id="661d5-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="661d5-157">Request</span></span>

<span data-ttu-id="661d5-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="661d5-158">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="661d5-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="661d5-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_connections"
}-->

```http
PUT https://graph.microsoft.com/beta/external/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "@odata.type": "microsoft.graph.externalItem",
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
# <a name="c"></a>[<span data-ttu-id="661d5-160">C#</span><span class="sxs-lookup"><span data-stu-id="661d5-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="661d5-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="661d5-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="661d5-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="661d5-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="661d5-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="661d5-163">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="661d5-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="661d5-164">The following is an example of the response.</span></span>

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
