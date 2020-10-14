---
title: 'orgContact: List memberOf'
description: Получение списка групп и единиц админстративе, участником которых является контакт.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 90cc67c4f12ba59ea66446fedf8cb1dbea991048
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459027"
---
# <a name="orgcontact-list-memberof"></a><span data-ttu-id="295fb-103">orgContact: List memberOf</span><span class="sxs-lookup"><span data-stu-id="295fb-103">orgContact: List memberOf</span></span>

<span data-ttu-id="295fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="295fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="295fb-105">Получение списка групп и единиц админстративе, участником которых является контакт.</span><span class="sxs-lookup"><span data-stu-id="295fb-105">Retrieve the list of groups and adminstrative units the contact is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="295fb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="295fb-106">Permissions</span></span>
<span data-ttu-id="295fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="295fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="295fb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="295fb-109">Permission type</span></span>      | <span data-ttu-id="295fb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="295fb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="295fb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="295fb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="295fb-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="295fb-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="295fb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="295fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="295fb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="295fb-114">Not supported.</span></span>    |
|<span data-ttu-id="295fb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="295fb-115">Application</span></span> | <span data-ttu-id="295fb-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="295fb-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="295fb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="295fb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="295fb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="295fb-118">Optional query parameters</span></span>
<span data-ttu-id="295fb-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="295fb-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="295fb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="295fb-120">Request headers</span></span>
| <span data-ttu-id="295fb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="295fb-121">Name</span></span>       | <span data-ttu-id="295fb-122">Тип</span><span class="sxs-lookup"><span data-stu-id="295fb-122">Type</span></span> | <span data-ttu-id="295fb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="295fb-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="295fb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="295fb-124">Authorization</span></span>  | <span data-ttu-id="295fb-125">string</span><span class="sxs-lookup"><span data-stu-id="295fb-125">string</span></span>  | <span data-ttu-id="295fb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="295fb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="295fb-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="295fb-128">Request body</span></span>
<span data-ttu-id="295fb-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="295fb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="295fb-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="295fb-130">Response</span></span>

<span data-ttu-id="295fb-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="295fb-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="295fb-132">Пример</span><span class="sxs-lookup"><span data-stu-id="295fb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="295fb-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="295fb-133">Request</span></span>
<span data-ttu-id="295fb-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="295fb-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="295fb-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="295fb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contact_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="295fb-136">C#</span><span class="sxs-lookup"><span data-stu-id="295fb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contact-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="295fb-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="295fb-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contact-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="295fb-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="295fb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contact-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="295fb-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="295fb-139">Response</span></span>
<span data-ttu-id="295fb-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="295fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
