---
title: Получить параметр группы
description: Извлечение свойств определенного объекта настройки группы.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b92840fd1a10ab6960886e8d783ee758d5d1e96b
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679780"
---
# <a name="get-a-group-setting"></a><span data-ttu-id="b397f-103">Получить параметр группы</span><span class="sxs-lookup"><span data-stu-id="b397f-103">Get a group setting</span></span>

<span data-ttu-id="b397f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b397f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b397f-105">Извлечение свойств определенного объекта настройки группы.</span><span class="sxs-lookup"><span data-stu-id="b397f-105">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b397f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b397f-106">Permissions</span></span>

<span data-ttu-id="b397f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b397f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b397f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b397f-109">Permission type</span></span>      | <span data-ttu-id="b397f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b397f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b397f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b397f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b397f-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b397f-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b397f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b397f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b397f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b397f-114">Not supported.</span></span>    |
|<span data-ttu-id="b397f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b397f-115">Application</span></span> | <span data-ttu-id="b397f-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b397f-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b397f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b397f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="b397f-118">Получите определенный параметр клиента или группы.</span><span class="sxs-lookup"><span data-stu-id="b397f-118">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b397f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b397f-119">Optional query parameters</span></span>
<span data-ttu-id="b397f-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b397f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

> <span data-ttu-id="b397f-121">Примечание. $filter не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b397f-121">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b397f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b397f-122">Request headers</span></span>
| <span data-ttu-id="b397f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="b397f-123">Name</span></span> | <span data-ttu-id="b397f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b397f-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="b397f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b397f-125">Authorization</span></span> | <span data-ttu-id="b397f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b397f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b397f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b397f-128">Request body</span></span>

<span data-ttu-id="b397f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b397f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b397f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b397f-130">Response</span></span>

<span data-ttu-id="b397f-131">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект groupSetting](../resources/groupsetting.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b397f-131">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b397f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b397f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b397f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b397f-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b397f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b397f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
# <a name="c"></a>[<span data-ttu-id="b397f-135">C#</span><span class="sxs-lookup"><span data-stu-id="b397f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b397f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b397f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b397f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b397f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b397f-138">Java</span><span class="sxs-lookup"><span data-stu-id="b397f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b397f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b397f-139">Response</span></span>

<span data-ttu-id="b397f-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b397f-140">Note: The response object shown here might be shortened for readability.</span></span>
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
