---
title: Создание memberOf
description: Используйте этот API для создания нового memberOf.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b8919fb0a9513d2278d07a73cf1dc95327fdc983
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055514"
---
# <a name="create-memberof"></a><span data-ttu-id="fba31-103">Создание memberOf</span><span class="sxs-lookup"><span data-stu-id="fba31-103">Create memberOf</span></span>

<span data-ttu-id="fba31-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fba31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fba31-105">Используйте этот API для создания нового memberOf.</span><span class="sxs-lookup"><span data-stu-id="fba31-105">Use this API to create a new memberOf.</span></span>
## <a name="permissions"></a><span data-ttu-id="fba31-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fba31-106">Permissions</span></span>
<span data-ttu-id="fba31-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fba31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fba31-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fba31-109">Permission type</span></span>      | <span data-ttu-id="fba31-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fba31-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fba31-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fba31-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fba31-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fba31-112">Not supported.</span></span>    |
|<span data-ttu-id="fba31-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fba31-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fba31-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fba31-114">Not supported.</span></span>    |
|<span data-ttu-id="fba31-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fba31-115">Application</span></span> | <span data-ttu-id="fba31-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fba31-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fba31-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fba31-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="fba31-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fba31-118">Request headers</span></span>
| <span data-ttu-id="fba31-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fba31-119">Name</span></span>       | <span data-ttu-id="fba31-120">Тип</span><span class="sxs-lookup"><span data-stu-id="fba31-120">Type</span></span> | <span data-ttu-id="fba31-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fba31-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fba31-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fba31-122">Authorization</span></span>  | <span data-ttu-id="fba31-123">string</span><span class="sxs-lookup"><span data-stu-id="fba31-123">string</span></span>  | <span data-ttu-id="fba31-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fba31-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fba31-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fba31-126">Request body</span></span>
<span data-ttu-id="fba31-127">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fba31-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fba31-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fba31-128">Response</span></span>

<span data-ttu-id="fba31-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fba31-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fba31-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fba31-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fba31-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fba31-131">Request</span></span>
<span data-ttu-id="fba31-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fba31-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fba31-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fba31-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact_2"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/memberOf
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="fba31-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fba31-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-orgcontact-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="fba31-135">C#</span><span class="sxs-lookup"><span data-stu-id="fba31-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-orgcontact-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="fba31-136">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fba31-136">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fba31-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fba31-137">Response</span></span>
<span data-ttu-id="fba31-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fba31-138">Here is an example of the response.</span></span> <span data-ttu-id="fba31-139">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fba31-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


