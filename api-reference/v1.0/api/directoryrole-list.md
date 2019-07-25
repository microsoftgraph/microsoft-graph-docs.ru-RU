---
title: Перечисление объектов directoryRole
description: Перечисление ролей каталога, активированных в клиенте.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 25c743b0eed01ffa760fb2f4387ad4ca39fca37b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865945"
---
# <a name="list-directoryroles"></a><span data-ttu-id="d946b-103">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="d946b-103">List directoryRoles</span></span>

<span data-ttu-id="d946b-104">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d946b-104">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="d946b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d946b-105">Permissions</span></span>
<span data-ttu-id="d946b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d946b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d946b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d946b-108">Permission type</span></span>      | <span data-ttu-id="d946b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d946b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d946b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d946b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d946b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d946b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d946b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d946b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d946b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d946b-113">Not supported.</span></span>    |
|<span data-ttu-id="d946b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d946b-114">Application</span></span> | <span data-ttu-id="d946b-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d946b-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d946b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d946b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d946b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d946b-117">Optional query parameters</span></span>
<span data-ttu-id="d946b-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="d946b-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d946b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d946b-119">Request headers</span></span>
| <span data-ttu-id="d946b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d946b-120">Name</span></span>       | <span data-ttu-id="d946b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d946b-121">Type</span></span> | <span data-ttu-id="d946b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d946b-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d946b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d946b-123">Authorization</span></span>  | <span data-ttu-id="d946b-124">string</span><span class="sxs-lookup"><span data-stu-id="d946b-124">string</span></span>  | <span data-ttu-id="d946b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d946b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d946b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d946b-127">Request body</span></span>
<span data-ttu-id="d946b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d946b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d946b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d946b-129">Response</span></span>

<span data-ttu-id="d946b-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d946b-130">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d946b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d946b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d946b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d946b-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d946b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d946b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d946b-134">C#</span><span class="sxs-lookup"><span data-stu-id="d946b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d946b-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="d946b-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d946b-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d946b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d946b-137">Java</span><span class="sxs-lookup"><span data-stu-id="d946b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d946b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d946b-138">Response</span></span>
<span data-ttu-id="d946b-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d946b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
