---
title: Обновление екстерналитем
description: Обновление свойств объекта екстерналитем.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 1135d889142b66e4ce980244a7f3e6020246228c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938641"
---
# <a name="update-externalitem"></a><span data-ttu-id="e7949-103">Обновление екстерналитем</span><span class="sxs-lookup"><span data-stu-id="e7949-103">Update externalitem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7949-104">Обновление свойств объекта [екстерналитем](../resources/externalitem.md) или [екстерналфиле](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="e7949-104">Update the properties of an [externalitem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e7949-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7949-105">Permissions</span></span>

<span data-ttu-id="e7949-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7949-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e7949-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7949-108">Permission type</span></span>                        | <span data-ttu-id="e7949-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7949-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e7949-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7949-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e7949-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7949-111">Not supported.</span></span> |
| <span data-ttu-id="e7949-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7949-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7949-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7949-113">Not supported.</span></span> |
| <span data-ttu-id="e7949-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7949-114">Application</span></span>                            | <span data-ttu-id="e7949-115">Екстерналитем. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e7949-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7949-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7949-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="e7949-117">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="e7949-117">Path parameters</span></span>

| <span data-ttu-id="e7949-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="e7949-118">Parameter</span></span>     | <span data-ttu-id="e7949-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e7949-119">Type</span></span>   | <span data-ttu-id="e7949-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e7949-120">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="e7949-121">ИД подключения</span><span class="sxs-lookup"><span data-stu-id="e7949-121">connection-id</span></span> | <span data-ttu-id="e7949-122">string</span><span class="sxs-lookup"><span data-stu-id="e7949-122">string</span></span> | <span data-ttu-id="e7949-123">`id` Свойство содержащего [екстерналконнектион](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="e7949-123">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="e7949-124">item-id</span><span class="sxs-lookup"><span data-stu-id="e7949-124">item-id</span></span>       | <span data-ttu-id="e7949-125">string</span><span class="sxs-lookup"><span data-stu-id="e7949-125">string</span></span> | <span data-ttu-id="e7949-126">Предоставляемое `id` разработчиком свойство [екстерналитем](../resources/externalitem.md) или [екстерналфиле](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="e7949-126">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e7949-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7949-127">Request headers</span></span>

| <span data-ttu-id="e7949-128">Имя</span><span class="sxs-lookup"><span data-stu-id="e7949-128">Name</span></span>          | <span data-ttu-id="e7949-129">Описание</span><span class="sxs-lookup"><span data-stu-id="e7949-129">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="e7949-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e7949-130">Authorization</span></span> | <span data-ttu-id="e7949-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7949-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e7949-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e7949-133">Content-Type</span></span>  | <span data-ttu-id="e7949-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7949-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7949-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7949-136">Request body</span></span>

<span data-ttu-id="e7949-137">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="e7949-137">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e7949-138">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="e7949-138">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e7949-139">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e7949-139">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="e7949-140">Могут быть обновлены перечисленные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="e7949-140">The following properties can be updated.</span></span>

> [!NOTE]
> <span data-ttu-id="e7949-141">В режиме предварительного просмотра можно `acl` обновить только свойство с помощью patch.</span><span class="sxs-lookup"><span data-stu-id="e7949-141">During the preview only the `acl` property can be updated via PATCH.</span></span> <span data-ttu-id="e7949-142">Чтобы обновить другие свойства, используйте [PUT, чтобы перезаписать существующий элемент новым элементом](externalconnection-put-items.md).</span><span class="sxs-lookup"><span data-stu-id="e7949-142">In order to update other properties, use a [PUT to overwrite the existing item with a new item](externalconnection-put-items.md).</span></span>

### <a name="externalitem-properties"></a><span data-ttu-id="e7949-143">свойства Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="e7949-143">externalItem properties</span></span>

| <span data-ttu-id="e7949-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7949-144">Property</span></span> | <span data-ttu-id="e7949-145">Тип</span><span class="sxs-lookup"><span data-stu-id="e7949-145">Type</span></span>                                  | <span data-ttu-id="e7949-146">Описание</span><span class="sxs-lookup"><span data-stu-id="e7949-146">Description</span></span>               |
|:---------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="e7949-147">списки</span><span class="sxs-lookup"><span data-stu-id="e7949-147">acl</span></span>      | <span data-ttu-id="e7949-148">Коллекция [списков управления доступом](../resources/acl.md)</span><span class="sxs-lookup"><span data-stu-id="e7949-148">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="e7949-149">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="e7949-149">An array of access control entries.</span></span> <span data-ttu-id="e7949-150">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="e7949-150">Each entry specifies the access granted to a user or group.</span></span> |

### <a name="externalfile-properties"></a><span data-ttu-id="e7949-151">свойства Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="e7949-151">externalFile properties</span></span>

| <span data-ttu-id="e7949-152">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7949-152">Property</span></span> | <span data-ttu-id="e7949-153">Тип</span><span class="sxs-lookup"><span data-stu-id="e7949-153">Type</span></span>                                  | <span data-ttu-id="e7949-154">Описание</span><span class="sxs-lookup"><span data-stu-id="e7949-154">Description</span></span>               |
|:---------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="e7949-155">списки</span><span class="sxs-lookup"><span data-stu-id="e7949-155">acl</span></span>      | <span data-ttu-id="e7949-156">Коллекция [списков управления доступом](../resources/acl.md)</span><span class="sxs-lookup"><span data-stu-id="e7949-156">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="e7949-157">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="e7949-157">An array of access control entries.</span></span> <span data-ttu-id="e7949-158">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="e7949-158">Each entry specifies the access granted to a user or group.</span></span> |

## <a name="response"></a><span data-ttu-id="e7949-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7949-159">Response</span></span>

<span data-ttu-id="e7949-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [екстерналитем](../resources/externalitem.md) или [екстерналфиле](../resources/externalfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e7949-160">If successful, this method returns a `200 OK` response code and an updated [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e7949-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="e7949-161">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e7949-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7949-162">Request</span></span>

<span data-ttu-id="e7949-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7949-163">The following is an example of the request.</span></span>
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

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="e7949-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7949-164">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="e7949-165">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e7949-165">The following is an example of the response.</span></span>

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
