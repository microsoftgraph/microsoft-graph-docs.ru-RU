---
title: Создание directReport
description: Используйте этот API для создания нового directReport.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d2a45ffc46c15b28e81c1c3a871b39b1b7ffed93
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055521"
---
# <a name="create-directreport"></a><span data-ttu-id="93828-103">Создание directReport</span><span class="sxs-lookup"><span data-stu-id="93828-103">Create directReport</span></span>

<span data-ttu-id="93828-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93828-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93828-105">Используйте этот API для создания нового directReport.</span><span class="sxs-lookup"><span data-stu-id="93828-105">Use this API to create a new directReport.</span></span>
## <a name="permissions"></a><span data-ttu-id="93828-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93828-106">Permissions</span></span>
<span data-ttu-id="93828-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93828-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93828-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93828-109">Permission type</span></span>      | <span data-ttu-id="93828-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93828-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93828-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93828-111">Delegated (work or school account)</span></span> | <span data-ttu-id="93828-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93828-112">Not supported.</span></span>    |
|<span data-ttu-id="93828-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93828-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93828-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93828-114">Not supported.</span></span>    |
|<span data-ttu-id="93828-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93828-115">Application</span></span> | <span data-ttu-id="93828-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93828-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="93828-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93828-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/directReports

```
## <a name="request-headers"></a><span data-ttu-id="93828-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93828-118">Request headers</span></span>
| <span data-ttu-id="93828-119">Имя</span><span class="sxs-lookup"><span data-stu-id="93828-119">Name</span></span>       | <span data-ttu-id="93828-120">Тип</span><span class="sxs-lookup"><span data-stu-id="93828-120">Type</span></span> | <span data-ttu-id="93828-121">Описание</span><span class="sxs-lookup"><span data-stu-id="93828-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="93828-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="93828-122">Authorization</span></span>  | <span data-ttu-id="93828-123">string</span><span class="sxs-lookup"><span data-stu-id="93828-123">string</span></span>  | <span data-ttu-id="93828-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93828-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93828-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93828-126">Request body</span></span>
<span data-ttu-id="93828-127">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93828-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="93828-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="93828-128">Response</span></span>

<span data-ttu-id="93828-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="93828-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93828-130">Пример</span><span class="sxs-lookup"><span data-stu-id="93828-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93828-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="93828-131">Request</span></span>
<span data-ttu-id="93828-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93828-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="93828-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="93828-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact_1"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/directReports
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="93828-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93828-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-orgcontact-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="93828-135">C#</span><span class="sxs-lookup"><span data-stu-id="93828-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-orgcontact-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="93828-136">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93828-136">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="93828-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="93828-137">Response</span></span>
<span data-ttu-id="93828-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="93828-138">Here is an example of the response.</span></span> <span data-ttu-id="93828-139">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="93828-139">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Create directReport",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


