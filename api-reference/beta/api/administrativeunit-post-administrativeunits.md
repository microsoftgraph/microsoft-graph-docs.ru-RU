---
title: Создание administrativeUnit
description: Используйте этот API для создания нового administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5195bd4cfce03e20a93b8cc465b6ddd28e616d5c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258690"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="e902b-103">Создание administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="e902b-103">Create administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e902b-104">Используйте этот API для создания нового [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="e902b-104">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="e902b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e902b-105">Permissions</span></span>
<span data-ttu-id="e902b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e902b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e902b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e902b-108">Permission type</span></span>      | <span data-ttu-id="e902b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e902b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e902b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e902b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e902b-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e902b-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e902b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e902b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e902b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e902b-113">Not supported.</span></span>    |
|<span data-ttu-id="e902b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e902b-114">Application</span></span> | <span data-ttu-id="e902b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e902b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e902b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e902b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="e902b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e902b-117">Request headers</span></span>
| <span data-ttu-id="e902b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e902b-118">Name</span></span>      |<span data-ttu-id="e902b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e902b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e902b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e902b-120">Authorization</span></span>  | <span data-ttu-id="e902b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e902b-p102">Bearer {token}. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="e902b-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e902b-123">Request body</span></span>
<span data-ttu-id="e902b-124">В тексте запроса добавьте представление объекта [administrativeUnit](../resources/administrativeunit.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e902b-124">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="e902b-125">Так как ресурс **administrativeUnit** поддерживает [расширения](/graph/extensibility-overview), вы можете использовать `POST` операцию и добавлять настраиваемые свойства с собственными данными в административную единицу при создании.</span><span class="sxs-lookup"><span data-stu-id="e902b-125">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="e902b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e902b-126">Response</span></span>

<span data-ttu-id="e902b-127">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [administrativeUnit](../resources/administrativeunit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e902b-127">If successful, this method returns `201 Created` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e902b-128">Пример</span><span class="sxs-lookup"><span data-stu-id="e902b-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e902b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e902b-129">Request</span></span>
<span data-ttu-id="e902b-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e902b-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_administrativeunit_from_administrativeunits"
}-->
```http
POST https://graph.microsoft.com/beta/administrativeUnits
Content-type: application/json
Content-length: 150

{
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "true"
}
```
<span data-ttu-id="e902b-131">В тексте запроса добавьте представление объекта [administrativeUnit](../resources/administrativeunit.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e902b-131">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e902b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e902b-132">Response</span></span>
<span data-ttu-id="e902b-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e902b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 172

{
  "administrativeUnit": {
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "true",
    "id": "7a3dc8f3-b3a0-4164-9a99-ed36f3af039f"
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e902b-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="e902b-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e902b-137">C#</span><span class="sxs-lookup"><span data-stu-id="e902b-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_administrativeunit_from_administrativeunits-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e902b-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="e902b-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_administrativeunit_from_administrativeunits-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e902b-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e902b-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_administrativeunit_from_administrativeunits-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="e902b-140">См. также</span><span class="sxs-lookup"><span data-stu-id="e902b-140">See also</span></span>

- [<span data-ttu-id="e902b-141">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="e902b-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e902b-142">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e902b-142">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-post-administrativeunits.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/administrativeunit-post-administrativeunits.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/administrativeunit-post-administrativeunits.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
