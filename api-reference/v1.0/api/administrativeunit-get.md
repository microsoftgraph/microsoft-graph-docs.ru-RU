---
title: Get administrativeUnit
description: Извлечение свойств и связей объекта administrativeUnit.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: bbadb0cfdf8a8aaa613482fc08fdb2535696b1ea
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050642"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="eafb9-103">Get administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="eafb9-103">Get administrativeUnit</span></span>

<span data-ttu-id="eafb9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eafb9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eafb9-105">Извлечение свойств и связей объекта [administrativeUnit.](../resources/administrativeunit.md)</span><span class="sxs-lookup"><span data-stu-id="eafb9-105">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="eafb9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eafb9-106">Permissions</span></span>
<span data-ttu-id="eafb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eafb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="eafb9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eafb9-109">Permission type</span></span>      | <span data-ttu-id="eafb9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eafb9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eafb9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eafb9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eafb9-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eafb9-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eafb9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eafb9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eafb9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eafb9-114">Not supported.</span></span>    |
|<span data-ttu-id="eafb9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eafb9-115">Application</span></span> | <span data-ttu-id="eafb9-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eafb9-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eafb9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eafb9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eafb9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eafb9-118">Optional query parameters</span></span>
<span data-ttu-id="eafb9-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="eafb9-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eafb9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eafb9-120">Request headers</span></span>
| <span data-ttu-id="eafb9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="eafb9-121">Name</span></span>      |<span data-ttu-id="eafb9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="eafb9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eafb9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eafb9-123">Authorization</span></span>  | <span data-ttu-id="eafb9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eafb9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eafb9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eafb9-126">Request body</span></span>
<span data-ttu-id="eafb9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eafb9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eafb9-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="eafb9-128">Response</span></span>

<span data-ttu-id="eafb9-129">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект administrativeUnit](../resources/administrativeunit.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="eafb9-129">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eafb9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="eafb9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eafb9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="eafb9-131">Request</span></span>
<span data-ttu-id="eafb9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eafb9-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="eafb9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="eafb9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}
```
# <a name="c"></a>[<span data-ttu-id="eafb9-134">C#</span><span class="sxs-lookup"><span data-stu-id="eafb9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eafb9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eafb9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eafb9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eafb9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eafb9-137">Java</span><span class="sxs-lookup"><span data-stu-id="eafb9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="eafb9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="eafb9-138">Response</span></span>
<span data-ttu-id="eafb9-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eafb9-139">Here is an example of the response.</span></span> <span data-ttu-id="eafb9-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="eafb9-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

## <a name="see-also"></a><span data-ttu-id="eafb9-141">См. также</span><span class="sxs-lookup"><span data-stu-id="eafb9-141">See also</span></span>

- [<span data-ttu-id="eafb9-142">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="eafb9-142">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="eafb9-143">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="eafb9-143">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
