---
title: Обновление externalItem
description: Обновление свойств объекта externalItem.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 10c59c40dd5ae889469b00b708b852326a2fd0e8
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467494"
---
# <a name="update-externalitem"></a><span data-ttu-id="07cdb-103">Обновление externalItem</span><span class="sxs-lookup"><span data-stu-id="07cdb-103">Update externalItem</span></span>
<span data-ttu-id="07cdb-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="07cdb-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="07cdb-105">Обновление свойств объекта [externalItem.](../resources/externalconnectors-externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="07cdb-105">Update the properties of an [externalItem](../resources/externalconnectors-externalitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="07cdb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07cdb-106">Permissions</span></span>
<span data-ttu-id="07cdb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07cdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07cdb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07cdb-109">Permission type</span></span>|<span data-ttu-id="07cdb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07cdb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07cdb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07cdb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="07cdb-112">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="07cdb-112">Not applicable</span></span>|
|<span data-ttu-id="07cdb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07cdb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07cdb-114">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="07cdb-114">Not applicable</span></span>|
|<span data-ttu-id="07cdb-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="07cdb-115">Application</span></span>| <span data-ttu-id="07cdb-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07cdb-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07cdb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07cdb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="07cdb-118">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="07cdb-118">Path parameters</span></span>

| <span data-ttu-id="07cdb-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="07cdb-119">Parameter</span></span>     | <span data-ttu-id="07cdb-120">Тип</span><span class="sxs-lookup"><span data-stu-id="07cdb-120">Type</span></span>   | <span data-ttu-id="07cdb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="07cdb-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="07cdb-122">connection-id</span><span class="sxs-lookup"><span data-stu-id="07cdb-122">connection-id</span></span> | <span data-ttu-id="07cdb-123">String</span><span class="sxs-lookup"><span data-stu-id="07cdb-123">string</span></span> | <span data-ttu-id="07cdb-124">`id`Свойствосодержащего [externalConnection](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="07cdb-124">The `id` property of the containing [externalConnection](../resources/externalconnectors-externalconnection.md)</span></span> |
| <span data-ttu-id="07cdb-125">item-id</span><span class="sxs-lookup"><span data-stu-id="07cdb-125">item-id</span></span>       | <span data-ttu-id="07cdb-126">String</span><span class="sxs-lookup"><span data-stu-id="07cdb-126">string</span></span> | <span data-ttu-id="07cdb-127">Свойство `id` [externalItem,](../resources/externalconnectors-externalitem.md)предоставленное разработчиком.</span><span class="sxs-lookup"><span data-stu-id="07cdb-127">The developer-provided `id` property of the [externalItem](../resources/externalconnectors-externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="07cdb-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07cdb-128">Request headers</span></span>

| <span data-ttu-id="07cdb-129">Имя</span><span class="sxs-lookup"><span data-stu-id="07cdb-129">Name</span></span>          | <span data-ttu-id="07cdb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="07cdb-130">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="07cdb-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07cdb-131">Authorization</span></span> | <span data-ttu-id="07cdb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07cdb-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="07cdb-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="07cdb-134">Content-Type</span></span>  | <span data-ttu-id="07cdb-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07cdb-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07cdb-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07cdb-137">Request body</span></span>

<span data-ttu-id="07cdb-138">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="07cdb-138">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="07cdb-139">Существующие свойства (за исключением свойств внутри объекта), не включенные в тело запроса, будут поддерживать прежние значения или пересчитываться на основе изменений других `properties` значений свойств.</span><span class="sxs-lookup"><span data-stu-id="07cdb-139">Existing properties (excluding properties inside the `properties` object) that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="07cdb-140">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="07cdb-140">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="07cdb-141">Могут быть обновлены перечисленные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="07cdb-141">The following properties can be updated.</span></span>

| <span data-ttu-id="07cdb-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="07cdb-142">Property</span></span>   | <span data-ttu-id="07cdb-143">Тип</span><span class="sxs-lookup"><span data-stu-id="07cdb-143">Type</span></span>                                  | <span data-ttu-id="07cdb-144">Описание</span><span class="sxs-lookup"><span data-stu-id="07cdb-144">Description</span></span>               |
|:-----------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="07cdb-145">acl</span><span class="sxs-lookup"><span data-stu-id="07cdb-145">acl</span></span>        | <span data-ttu-id="07cdb-146">[коллекция microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md)</span><span class="sxs-lookup"><span data-stu-id="07cdb-146">[microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md) collection</span></span> | <span data-ttu-id="07cdb-147">Массив записей управления доступом.</span><span class="sxs-lookup"><span data-stu-id="07cdb-147">An array of access control entries.</span></span> <span data-ttu-id="07cdb-148">Каждая запись указывает доступ, предоставленный пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="07cdb-148">Each entry specifies the access granted to a user or group.</span></span> |
| <span data-ttu-id="07cdb-149">содержимое</span><span class="sxs-lookup"><span data-stu-id="07cdb-149">content</span></span>    | [<span data-ttu-id="07cdb-150">microsoft.graph.externalConnectors.externalItemContent</span><span class="sxs-lookup"><span data-stu-id="07cdb-150">microsoft.graph.externalConnectors.externalItemContent</span></span>](../resources/externalconnectors-externalitemcontent.md) | <span data-ttu-id="07cdb-151">Простое текстовое представление содержимого элемента.</span><span class="sxs-lookup"><span data-stu-id="07cdb-151">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="07cdb-152">Текст в этом свойстве индексироваться с полным текстом.</span><span class="sxs-lookup"><span data-stu-id="07cdb-152">The text in this property is full-text indexed.</span></span> |
| <span data-ttu-id="07cdb-153">properties</span><span class="sxs-lookup"><span data-stu-id="07cdb-153">properties</span></span> | <span data-ttu-id="07cdb-154">Объект</span><span class="sxs-lookup"><span data-stu-id="07cdb-154">Object</span></span>                              | <span data-ttu-id="07cdb-155">Пакет свойств со свойствами элемента.</span><span class="sxs-lookup"><span data-stu-id="07cdb-155">A property bag with the properties of the item.</span></span> <span data-ttu-id="07cdb-156">Свойства должны соответствовать [схеме,](../resources/externalconnectors-schema.md) определенной для [externalConnection.](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="07cdb-156">The properties MUST conform to the [schema](../resources/externalconnectors-schema.md) defined for the [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span> |

### <a name="updating-the-acl-collection"></a><span data-ttu-id="07cdb-157">Обновление коллекции acl</span><span class="sxs-lookup"><span data-stu-id="07cdb-157">Updating the acl collection</span></span>

<span data-ttu-id="07cdb-158">Если свойство включено в запрос на обновление, существующая коллекция ACL перезаписывается с коллекцией, `acl` включенной в запрос.</span><span class="sxs-lookup"><span data-stu-id="07cdb-158">If the `acl` property is included in an update request, the existing ACL collection is overwritten with the collection included in the request.</span></span>

### <a name="updating-the-properties-object"></a><span data-ttu-id="07cdb-159">Обновление объекта свойств</span><span class="sxs-lookup"><span data-stu-id="07cdb-159">Updating the properties object</span></span>

<span data-ttu-id="07cdb-160">Если свойство включено в запрос на обновление, существующий пакет свойств перезаписывается со значением, `properties` включенным в запрос.</span><span class="sxs-lookup"><span data-stu-id="07cdb-160">If the `properties` property is included in an update request, the existing property bag is overwritten with the value included in the request.</span></span>

## <a name="response"></a><span data-ttu-id="07cdb-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="07cdb-161">Response</span></span>

<span data-ttu-id="07cdb-162">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект externalItem](../resources/externalconnectors-externalitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="07cdb-162">If successful, this method returns a `200 OK` response code and an updated [externalItem](../resources/externalconnectors-externalitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="07cdb-163">Примеры</span><span class="sxs-lookup"><span data-stu-id="07cdb-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="07cdb-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="07cdb-164">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_externalitem",
  "@odata.type": "microsoft.graph.externalConnectors.externalItem"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/connections/contosohr/items/TSP228082938
Content-Type: application/json
Content-length: 360

{
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant"
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="07cdb-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="07cdb-165">Response</span></span>
<span data-ttu-id="07cdb-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="07cdb-166">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalItem"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "TSP228082938",
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "@odata.type": "microsoft.graph.externalConnectors.externalItemContent",
    "value": "<h1>Error in payment gateway</h1><p>Error details...</p>",
    "type": "html"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update externalitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: update_externalitem/properties:\r\n      Referenced type microsoft.graph.object is not defined in the doc set! Potential suggestion: microsoft.graph.directoryObject"
  ]
}-->