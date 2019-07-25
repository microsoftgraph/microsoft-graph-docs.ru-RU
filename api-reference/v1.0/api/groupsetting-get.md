---
title: Получение параметра группы
description: Получение свойств определенного объекта параметров группы.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ed3eadf8834256783b119670c02e193f22f79fdb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886767"
---
# <a name="get-a-group-setting"></a><span data-ttu-id="587ea-103">Получение параметра группы</span><span class="sxs-lookup"><span data-stu-id="587ea-103">Get a group setting</span></span>

<span data-ttu-id="587ea-104">Получение свойств определенного объекта параметров группы.</span><span class="sxs-lookup"><span data-stu-id="587ea-104">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="587ea-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="587ea-105">Permissions</span></span>

<span data-ttu-id="587ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="587ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="587ea-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="587ea-108">Permission type</span></span>      | <span data-ttu-id="587ea-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="587ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="587ea-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="587ea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="587ea-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="587ea-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="587ea-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="587ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="587ea-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="587ea-113">Not supported.</span></span>    |
|<span data-ttu-id="587ea-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="587ea-114">Application</span></span> | <span data-ttu-id="587ea-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="587ea-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="587ea-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="587ea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="587ea-117">Получение определенного параметра на уровне клиента или группы.</span><span class="sxs-lookup"><span data-stu-id="587ea-117">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="587ea-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="587ea-118">Optional query parameters</span></span>
<span data-ttu-id="587ea-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="587ea-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="587ea-120">Примечание. $filter не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="587ea-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="587ea-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="587ea-121">Request headers</span></span>
| <span data-ttu-id="587ea-122">Имя</span><span class="sxs-lookup"><span data-stu-id="587ea-122">Name</span></span> | <span data-ttu-id="587ea-123">Описание</span><span class="sxs-lookup"><span data-stu-id="587ea-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="587ea-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="587ea-124">Authorization</span></span> | <span data-ttu-id="587ea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="587ea-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="587ea-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="587ea-127">Request body</span></span>

<span data-ttu-id="587ea-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="587ea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="587ea-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="587ea-129">Response</span></span>

<span data-ttu-id="587ea-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [groupSetting](../resources/groupsetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="587ea-130">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="587ea-131">Пример</span><span class="sxs-lookup"><span data-stu-id="587ea-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="587ea-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="587ea-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="587ea-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="587ea-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```http
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="587ea-134">C#</span><span class="sxs-lookup"><span data-stu-id="587ea-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="587ea-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="587ea-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="587ea-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="587ea-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="587ea-137">Java</span><span class="sxs-lookup"><span data-stu-id="587ea-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="587ea-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="587ea-138">Response</span></span>

<span data-ttu-id="587ea-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="587ea-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
