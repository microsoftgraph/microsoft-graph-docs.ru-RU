---
title: Обновление administrativeunit
description: Обновление свойств объекта administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: adf8d355c9e693ef1c79b0b774dc859e7a8d4f26
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655217"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="28b8e-103">Обновление administrativeunit</span><span class="sxs-lookup"><span data-stu-id="28b8e-103">Update administrativeunit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28b8e-104">Обновление свойств объекта [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="28b8e-104">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="28b8e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28b8e-105">Permissions</span></span>
<span data-ttu-id="28b8e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28b8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="28b8e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28b8e-108">Permission type</span></span>      | <span data-ttu-id="28b8e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28b8e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28b8e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28b8e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="28b8e-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="28b8e-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="28b8e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28b8e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28b8e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28b8e-113">Not supported.</span></span>    |
|<span data-ttu-id="28b8e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28b8e-114">Application</span></span> | <span data-ttu-id="28b8e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28b8e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28b8e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28b8e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="28b8e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28b8e-117">Request headers</span></span>

| <span data-ttu-id="28b8e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="28b8e-118">Name</span></span>      |<span data-ttu-id="28b8e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="28b8e-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="28b8e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28b8e-120">Authorization</span></span>  | <span data-ttu-id="28b8e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28b8e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28b8e-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="28b8e-123">Request body</span></span>

<span data-ttu-id="28b8e-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="28b8e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="28b8e-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="28b8e-127">Property</span></span>   | <span data-ttu-id="28b8e-128">Тип</span><span class="sxs-lookup"><span data-stu-id="28b8e-128">Type</span></span> |<span data-ttu-id="28b8e-129">Описание</span><span class="sxs-lookup"><span data-stu-id="28b8e-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28b8e-130">description</span><span class="sxs-lookup"><span data-stu-id="28b8e-130">description</span></span>|<span data-ttu-id="28b8e-131">строка</span><span class="sxs-lookup"><span data-stu-id="28b8e-131">string</span></span>|<span data-ttu-id="28b8e-132">Описание административной единицы.</span><span class="sxs-lookup"><span data-stu-id="28b8e-132">Description for the administrative unit.</span></span>|
|<span data-ttu-id="28b8e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="28b8e-133">displayName</span></span>|<span data-ttu-id="28b8e-134">string</span><span class="sxs-lookup"><span data-stu-id="28b8e-134">string</span></span>|<span data-ttu-id="28b8e-135">Отображаемое имя административной единицы.</span><span class="sxs-lookup"><span data-stu-id="28b8e-135">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="28b8e-136">visibility</span><span class="sxs-lookup"><span data-stu-id="28b8e-136">visibility</span></span>|<span data-ttu-id="28b8e-137">string</span><span class="sxs-lookup"><span data-stu-id="28b8e-137">string</span></span>|<span data-ttu-id="28b8e-138">Видимость административной единицы.</span><span class="sxs-lookup"><span data-stu-id="28b8e-138">Visibility for the administrative unit.</span></span> <span data-ttu-id="28b8e-139">Если не задано, то значение по умолчанию — "общедоступный".</span><span class="sxs-lookup"><span data-stu-id="28b8e-139">If not set then the default is "public".</span></span> <span data-ttu-id="28b8e-140">Может иметь значение "значение hiddenmembership", которое скрывает членство в группах, не являющихся участниками.</span><span class="sxs-lookup"><span data-stu-id="28b8e-140">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="28b8e-141">Так как ресурс **administrativeUnit** поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, зависящие от приложения, в пользовательских свойствах расширения в существующем экземпляре **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="28b8e-141">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="28b8e-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="28b8e-142">Response</span></span>

<span data-ttu-id="28b8e-143">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="28b8e-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="28b8e-144">Пример</span><span class="sxs-lookup"><span data-stu-id="28b8e-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="28b8e-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="28b8e-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_administrativeunit"
}-->
```http
PATCH https://graph.microsoft.com/beta/administrativeUnits/{id}
Content-type: application/json
Content-length: 114

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value"
}
```

##### <a name="response"></a><span data-ttu-id="28b8e-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="28b8e-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="28b8e-147">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="28b8e-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="28b8e-148">C#</span><span class="sxs-lookup"><span data-stu-id="28b8e-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_administrativeunit-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="28b8e-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="28b8e-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_administrativeunit-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="28b8e-150">См. также</span><span class="sxs-lookup"><span data-stu-id="28b8e-150">See also</span></span>

- [<span data-ttu-id="28b8e-151">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="28b8e-151">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="28b8e-152">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="28b8e-152">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update administrativeunit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/administrativeunit-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
