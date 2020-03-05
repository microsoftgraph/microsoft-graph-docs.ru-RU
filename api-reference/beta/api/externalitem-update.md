---
title: Обновление екстерналитем
description: Обновление свойств объекта екстерналитем.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: ff3237204310365eb8945a739bd423668494f786
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422000"
---
# <a name="update-externalitem"></a><span data-ttu-id="d2e45-103">Обновление екстерналитем</span><span class="sxs-lookup"><span data-stu-id="d2e45-103">Update externalitem</span></span>

<span data-ttu-id="d2e45-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d2e45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2e45-105">Обновление свойств объекта [екстерналитем](../resources/externalitem.md) или [екстерналфиле](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="d2e45-105">Update the properties of an [externalitem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="d2e45-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2e45-106">Permissions</span></span>

<span data-ttu-id="d2e45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2e45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2e45-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2e45-109">Permission type</span></span>                        | <span data-ttu-id="d2e45-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2e45-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d2e45-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2e45-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2e45-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2e45-112">Not supported.</span></span> |
| <span data-ttu-id="d2e45-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2e45-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2e45-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2e45-114">Not supported.</span></span> |
| <span data-ttu-id="d2e45-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2e45-115">Application</span></span>                            | <span data-ttu-id="d2e45-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2e45-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2e45-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2e45-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="d2e45-118">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="d2e45-118">Path parameters</span></span>

| <span data-ttu-id="d2e45-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="d2e45-119">Parameter</span></span>     | <span data-ttu-id="d2e45-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d2e45-120">Type</span></span>   | <span data-ttu-id="d2e45-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d2e45-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="d2e45-122">ИД подключения</span><span class="sxs-lookup"><span data-stu-id="d2e45-122">connection-id</span></span> | <span data-ttu-id="d2e45-123">строка</span><span class="sxs-lookup"><span data-stu-id="d2e45-123">string</span></span> | <span data-ttu-id="d2e45-124">`id` Свойство содержащего [екстерналконнектион](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="d2e45-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="d2e45-125">item-id</span><span class="sxs-lookup"><span data-stu-id="d2e45-125">item-id</span></span>       | <span data-ttu-id="d2e45-126">строка</span><span class="sxs-lookup"><span data-stu-id="d2e45-126">string</span></span> | <span data-ttu-id="d2e45-127">Предоставляемое `id` разработчиком свойство [екстерналитем](../resources/externalitem.md) или [екстерналфиле](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="d2e45-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d2e45-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2e45-128">Request headers</span></span>

| <span data-ttu-id="d2e45-129">Имя</span><span class="sxs-lookup"><span data-stu-id="d2e45-129">Name</span></span>          | <span data-ttu-id="d2e45-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d2e45-130">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="d2e45-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2e45-131">Authorization</span></span> | <span data-ttu-id="d2e45-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2e45-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d2e45-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2e45-134">Content-Type</span></span>  | <span data-ttu-id="d2e45-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2e45-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2e45-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2e45-137">Request body</span></span>

<span data-ttu-id="d2e45-138">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d2e45-138">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d2e45-139">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="d2e45-139">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d2e45-140">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d2e45-140">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="d2e45-141">Могут быть обновлены перечисленные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="d2e45-141">The following properties can be updated.</span></span>

> [!NOTE]
> <span data-ttu-id="d2e45-142">В режиме предварительного просмотра можно `acl` обновить только свойство с помощью patch.</span><span class="sxs-lookup"><span data-stu-id="d2e45-142">During the preview only the `acl` property can be updated via PATCH.</span></span> <span data-ttu-id="d2e45-143">Чтобы обновить другие свойства, используйте [PUT, чтобы перезаписать существующий элемент новым элементом](externalconnection-put-items.md).</span><span class="sxs-lookup"><span data-stu-id="d2e45-143">In order to update other properties, use a [PUT to overwrite the existing item with a new item](externalconnection-put-items.md).</span></span>

### <a name="externalitem-properties"></a><span data-ttu-id="d2e45-144">свойства Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="d2e45-144">externalItem properties</span></span>

| <span data-ttu-id="d2e45-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2e45-145">Property</span></span> | <span data-ttu-id="d2e45-146">Тип</span><span class="sxs-lookup"><span data-stu-id="d2e45-146">Type</span></span>                                  | <span data-ttu-id="d2e45-147">Описание</span><span class="sxs-lookup"><span data-stu-id="d2e45-147">Description</span></span>               |
|:---------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="d2e45-148">списки</span><span class="sxs-lookup"><span data-stu-id="d2e45-148">acl</span></span>      | <span data-ttu-id="d2e45-149">Коллекция [списков управления доступом](../resources/acl.md)</span><span class="sxs-lookup"><span data-stu-id="d2e45-149">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="d2e45-150">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="d2e45-150">An array of access control entries.</span></span> <span data-ttu-id="d2e45-151">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="d2e45-151">Each entry specifies the access granted to a user or group.</span></span> |

### <a name="externalfile-properties"></a><span data-ttu-id="d2e45-152">свойства Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="d2e45-152">externalFile properties</span></span>

| <span data-ttu-id="d2e45-153">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2e45-153">Property</span></span> | <span data-ttu-id="d2e45-154">Тип</span><span class="sxs-lookup"><span data-stu-id="d2e45-154">Type</span></span>                                  | <span data-ttu-id="d2e45-155">Описание</span><span class="sxs-lookup"><span data-stu-id="d2e45-155">Description</span></span>               |
|:---------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="d2e45-156">списки</span><span class="sxs-lookup"><span data-stu-id="d2e45-156">acl</span></span>      | <span data-ttu-id="d2e45-157">Коллекция [списков управления доступом](../resources/acl.md)</span><span class="sxs-lookup"><span data-stu-id="d2e45-157">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="d2e45-158">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="d2e45-158">An array of access control entries.</span></span> <span data-ttu-id="d2e45-159">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="d2e45-159">Each entry specifies the access granted to a user or group.</span></span> |

## <a name="response"></a><span data-ttu-id="d2e45-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2e45-160">Response</span></span>

<span data-ttu-id="d2e45-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [екстерналитем](../resources/externalitem.md) или [екстерналфиле](../resources/externalfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d2e45-161">If successful, this method returns a `200 OK` response code and an updated [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2e45-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="d2e45-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2e45-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2e45-163">Request</span></span>

<span data-ttu-id="d2e45-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2e45-164">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2e45-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2e45-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_externalitem"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "grant",
      "identitySource": "Azure Active Directory"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="d2e45-166">C#</span><span class="sxs-lookup"><span data-stu-id="d2e45-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2e45-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2e45-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2e45-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2e45-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="d2e45-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2e45-169">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="d2e45-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d2e45-170">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalItem"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "TSP228082938",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "grant",
      "identitySource": "Azure Active Directory"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": "Textual content of the file"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update externalitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
