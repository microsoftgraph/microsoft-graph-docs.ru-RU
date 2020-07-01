---
title: Добавление соединителя в Коннекторграуп
description: Используйте этот API, чтобы добавить соединитель в Коннекторграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4df3f5a1b721528e1a72a0b5970f5577d6cf5696
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006879"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="fee96-103">Добавление соединителя в Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="fee96-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="fee96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fee96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fee96-105">Добавление [соединителя](../resources/connector.md) в [коннекторграуп](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="fee96-105">Add a [connector](../resources/connector.md) to a [connectorGroup](../resources/connectorgroup.md).</span></span>

<span data-ttu-id="fee96-106">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="fee96-106">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fee96-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fee96-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fee96-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fee96-108">Permission type</span></span>      | <span data-ttu-id="fee96-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fee96-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fee96-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fee96-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fee96-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fee96-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fee96-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fee96-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fee96-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fee96-113">Not supported.</span></span>    |
|<span data-ttu-id="fee96-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fee96-114">Application</span></span> | <span data-ttu-id="fee96-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fee96-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="fee96-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fee96-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="fee96-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fee96-117">Request headers</span></span>
| <span data-ttu-id="fee96-118">Имя</span><span class="sxs-lookup"><span data-stu-id="fee96-118">Name</span></span>       | <span data-ttu-id="fee96-119">Описание</span><span class="sxs-lookup"><span data-stu-id="fee96-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fee96-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fee96-120">Authorization</span></span>  | <span data-ttu-id="fee96-121">Носителя.</span><span class="sxs-lookup"><span data-stu-id="fee96-121">Bearer.</span></span> <span data-ttu-id="fee96-122">Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="fee96-122">Required.</span></span>|
| <span data-ttu-id="fee96-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fee96-123">Content-type</span></span> | <span data-ttu-id="fee96-124">application/json.</span><span class="sxs-lookup"><span data-stu-id="fee96-124">application/json.</span></span> <span data-ttu-id="fee96-125">Required.</span><span class="sxs-lookup"><span data-stu-id="fee96-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fee96-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fee96-126">Request body</span></span>
<span data-ttu-id="fee96-127">В тексте запроса добавьте представление ссылки на объект [Connector](../resources/connector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fee96-127">In the request body, supply a JSON representation of a link to a [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fee96-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fee96-128">Response</span></span>

<span data-ttu-id="fee96-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Connector](../resources/connector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fee96-129">If successful, this method returns a `201 Created` response code and a [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fee96-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fee96-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="fee96-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fee96-131">Request</span></span>
<span data-ttu-id="fee96-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fee96-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fee96-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fee96-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fee96-134">C#</span><span class="sxs-lookup"><span data-stu-id="fee96-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connector-from-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fee96-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fee96-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connector-from-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fee96-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fee96-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connector-from-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="fee96-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fee96-137">Response</span></span>
<span data-ttu-id="fee96-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fee96-138">The following is an example of the response.</span></span> 

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
