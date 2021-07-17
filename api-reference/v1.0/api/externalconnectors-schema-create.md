---
title: Создание схемы
description: Создайте схему для Поиск (Майкрософт) подключения.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 98c4c83ff8a8712905ace9fa80ec4fdae0de7180
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467493"
---
# <a name="create-schema"></a><span data-ttu-id="51f2f-103">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="51f2f-103">Create schema</span></span>
<span data-ttu-id="51f2f-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="51f2f-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="51f2f-105">Создайте новый [объект схемы.](../resources/externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="51f2f-105">Create a new [schema](../resources/externalconnectors-schema.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="51f2f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51f2f-106">Permissions</span></span>
<span data-ttu-id="51f2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51f2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51f2f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51f2f-109">Permission type</span></span>|<span data-ttu-id="51f2f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51f2f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51f2f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51f2f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51f2f-112">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="51f2f-112">Not applicable</span></span>|
|<span data-ttu-id="51f2f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51f2f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51f2f-114">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="51f2f-114">Not applicable</span></span>|
|<span data-ttu-id="51f2f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="51f2f-115">Application</span></span>| <span data-ttu-id="51f2f-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="51f2f-116">ExternalConnection.ReadWrite.OwnedBy</span></span>|

## <a name="http-request"></a><span data-ttu-id="51f2f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51f2f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /external/connections/{id}/schema
```
<span data-ttu-id="51f2f-118">В теле запроса поставляем представление JSON объекта [схемы.](../resources/externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="51f2f-118">In the request body, supply a JSON representation of a [schema](../resources/externalconnectors-schema.md) object.</span></span>

<span data-ttu-id="51f2f-119">При регистрации настраиваемой схемы элементов объект должен иметь свойство, к котором должно быть установлено свойство, `schema` `baseType` и должен содержать `microsoft.graph.externalItem` `properties` его.</span><span class="sxs-lookup"><span data-stu-id="51f2f-119">When registering a custom item schema, the `schema` object MUST have the `baseType` property set to `microsoft.graph.externalItem` and MUST contain the `properties` property.</span></span> <span data-ttu-id="51f2f-120">Объект должен содержать по крайней мере одно свойство, не `properties` более 64.</span><span class="sxs-lookup"><span data-stu-id="51f2f-120">The `properties` object must contain at least one property, up to a maximum of 64.</span></span>

## <a name="response"></a><span data-ttu-id="51f2f-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="51f2f-121">Response</span></span>

<span data-ttu-id="51f2f-122">Если заготка включена в запрос, этот метод возвращает код ответа и URL-адрес в загонах ответа, которые можно использовать для получения состояния `Prefer: respond-async` `202 Accepted` `Location` [операции.](../api/externalconnectors-connectionoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="51f2f-122">With the `Prefer: respond-async` header included in the request, if successful, this method returns a `202 Accepted` response code and a URL in the `Location` response header that can be used to [get the operation status](../api/externalconnectors-connectionoperation-get.md).</span></span>

<span data-ttu-id="51f2f-123">Без заголовка, включенного в запрос, в случае успешного использования этот метод возвращает код ответа и новый объект схемы в `Prefer: respond-async` `201 Created` тексте ответа. [](../resources/externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="51f2f-123">Without the `Prefer: respond-async` header included in the request, if successful, this method returns a `201 Created` response code and a new [schema](../resources/externalconnectors-schema.md) object in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="51f2f-124">Создание схемы — это длительный процесс, склонный к выходу времени шлюза.</span><span class="sxs-lookup"><span data-stu-id="51f2f-124">Creating a schema is a long-running process prone to gateway timeouts.</span></span> <span data-ttu-id="51f2f-125">Рекомендуется использовать `Prefer: respond-async` заготку, чтобы избежать ошибок в периодике.</span><span class="sxs-lookup"><span data-stu-id="51f2f-125">We recommend using the `Prefer: respond-async` header to avoid timeout errors.</span></span>

## <a name="examples"></a><span data-ttu-id="51f2f-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="51f2f-126">Examples</span></span>

### <a name="example-register-custom-schema-asynchronously"></a><span data-ttu-id="51f2f-127">Пример. Регистрация настраиваемой схемы асинхронно</span><span class="sxs-lookup"><span data-stu-id="51f2f-127">Example: Register custom schema asynchronously</span></span>

#### <a name="request"></a><span data-ttu-id="51f2f-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="51f2f-128">Request</span></span>

<span data-ttu-id="51f2f-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51f2f-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51f2f-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="51f2f-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection_async",
  "@odata.type": "microsoft.graph.externalConnectors.schema"
}-->

```http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/schema
Content-type: application/json
Prefer: respond-async

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "ticketTitle",
      "type": "String",
      "isSearchable": "true",
      "isRetrievable": "true",
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": "true",
      "isRetrievable": "true",
      "isSearchable": "false"
    },
    {
      "name": "assignee",
      "type": "String",
      "isRetrievable": "true"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="51f2f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="51f2f-131">Response</span></span>

<span data-ttu-id="51f2f-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="51f2f-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc
```
