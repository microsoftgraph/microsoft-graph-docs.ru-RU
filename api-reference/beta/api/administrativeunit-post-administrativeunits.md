---
title: Создание administrativeUnit
description: Используйте этот API для создания нового administrativeUnit.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4815082a8a5930e426e0843d2dcf2ebe6ef190d5
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636634"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="07d76-103">Создание administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="07d76-103">Create administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07d76-104">Используйте этот API для создания нового [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="07d76-104">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="07d76-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07d76-105">Permissions</span></span>
<span data-ttu-id="07d76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07d76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="07d76-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07d76-108">Permission type</span></span>      | <span data-ttu-id="07d76-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07d76-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07d76-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07d76-110">Delegated (work or school account)</span></span> | <span data-ttu-id="07d76-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07d76-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="07d76-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07d76-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07d76-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07d76-113">Not supported.</span></span>    |
|<span data-ttu-id="07d76-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07d76-114">Application</span></span> | <span data-ttu-id="07d76-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07d76-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="07d76-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07d76-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="07d76-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07d76-117">Request headers</span></span>
| <span data-ttu-id="07d76-118">Имя</span><span class="sxs-lookup"><span data-stu-id="07d76-118">Name</span></span>      |<span data-ttu-id="07d76-119">Описание</span><span class="sxs-lookup"><span data-stu-id="07d76-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="07d76-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07d76-120">Authorization</span></span>  | <span data-ttu-id="07d76-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07d76-p102">Bearer {token}. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="07d76-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07d76-123">Request body</span></span>
<span data-ttu-id="07d76-124">В тексте запроса добавьте представление объекта [AdministrativeUnit](../resources/administrativeunit.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07d76-124">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="07d76-125">Так как ресурс **administrativeUnit** поддерживает [расширения](/graph/extensibility-overview), вы можете использовать `POST` операцию и добавлять настраиваемые свойства с собственными данными в административную единицу при создании.</span><span class="sxs-lookup"><span data-stu-id="07d76-125">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="07d76-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="07d76-126">Response</span></span>

<span data-ttu-id="07d76-127">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [administrativeUnit](../resources/administrativeunit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="07d76-127">If successful, this method returns `201 Created` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07d76-128">Пример</span><span class="sxs-lookup"><span data-stu-id="07d76-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07d76-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="07d76-129">Request</span></span>
<span data-ttu-id="07d76-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07d76-130">Here is an example of the request.</span></span>
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
<span data-ttu-id="07d76-131">В тексте запроса добавьте представление объекта [AdministrativeUnit](../resources/administrativeunit.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07d76-131">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="07d76-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="07d76-132">Response</span></span>
<span data-ttu-id="07d76-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07d76-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="07d76-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="07d76-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="07d76-137">Языках</span><span class="sxs-lookup"><span data-stu-id="07d76-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_administrativeunit_from_administrativeunits-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="07d76-138">Язык</span><span class="sxs-lookup"><span data-stu-id="07d76-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_administrativeunit_from_administrativeunits-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="07d76-139">См. также</span><span class="sxs-lookup"><span data-stu-id="07d76-139">See also</span></span>

- [<span data-ttu-id="07d76-140">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="07d76-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="07d76-141">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="07d76-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
    "Error: /api-reference/beta/api/administrativeunit-post-administrativeunits.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/administrativeunit-post-administrativeunits.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
