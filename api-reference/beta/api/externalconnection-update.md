---
title: Обновление Екстерналконнектион
description: Обновление свойств объекта Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7e2b6418c9dcbdc89fc7701302ddf28a780cb6d0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954677"
---
# <a name="update-connection"></a><span data-ttu-id="dd094-103">Обновление подключения</span><span class="sxs-lookup"><span data-stu-id="dd094-103">Update connection</span></span>

<span data-ttu-id="dd094-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd094-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd094-105">Обновление свойств объекта [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="dd094-105">Update the properties of an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="dd094-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd094-106">Permissions</span></span>

<span data-ttu-id="dd094-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd094-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd094-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd094-109">Permission type</span></span>                        | <span data-ttu-id="dd094-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd094-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dd094-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd094-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd094-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd094-112">Not supported.</span></span> |
| <span data-ttu-id="dd094-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd094-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd094-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd094-114">Not supported.</span></span> |
| <span data-ttu-id="dd094-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd094-115">Application</span></span>                            | <span data-ttu-id="dd094-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd094-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd094-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd094-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dd094-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd094-118">Request headers</span></span>

| <span data-ttu-id="dd094-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dd094-119">Name</span></span>          | <span data-ttu-id="dd094-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dd094-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="dd094-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd094-121">Authorization</span></span> | <span data-ttu-id="dd094-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd094-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="dd094-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd094-124">Content-Type</span></span>  | <span data-ttu-id="dd094-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd094-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd094-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd094-127">Request body</span></span>

<span data-ttu-id="dd094-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="dd094-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="dd094-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="dd094-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="dd094-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="dd094-130">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="dd094-131">Могут быть обновлены перечисленные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="dd094-131">The following properties can be updated.</span></span>

| <span data-ttu-id="dd094-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd094-132">Property</span></span>      | <span data-ttu-id="dd094-133">Тип</span><span class="sxs-lookup"><span data-stu-id="dd094-133">Type</span></span>                                           | <span data-ttu-id="dd094-134">Описание</span><span class="sxs-lookup"><span data-stu-id="dd094-134">Description</span></span> |
|:--------------|:-----------------------------------------------|:------------|
| <span data-ttu-id="dd094-135">configuration</span><span class="sxs-lookup"><span data-stu-id="dd094-135">configuration</span></span> | [<span data-ttu-id="dd094-136">configuration</span><span class="sxs-lookup"><span data-stu-id="dd094-136">configuration</span></span>](../resources/configuration.md) | <span data-ttu-id="dd094-137">Задает дополнительные идентификаторы приложений, которым разрешено управлять подключением и индексировать содержимое в подключении.</span><span class="sxs-lookup"><span data-stu-id="dd094-137">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> |
| <span data-ttu-id="dd094-138">description</span><span class="sxs-lookup"><span data-stu-id="dd094-138">description</span></span>   | <span data-ttu-id="dd094-139">String</span><span class="sxs-lookup"><span data-stu-id="dd094-139">String</span></span>                                         | <span data-ttu-id="dd094-140">Описание подключения, отображаемое в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="dd094-140">Description of the connection displayed in the Microsoft 365 admin center.</span></span> |
| <span data-ttu-id="dd094-141">name</span><span class="sxs-lookup"><span data-stu-id="dd094-141">name</span></span>          | <span data-ttu-id="dd094-142">String</span><span class="sxs-lookup"><span data-stu-id="dd094-142">String</span></span>                                         | <span data-ttu-id="dd094-143">Отображаемое имя подключения, отображаемое в центре администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="dd094-143">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="dd094-144">Максимальная длина 128 символов.</span><span class="sxs-lookup"><span data-stu-id="dd094-144">Maximum length of 128 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="dd094-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd094-145">Response</span></span>

<span data-ttu-id="dd094-146">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dd094-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="dd094-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="dd094-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dd094-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd094-148">Request</span></span>

<span data-ttu-id="dd094-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd094-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd094-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd094-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connection"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr
Content-type: application/json

{
  "name": "Contoso HR Service Tickets",
  "description": "Connection to index HR service tickets"
}
```
# <a name="c"></a>[<span data-ttu-id="dd094-151">C#</span><span class="sxs-lookup"><span data-stu-id="dd094-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd094-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd094-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd094-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd094-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd094-154">Java</span><span class="sxs-lookup"><span data-stu-id="dd094-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="dd094-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd094-155">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="dd094-156">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dd094-156">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update connection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


