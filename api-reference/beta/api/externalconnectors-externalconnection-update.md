---
title: Обновление externalConnection
description: Обновление свойств externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 8b14abf1a010b8d28e80308077bcc5aa2f72eecf
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467690"
---
# <a name="update-connection"></a><span data-ttu-id="ba51b-103">Обновление подключения</span><span class="sxs-lookup"><span data-stu-id="ba51b-103">Update connection</span></span>

<span data-ttu-id="ba51b-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="ba51b-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba51b-105">Обновление свойств [externalConnection](../resources/externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="ba51b-105">Update the properties of an [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ba51b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba51b-106">Permissions</span></span>

<span data-ttu-id="ba51b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba51b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba51b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba51b-109">Permission type</span></span>                        | <span data-ttu-id="ba51b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba51b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ba51b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba51b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba51b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba51b-112">Not supported.</span></span> |
| <span data-ttu-id="ba51b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba51b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba51b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba51b-114">Not supported.</span></span> |
| <span data-ttu-id="ba51b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ba51b-115">Application</span></span>                            | <span data-ttu-id="ba51b-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="ba51b-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba51b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba51b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ba51b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba51b-118">Request headers</span></span>

| <span data-ttu-id="ba51b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ba51b-119">Name</span></span>          | <span data-ttu-id="ba51b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ba51b-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="ba51b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba51b-121">Authorization</span></span> | <span data-ttu-id="ba51b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba51b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="ba51b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba51b-124">Content-Type</span></span>  | <span data-ttu-id="ba51b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba51b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba51b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba51b-127">Request body</span></span>

<span data-ttu-id="ba51b-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="ba51b-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ba51b-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="ba51b-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ba51b-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ba51b-130">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="ba51b-131">Могут быть обновлены перечисленные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="ba51b-131">The following properties can be updated.</span></span>

| <span data-ttu-id="ba51b-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba51b-132">Property</span></span>      | <span data-ttu-id="ba51b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="ba51b-133">Type</span></span>                                           | <span data-ttu-id="ba51b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ba51b-134">Description</span></span> |
|:--------------|:-----------------------------------------------|:------------|
| <span data-ttu-id="ba51b-135">configuration</span><span class="sxs-lookup"><span data-stu-id="ba51b-135">configuration</span></span> | [<span data-ttu-id="ba51b-136">microsoft.graph.externalConnectors.configuration</span><span class="sxs-lookup"><span data-stu-id="ba51b-136">microsoft.graph.externalConnectors.configuration</span></span>](../resources/externalconnectors-configuration.md) | <span data-ttu-id="ba51b-137">Указывает дополнительные ID-адреса приложений, которые разрешены для управления подключением и индексации контента в подключении.</span><span class="sxs-lookup"><span data-stu-id="ba51b-137">Specifies additional application IDs that are allowed to manage the connection and to index content in the connection.</span></span> |
| <span data-ttu-id="ba51b-138">description</span><span class="sxs-lookup"><span data-stu-id="ba51b-138">description</span></span>   | <span data-ttu-id="ba51b-139">String</span><span class="sxs-lookup"><span data-stu-id="ba51b-139">String</span></span>                                         | <span data-ttu-id="ba51b-140">Описание подключения, отображаемого в Центр администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ba51b-140">Description of the connection displayed in the Microsoft 365 admin center.</span></span> |
| <span data-ttu-id="ba51b-141">name</span><span class="sxs-lookup"><span data-stu-id="ba51b-141">name</span></span>          | <span data-ttu-id="ba51b-142">String</span><span class="sxs-lookup"><span data-stu-id="ba51b-142">String</span></span>                                         | <span data-ttu-id="ba51b-143">Отображает имя подключения, отображаемого в Центр администрирования Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ba51b-143">The display name of the connection to be displayed in the Microsoft 365 admin center.</span></span> <span data-ttu-id="ba51b-144">Максимальная длина 128 символов.</span><span class="sxs-lookup"><span data-stu-id="ba51b-144">Maximum length of 128 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="ba51b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba51b-145">Response</span></span>

<span data-ttu-id="ba51b-146">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ba51b-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ba51b-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="ba51b-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba51b-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba51b-148">Request</span></span>

<span data-ttu-id="ba51b-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba51b-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ba51b-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba51b-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connection",
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr
Content-type: application/json

{
  "name": "Contoso HR Service Tickets",
  "description": "Connection to index HR service tickets"
}
```
# <a name="c"></a>[<span data-ttu-id="ba51b-151">C#</span><span class="sxs-lookup"><span data-stu-id="ba51b-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba51b-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba51b-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba51b-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba51b-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba51b-154">Java</span><span class="sxs-lookup"><span data-stu-id="ba51b-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="ba51b-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba51b-155">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="ba51b-156">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ba51b-156">The following is an example of the response.</span></span>

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
