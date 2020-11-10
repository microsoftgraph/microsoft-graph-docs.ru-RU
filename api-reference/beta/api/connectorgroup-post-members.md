---
title: Добавление соединителя для connectorGroup
description: Используйте этот API, чтобы добавить соединитель в Коннекторграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7a64d86563456f0d5fb9152715d88657a11d6016
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957310"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="99e05-103">Добавление соединителя для connectorGroup</span><span class="sxs-lookup"><span data-stu-id="99e05-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="99e05-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99e05-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99e05-105">Добавление [соединителя](../resources/connector.md) в [коннекторграуп](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="99e05-105">Add a [connector](../resources/connector.md) to a [connectorGroup](../resources/connectorgroup.md).</span></span>

<span data-ttu-id="99e05-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99e05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99e05-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99e05-108">Permission type</span></span>      | <span data-ttu-id="99e05-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99e05-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99e05-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99e05-110">Delegated (work or school account)</span></span> | <span data-ttu-id="99e05-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="99e05-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="99e05-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99e05-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99e05-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99e05-113">Not supported.</span></span>    |
|<span data-ttu-id="99e05-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99e05-114">Application</span></span> | <span data-ttu-id="99e05-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99e05-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="99e05-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99e05-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="99e05-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99e05-117">Request headers</span></span>
| <span data-ttu-id="99e05-118">Имя</span><span class="sxs-lookup"><span data-stu-id="99e05-118">Name</span></span>       | <span data-ttu-id="99e05-119">Описание</span><span class="sxs-lookup"><span data-stu-id="99e05-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="99e05-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="99e05-120">Authorization</span></span>  | <span data-ttu-id="99e05-121">Носителя.</span><span class="sxs-lookup"><span data-stu-id="99e05-121">Bearer.</span></span> <span data-ttu-id="99e05-122">Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="99e05-122">Required.</span></span>|
| <span data-ttu-id="99e05-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="99e05-123">Content-type</span></span> | <span data-ttu-id="99e05-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99e05-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99e05-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99e05-126">Request body</span></span>
<span data-ttu-id="99e05-127">В тексте запроса добавьте представление ссылки на объект [Connector](../resources/connector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99e05-127">In the request body, supply a JSON representation of a link to a [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="99e05-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="99e05-128">Response</span></span>

<span data-ttu-id="99e05-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Connector](../resources/connector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="99e05-129">If successful, this method returns a `201 Created` response code and a [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99e05-130">Пример</span><span class="sxs-lookup"><span data-stu-id="99e05-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="99e05-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="99e05-131">Request</span></span>
<span data-ttu-id="99e05-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99e05-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="99e05-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="99e05-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_connector_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref
Content-type: application/json
Content-length: 104

{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="99e05-134">C#</span><span class="sxs-lookup"><span data-stu-id="99e05-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connector-from-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99e05-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99e05-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connector-from-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99e05-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99e05-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connector-from-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99e05-137">Java</span><span class="sxs-lookup"><span data-stu-id="99e05-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connector-from-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="99e05-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="99e05-138">Response</span></span>
<span data-ttu-id="99e05-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="99e05-139">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add connector to connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


