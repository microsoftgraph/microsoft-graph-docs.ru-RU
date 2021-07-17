---
title: Создание externalItem
description: Создание нового externalItem.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: eba04bf339eeed41f9fe59831773d413bbed3111
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467438"
---
# <a name="create-externalitem"></a><span data-ttu-id="c4a4e-103">Создание externalItem</span><span class="sxs-lookup"><span data-stu-id="c4a4e-103">Create externalItem</span></span>

<span data-ttu-id="c4a4e-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="c4a4e-104">Namespace: microsoft.graph.externalConnectors</span></span>

<span data-ttu-id="c4a4e-105">Создайте [новый объект externalItem.](../resources/externalconnectors-externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="c4a4e-105">Create a new [externalItem](../resources/externalconnectors-externalitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4a4e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4a4e-106">Permissions</span></span>
<span data-ttu-id="c4a4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4a4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4a4e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4a4e-109">Permission type</span></span>|<span data-ttu-id="c4a4e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4a4e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4a4e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4a4e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c4a4e-112">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="c4a4e-112">Not applicable</span></span>|
|<span data-ttu-id="c4a4e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4a4e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4a4e-114">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="c4a4e-114">Not applicable</span></span>|
|<span data-ttu-id="c4a4e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c4a4e-115">Application</span></span>| <span data-ttu-id="c4a4e-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4a4e-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4a4e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4a4e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /connections/{connectionsId}/items
```

## <a name="request-headers"></a><span data-ttu-id="c4a4e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4a4e-118">Request headers</span></span>
|<span data-ttu-id="c4a4e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c4a4e-119">Name</span></span>|<span data-ttu-id="c4a4e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c4a4e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c4a4e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4a4e-121">Authorization</span></span>|<span data-ttu-id="c4a4e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4a4e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c4a4e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4a4e-124">Content-Type</span></span>|<span data-ttu-id="c4a4e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4a4e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4a4e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4a4e-127">Request body</span></span>
<span data-ttu-id="c4a4e-128">В теле запроса поставляют представление JSON объекта [externalItem.](../resources/externalconnectors-externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="c4a4e-128">In the request body, supply a JSON representation of the [externalItem](../resources/externalconnectors-externalitem.md) object.</span></span>

<span data-ttu-id="c4a4e-129">В следующей таблице показаны свойства, необходимые при создании [externalItem.](../resources/externalconnectors-externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="c4a4e-129">The following table shows the properties that are required when you create the [externalItem](../resources/externalconnectors-externalitem.md).</span></span>

|<span data-ttu-id="c4a4e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4a4e-130">Property</span></span>|<span data-ttu-id="c4a4e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c4a4e-131">Type</span></span>| <span data-ttu-id="c4a4e-132">Обязательно (Y/N)</span><span class="sxs-lookup"><span data-stu-id="c4a4e-132">Required (Y/N)</span></span> | <span data-ttu-id="c4a4e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c4a4e-133">Description</span></span>|
|:---|:---|:---|:---|
|<span data-ttu-id="c4a4e-134">id</span><span class="sxs-lookup"><span data-stu-id="c4a4e-134">id</span></span>|<span data-ttu-id="c4a4e-135">String</span><span class="sxs-lookup"><span data-stu-id="c4a4e-135">String</span></span>|<span data-ttu-id="c4a4e-136">Да</span><span class="sxs-lookup"><span data-stu-id="c4a4e-136">Y</span></span>|<span data-ttu-id="c4a4e-137">ID элемента</span><span class="sxs-lookup"><span data-stu-id="c4a4e-137">The item ID</span></span>|
|<span data-ttu-id="c4a4e-138">properties</span><span class="sxs-lookup"><span data-stu-id="c4a4e-138">properties</span></span>|[<span data-ttu-id="c4a4e-139">microsoft.graph.externalConnectors.properties</span><span class="sxs-lookup"><span data-stu-id="c4a4e-139">microsoft.graph.externalConnectors.properties</span></span>](../resources/externalconnectors-properties.md)|<span data-ttu-id="c4a4e-140">Да</span><span class="sxs-lookup"><span data-stu-id="c4a4e-140">Y</span></span>|<span data-ttu-id="c4a4e-141">Свойства элемента.</span><span class="sxs-lookup"><span data-stu-id="c4a4e-141">The item properties.</span></span> <span data-ttu-id="c4a4e-142">Объект `properties` должен содержать по крайней мере одно свойство.</span><span class="sxs-lookup"><span data-stu-id="c4a4e-142">The `properties` object must contain at least one property.</span></span> <span data-ttu-id="c4a4e-143">Все `DateTime` свойства типа должны быть в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="c4a4e-143">All `DateTime` type properties must be in ISO 8601 format.</span></span>|
|<span data-ttu-id="c4a4e-144">содержимое</span><span class="sxs-lookup"><span data-stu-id="c4a4e-144">content</span></span>|[<span data-ttu-id="c4a4e-145">microsoft.graph.externalConnectors.externalItemContent</span><span class="sxs-lookup"><span data-stu-id="c4a4e-145">microsoft.graph.externalConnectors.externalItemContent</span></span>](../resources/externalconnectors-externalitemcontent.md)|<span data-ttu-id="c4a4e-146">Нет</span><span class="sxs-lookup"><span data-stu-id="c4a4e-146">N</span></span>|<span data-ttu-id="c4a4e-147">Внешний контент элемента</span><span class="sxs-lookup"><span data-stu-id="c4a4e-147">The external item content</span></span>|
|<span data-ttu-id="c4a4e-148">acl</span><span class="sxs-lookup"><span data-stu-id="c4a4e-148">acl</span></span>|<span data-ttu-id="c4a4e-149">[коллекция microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md)</span><span class="sxs-lookup"><span data-stu-id="c4a4e-149">[microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md) collection</span></span>|<span data-ttu-id="c4a4e-150">Да</span><span class="sxs-lookup"><span data-stu-id="c4a4e-150">Y</span></span>|<span data-ttu-id="c4a4e-151">Список управления доступом</span><span class="sxs-lookup"><span data-stu-id="c4a4e-151">The access control list</span></span>|

<span data-ttu-id="c4a4e-152">Свойства на объекте должны использовать указанные типы в полезной `externalItem` нагрузке в следующих сценариях:</span><span class="sxs-lookup"><span data-stu-id="c4a4e-152">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="c4a4e-153">Для `String` свойств типа, если значение содержит символы, не относимые к ASCII.</span><span class="sxs-lookup"><span data-stu-id="c4a4e-153">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="c4a4e-154">Для всех типов коллекций.</span><span class="sxs-lookup"><span data-stu-id="c4a4e-154">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="c4a4e-155">При включаем свойстве типа `Collection(DateTime)` необходимо использовать указанный `Collection(DateTimeOffset)` тип.</span><span class="sxs-lookup"><span data-stu-id="c4a4e-155">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

## <a name="response"></a><span data-ttu-id="c4a4e-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4a4e-156">Response</span></span> 

<span data-ttu-id="c4a4e-157">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="c4a4e-157">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c4a4e-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="c4a4e-158">Examples</span></span>

### <a name="example-create-a-custom-item"></a><span data-ttu-id="c4a4e-159">Пример: Создание настраиваемой номенклатуры</span><span class="sxs-lookup"><span data-stu-id="c4a4e-159">Example: Create a custom item</span></span>

### <a name="request"></a><span data-ttu-id="c4a4e-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4a4e-160">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_externalConnections"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "acl": [
    {
      "type": "user",
      "value": "e811976d-83df-4cbd-8b9b-5215b18aa874",
      "accessType": "grant"
    },
    {
      "type": "externalGroup",
      "value": "14m1b9c38qe647f6a",
      "accessType": "deny"
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


### <a name="response"></a><span data-ttu-id="c4a4e-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4a4e-161">Response</span></span>

<span data-ttu-id="c4a4e-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c4a4e-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

