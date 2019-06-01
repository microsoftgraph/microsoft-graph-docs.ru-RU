---
title: Получение administrativeUnit
description: Получение свойств и связей объекта administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: aa56f7752e303ffbf694bd8ecbe21dd71884d3b1
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655301"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="88236-103">Получение administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="88236-103">Get administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88236-104">Получение свойств и связей объекта [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="88236-104">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="88236-105">Так как ресурс **administrativeUnit** поддерживает [расширения](/graph/extensibility-overview), с помощью `GET` операции можно также получить настраиваемые свойства и данные расширения в экземпляре **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="88236-105">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="88236-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88236-106">Permissions</span></span>
<span data-ttu-id="88236-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88236-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="88236-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88236-109">Permission type</span></span>      | <span data-ttu-id="88236-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88236-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88236-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88236-111">Delegated (work or school account)</span></span> | <span data-ttu-id="88236-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="88236-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="88236-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88236-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88236-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88236-114">Not supported.</span></span>    |
|<span data-ttu-id="88236-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88236-115">Application</span></span> | <span data-ttu-id="88236-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88236-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88236-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88236-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="88236-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="88236-118">Optional query parameters</span></span>
<span data-ttu-id="88236-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="88236-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88236-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88236-120">Request headers</span></span>
| <span data-ttu-id="88236-121">Имя</span><span class="sxs-lookup"><span data-stu-id="88236-121">Name</span></span>      |<span data-ttu-id="88236-122">Описание</span><span class="sxs-lookup"><span data-stu-id="88236-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="88236-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88236-123">Authorization</span></span>  | <span data-ttu-id="88236-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88236-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88236-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="88236-126">Request body</span></span>
<span data-ttu-id="88236-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88236-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88236-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="88236-128">Response</span></span>

<span data-ttu-id="88236-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [administrativeUnit](../resources/administrativeunit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="88236-129">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="88236-130">Пример</span><span class="sxs-lookup"><span data-stu-id="88236-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88236-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="88236-131">Request</span></span>
<span data-ttu-id="88236-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88236-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="88236-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="88236-133">Response</span></span>
<span data-ttu-id="88236-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88236-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="88236-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="88236-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="88236-138">C#</span><span class="sxs-lookup"><span data-stu-id="88236-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_administrativeunit-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="88236-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="88236-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_administrativeunit-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="88236-140">См. также</span><span class="sxs-lookup"><span data-stu-id="88236-140">See also</span></span>

- [<span data-ttu-id="88236-141">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="88236-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="88236-142">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="88236-142">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
    "Error: /api-reference/beta/api/administrativeunit-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/administrativeunit-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
