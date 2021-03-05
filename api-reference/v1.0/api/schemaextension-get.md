---
title: Получение schemaExtension
description: Получите свойства указанного определения схемыExtension.
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 2b08b4600a729af8289c2592a023b95a0e73a182
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474516"
---
# <a name="get-schemaextension"></a><span data-ttu-id="0ccdf-103">Получение schemaExtension</span><span class="sxs-lookup"><span data-stu-id="0ccdf-103">Get schemaExtension</span></span>

<span data-ttu-id="0ccdf-104">Пространство имен: microsoft.graph Получите свойства указанного определения [схемыExtension.](../resources/schemaextension.md)</span><span class="sxs-lookup"><span data-stu-id="0ccdf-104">Namespace: microsoft.graph Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ccdf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ccdf-105">Permissions</span></span>
<span data-ttu-id="0ccdf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ccdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0ccdf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ccdf-108">Permission type</span></span>      | <span data-ttu-id="0ccdf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ccdf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ccdf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ccdf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ccdf-111">User.Read, Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ccdf-111">User.Read, Application.Read.All</span></span>    |
|<span data-ttu-id="0ccdf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ccdf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ccdf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ccdf-113">Not supported.</span></span>    |
|<span data-ttu-id="0ccdf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ccdf-114">Application</span></span> | <span data-ttu-id="0ccdf-115">Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ccdf-115">Application.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ccdf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ccdf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0ccdf-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0ccdf-117">Optional query parameters</span></span>
<span data-ttu-id="0ccdf-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0ccdf-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ccdf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ccdf-119">Request headers</span></span>
| <span data-ttu-id="0ccdf-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0ccdf-120">Name</span></span>      |<span data-ttu-id="0ccdf-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0ccdf-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0ccdf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ccdf-122">Authorization</span></span>  | <span data-ttu-id="0ccdf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ccdf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ccdf-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0ccdf-125">Content-Type</span></span>   | <span data-ttu-id="0ccdf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ccdf-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ccdf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ccdf-127">Request body</span></span>
<span data-ttu-id="0ccdf-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ccdf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ccdf-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ccdf-129">Response</span></span>

<span data-ttu-id="0ccdf-130">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект schemaExtension](../resources/schemaextension.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0ccdf-130">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ccdf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0ccdf-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ccdf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ccdf-132">Request</span></span>
<span data-ttu-id="0ccdf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ccdf-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0ccdf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ccdf-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/schemaExtensions/graphlearn_test
```
# <a name="c"></a>[<span data-ttu-id="0ccdf-135">C#</span><span class="sxs-lookup"><span data-stu-id="0ccdf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ccdf-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ccdf-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ccdf-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ccdf-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0ccdf-138">Java</span><span class="sxs-lookup"><span data-stu-id="0ccdf-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0ccdf-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ccdf-139">Response</span></span>
<span data-ttu-id="0ccdf-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ccdf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "id":"graphlearn_test",
    "description": "Yet another test schema",
    "targetTypes": [
        "User", "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "testName",
            "type": "String"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="0ccdf-143">См. также</span><span class="sxs-lookup"><span data-stu-id="0ccdf-143">See also</span></span>

- [<span data-ttu-id="0ccdf-144">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="0ccdf-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0ccdf-145">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="0ccdf-145">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
