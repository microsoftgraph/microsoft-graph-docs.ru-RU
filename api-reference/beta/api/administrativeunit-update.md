---
title: Обновление administrativeunit
description: Обновление свойств объекта administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3b8a41fd335d003abeaafaad08850d638716e2f1
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408568"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="83dff-103">Обновление administrativeunit</span><span class="sxs-lookup"><span data-stu-id="83dff-103">Update administrativeunit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83dff-104">Обновление свойств объекта [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="83dff-104">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="83dff-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83dff-105">Permissions</span></span>
<span data-ttu-id="83dff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83dff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="83dff-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83dff-108">Permission type</span></span>      | <span data-ttu-id="83dff-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="83dff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83dff-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83dff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="83dff-111">AdministrativeUnit. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="83dff-111">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="83dff-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83dff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83dff-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83dff-113">Not supported.</span></span>    |
|<span data-ttu-id="83dff-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83dff-114">Application</span></span> | <span data-ttu-id="83dff-115">AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="83dff-115">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83dff-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83dff-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="83dff-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83dff-117">Request headers</span></span>

| <span data-ttu-id="83dff-118">Имя</span><span class="sxs-lookup"><span data-stu-id="83dff-118">Name</span></span>      |<span data-ttu-id="83dff-119">Описание</span><span class="sxs-lookup"><span data-stu-id="83dff-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="83dff-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83dff-120">Authorization</span></span>  | <span data-ttu-id="83dff-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83dff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83dff-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="83dff-123">Request body</span></span>

<span data-ttu-id="83dff-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="83dff-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="83dff-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="83dff-127">Property</span></span>   | <span data-ttu-id="83dff-128">Тип</span><span class="sxs-lookup"><span data-stu-id="83dff-128">Type</span></span> |<span data-ttu-id="83dff-129">Описание</span><span class="sxs-lookup"><span data-stu-id="83dff-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83dff-130">description</span><span class="sxs-lookup"><span data-stu-id="83dff-130">description</span></span>|<span data-ttu-id="83dff-131">строка</span><span class="sxs-lookup"><span data-stu-id="83dff-131">string</span></span>|<span data-ttu-id="83dff-132">Описание административной единицы.</span><span class="sxs-lookup"><span data-stu-id="83dff-132">Description for the administrative unit.</span></span>|
|<span data-ttu-id="83dff-133">displayName</span><span class="sxs-lookup"><span data-stu-id="83dff-133">displayName</span></span>|<span data-ttu-id="83dff-134">string</span><span class="sxs-lookup"><span data-stu-id="83dff-134">string</span></span>|<span data-ttu-id="83dff-135">Отображаемое имя административной единицы.</span><span class="sxs-lookup"><span data-stu-id="83dff-135">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="83dff-136">visibility</span><span class="sxs-lookup"><span data-stu-id="83dff-136">visibility</span></span>|<span data-ttu-id="83dff-137">string</span><span class="sxs-lookup"><span data-stu-id="83dff-137">string</span></span>|<span data-ttu-id="83dff-138">Видимость административной единицы.</span><span class="sxs-lookup"><span data-stu-id="83dff-138">Visibility for the administrative unit.</span></span> <span data-ttu-id="83dff-139">Если не задано, то значение по умолчанию — "общедоступный".</span><span class="sxs-lookup"><span data-stu-id="83dff-139">If not set then the default is "public".</span></span> <span data-ttu-id="83dff-140">Может иметь значение "значение hiddenmembership", которое скрывает членство в группах, не являющихся участниками.</span><span class="sxs-lookup"><span data-stu-id="83dff-140">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="83dff-141">Так как ресурс **administrativeUnit** поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, зависящие от приложения, в пользовательских свойствах расширения в существующем экземпляре **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="83dff-141">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="83dff-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="83dff-142">Response</span></span>

<span data-ttu-id="83dff-143">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="83dff-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="83dff-144">Пример</span><span class="sxs-lookup"><span data-stu-id="83dff-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="83dff-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="83dff-145">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="83dff-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="83dff-146">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="83dff-147">C#</span><span class="sxs-lookup"><span data-stu-id="83dff-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="83dff-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83dff-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="83dff-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="83dff-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="83dff-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="83dff-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="83dff-151">См. также</span><span class="sxs-lookup"><span data-stu-id="83dff-151">See also</span></span>

- [<span data-ttu-id="83dff-152">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="83dff-152">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="83dff-153">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="83dff-153">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
  ]
}
-->
