---
title: Добавление соединителя для connectorGroup
description: Используйте этот API, чтобы добавить соединителю в соединителюGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 83829bdcfc3c3bfafe92971c42420f2fb9cf62d8
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786147"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="1337b-103">Добавление соединителя для connectorGroup</span><span class="sxs-lookup"><span data-stu-id="1337b-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="1337b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1337b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1337b-105">Добавьте [соединителю](../resources/connector.md) в [соединителюGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="1337b-105">Add a [connector](../resources/connector.md) to a [connectorGroup](../resources/connectorgroup.md).</span></span>

<span data-ttu-id="1337b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1337b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1337b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1337b-108">Permission type</span></span>      | <span data-ttu-id="1337b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1337b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1337b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1337b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1337b-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1337b-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1337b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1337b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1337b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1337b-113">Not supported.</span></span>    |
|<span data-ttu-id="1337b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1337b-114">Application</span></span> | <span data-ttu-id="1337b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1337b-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1337b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1337b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="1337b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1337b-117">Request headers</span></span>
| <span data-ttu-id="1337b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1337b-118">Name</span></span>       | <span data-ttu-id="1337b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1337b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1337b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1337b-120">Authorization</span></span>  | <span data-ttu-id="1337b-121">Носителер.</span><span class="sxs-lookup"><span data-stu-id="1337b-121">Bearer.</span></span> <span data-ttu-id="1337b-122">Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="1337b-122">Required.</span></span>|
| <span data-ttu-id="1337b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1337b-123">Content-type</span></span> | <span data-ttu-id="1337b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1337b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1337b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1337b-126">Request body</span></span>
<span data-ttu-id="1337b-127">В теле запроса поставляем представление JSON ссылки на [объект соединитель.](../resources/connector.md)</span><span class="sxs-lookup"><span data-stu-id="1337b-127">In the request body, supply a JSON representation of a link to a [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1337b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1337b-128">Response</span></span>

<span data-ttu-id="1337b-129">В случае успешной работы этот метод возвращает код отклика и `201 Created` объект [соединители](../resources/connector.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1337b-129">If successful, this method returns a `201 Created` response code and a [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1337b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1337b-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="1337b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1337b-131">Request</span></span>
<span data-ttu-id="1337b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1337b-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1337b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1337b-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1337b-134">C#</span><span class="sxs-lookup"><span data-stu-id="1337b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connector-from-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1337b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1337b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connector-from-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1337b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1337b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connector-from-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1337b-137">Java</span><span class="sxs-lookup"><span data-stu-id="1337b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connector-from-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="1337b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1337b-138">Response</span></span>
<span data-ttu-id="1337b-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1337b-139">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response"
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



