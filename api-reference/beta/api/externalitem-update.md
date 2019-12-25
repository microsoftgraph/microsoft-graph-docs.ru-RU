---
title: Обновление екстерналитем
description: Обновление свойств объекта екстерналитем.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 18830968484e9103ab751261293226105fcef112
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869733"
---
# <a name="update-externalitem"></a><span data-ttu-id="8dc7b-103">Обновление екстерналитем</span><span class="sxs-lookup"><span data-stu-id="8dc7b-103">Update externalitem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dc7b-104">Обновление свойств объекта [екстерналитем](../resources/externalitem.md) или [екстерналфиле](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="8dc7b-104">Update the properties of an [externalitem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="8dc7b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8dc7b-105">Permissions</span></span>

<span data-ttu-id="8dc7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dc7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8dc7b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8dc7b-108">Permission type</span></span>                        | <span data-ttu-id="8dc7b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8dc7b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8dc7b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8dc7b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8dc7b-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dc7b-111">Not supported.</span></span> |
| <span data-ttu-id="8dc7b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8dc7b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dc7b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dc7b-113">Not supported.</span></span> |
| <span data-ttu-id="8dc7b-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="8dc7b-114">Application</span></span>                            | <span data-ttu-id="8dc7b-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dc7b-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8dc7b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8dc7b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="8dc7b-117">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="8dc7b-117">Path parameters</span></span>

| <span data-ttu-id="8dc7b-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="8dc7b-118">Parameter</span></span>     | <span data-ttu-id="8dc7b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="8dc7b-119">Type</span></span>   | <span data-ttu-id="8dc7b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8dc7b-120">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="8dc7b-121">ИД подключения</span><span class="sxs-lookup"><span data-stu-id="8dc7b-121">connection-id</span></span> | <span data-ttu-id="8dc7b-122">string</span><span class="sxs-lookup"><span data-stu-id="8dc7b-122">string</span></span> | <span data-ttu-id="8dc7b-123">`id` Свойство содержащего [екстерналконнектион](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="8dc7b-123">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="8dc7b-124">item-id</span><span class="sxs-lookup"><span data-stu-id="8dc7b-124">item-id</span></span>       | <span data-ttu-id="8dc7b-125">string</span><span class="sxs-lookup"><span data-stu-id="8dc7b-125">string</span></span> | <span data-ttu-id="8dc7b-126">Предоставляемое `id` разработчиком свойство [екстерналитем](../resources/externalitem.md) или [екстерналфиле](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="8dc7b-126">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8dc7b-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8dc7b-127">Request headers</span></span>

| <span data-ttu-id="8dc7b-128">Имя</span><span class="sxs-lookup"><span data-stu-id="8dc7b-128">Name</span></span>          | <span data-ttu-id="8dc7b-129">Описание</span><span class="sxs-lookup"><span data-stu-id="8dc7b-129">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="8dc7b-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8dc7b-130">Authorization</span></span> | <span data-ttu-id="8dc7b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dc7b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8dc7b-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8dc7b-133">Content-Type</span></span>  | <span data-ttu-id="8dc7b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dc7b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8dc7b-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8dc7b-136">Request body</span></span>

<span data-ttu-id="8dc7b-137">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8dc7b-137">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8dc7b-138">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="8dc7b-138">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8dc7b-139">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8dc7b-139">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="8dc7b-140">Могут быть обновлены перечисленные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="8dc7b-140">The following properties can be updated.</span></span>

> [!NOTE]
> <span data-ttu-id="8dc7b-141">В режиме предварительного просмотра можно `acl` обновить только свойство с помощью patch.</span><span class="sxs-lookup"><span data-stu-id="8dc7b-141">During the preview only the `acl` property can be updated via PATCH.</span></span> <span data-ttu-id="8dc7b-142">Чтобы обновить другие свойства, используйте [PUT, чтобы перезаписать существующий элемент новым элементом](externalconnection-put-items.md).</span><span class="sxs-lookup"><span data-stu-id="8dc7b-142">In order to update other properties, use a [PUT to overwrite the existing item with a new item](externalconnection-put-items.md).</span></span>

### <a name="externalitem-properties"></a><span data-ttu-id="8dc7b-143">свойства Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="8dc7b-143">externalItem properties</span></span>

| <span data-ttu-id="8dc7b-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="8dc7b-144">Property</span></span> | <span data-ttu-id="8dc7b-145">Тип</span><span class="sxs-lookup"><span data-stu-id="8dc7b-145">Type</span></span>                                  | <span data-ttu-id="8dc7b-146">Описание</span><span class="sxs-lookup"><span data-stu-id="8dc7b-146">Description</span></span>               |
|:---------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="8dc7b-147">списки</span><span class="sxs-lookup"><span data-stu-id="8dc7b-147">acl</span></span>      | <span data-ttu-id="8dc7b-148">Коллекция [списков управления доступом](../resources/acl.md)</span><span class="sxs-lookup"><span data-stu-id="8dc7b-148">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="8dc7b-149">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="8dc7b-149">An array of access control entries.</span></span> <span data-ttu-id="8dc7b-150">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="8dc7b-150">Each entry specifies the access granted to a user or group.</span></span> |

### <a name="externalfile-properties"></a><span data-ttu-id="8dc7b-151">свойства Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="8dc7b-151">externalFile properties</span></span>

| <span data-ttu-id="8dc7b-152">Свойство</span><span class="sxs-lookup"><span data-stu-id="8dc7b-152">Property</span></span> | <span data-ttu-id="8dc7b-153">Тип</span><span class="sxs-lookup"><span data-stu-id="8dc7b-153">Type</span></span>                                  | <span data-ttu-id="8dc7b-154">Описание</span><span class="sxs-lookup"><span data-stu-id="8dc7b-154">Description</span></span>               |
|:---------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="8dc7b-155">списки</span><span class="sxs-lookup"><span data-stu-id="8dc7b-155">acl</span></span>      | <span data-ttu-id="8dc7b-156">Коллекция [списков управления доступом](../resources/acl.md)</span><span class="sxs-lookup"><span data-stu-id="8dc7b-156">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="8dc7b-157">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="8dc7b-157">An array of access control entries.</span></span> <span data-ttu-id="8dc7b-158">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="8dc7b-158">Each entry specifies the access granted to a user or group.</span></span> |

## <a name="response"></a><span data-ttu-id="8dc7b-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="8dc7b-159">Response</span></span>

<span data-ttu-id="8dc7b-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [екстерналитем](../resources/externalitem.md) или [екстерналфиле](../resources/externalfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8dc7b-160">If successful, this method returns a `200 OK` response code and an updated [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8dc7b-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="8dc7b-161">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8dc7b-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dc7b-162">Request</span></span>

<span data-ttu-id="8dc7b-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dc7b-163">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8dc7b-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="8dc7b-164">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8dc7b-165">C#</span><span class="sxs-lookup"><span data-stu-id="8dc7b-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8dc7b-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8dc7b-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8dc7b-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8dc7b-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="8dc7b-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dc7b-168">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="8dc7b-169">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8dc7b-169">The following is an example of the response.</span></span>

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
