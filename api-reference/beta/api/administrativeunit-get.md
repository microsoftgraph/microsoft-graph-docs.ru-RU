---
title: Получение administrativeUnit
description: Получение свойств и связей объекта administrativeUnit.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d674513606da3e19cb870c9a01a5bd106e29f060
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962640"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="66243-103">Получение administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="66243-103">Get administrativeUnit</span></span>

<span data-ttu-id="66243-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66243-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66243-105">Получение свойств и связей объекта [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="66243-105">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="66243-106">Так как ресурс **administrativeUnit** поддерживает [расширения](/graph/extensibility-overview), с помощью операции можно также `GET` получить настраиваемые свойства и данные расширения в экземпляре **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="66243-106">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="66243-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66243-107">Permissions</span></span>
<span data-ttu-id="66243-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66243-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="66243-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66243-110">Permission type</span></span>      | <span data-ttu-id="66243-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66243-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66243-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66243-112">Delegated (work or school account)</span></span> | <span data-ttu-id="66243-113">AdministrativeUnit. Read. ALL, Directory. Read. ALL, AdministrativeUnit. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="66243-113">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="66243-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66243-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66243-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66243-115">Not supported.</span></span>    |
|<span data-ttu-id="66243-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="66243-116">Application</span></span> | <span data-ttu-id="66243-117">AdministrativeUnit. Read. ALL, Directory. Read. ALL, AdministrativeUnit. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="66243-117">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66243-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66243-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="66243-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="66243-119">Optional query parameters</span></span>
<span data-ttu-id="66243-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="66243-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66243-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66243-121">Request headers</span></span>
| <span data-ttu-id="66243-122">Имя</span><span class="sxs-lookup"><span data-stu-id="66243-122">Name</span></span>      |<span data-ttu-id="66243-123">Описание</span><span class="sxs-lookup"><span data-stu-id="66243-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="66243-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66243-124">Authorization</span></span>  | <span data-ttu-id="66243-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66243-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66243-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66243-127">Request body</span></span>
<span data-ttu-id="66243-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="66243-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66243-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="66243-129">Response</span></span>

<span data-ttu-id="66243-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [administrativeUnit](../resources/administrativeunit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66243-130">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="66243-131">Пример</span><span class="sxs-lookup"><span data-stu-id="66243-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66243-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="66243-132">Request</span></span>
<span data-ttu-id="66243-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66243-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66243-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="66243-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
# <a name="c"></a>[<span data-ttu-id="66243-135">C#</span><span class="sxs-lookup"><span data-stu-id="66243-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66243-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66243-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66243-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66243-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66243-138">Java</span><span class="sxs-lookup"><span data-stu-id="66243-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="66243-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="66243-139">Response</span></span>
<span data-ttu-id="66243-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66243-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="66243-143">См. также</span><span class="sxs-lookup"><span data-stu-id="66243-143">See also</span></span>

- [<span data-ttu-id="66243-144">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="66243-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="66243-145">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="66243-145">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
