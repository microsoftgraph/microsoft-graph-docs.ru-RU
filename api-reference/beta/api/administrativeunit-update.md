---
title: Обновление administrativeunit
description: Обновление свойств объекта administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 86db267942255ca5cedfd66a2d1ec145096f9af9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945720"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="a5eb8-103">Обновление administrativeunit</span><span class="sxs-lookup"><span data-stu-id="a5eb8-103">Update administrativeunit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5eb8-104">Обновление свойств объекта [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="a5eb8-104">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a5eb8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5eb8-105">Permissions</span></span>
<span data-ttu-id="a5eb8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5eb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a5eb8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5eb8-108">Permission type</span></span>      | <span data-ttu-id="a5eb8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5eb8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5eb8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5eb8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a5eb8-111">AdministrativeUnit. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="a5eb8-111">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a5eb8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5eb8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5eb8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5eb8-113">Not supported.</span></span>    |
|<span data-ttu-id="a5eb8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5eb8-114">Application</span></span> | <span data-ttu-id="a5eb8-115">AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a5eb8-115">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5eb8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5eb8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a5eb8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5eb8-117">Request headers</span></span>

| <span data-ttu-id="a5eb8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a5eb8-118">Name</span></span>      |<span data-ttu-id="a5eb8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a5eb8-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a5eb8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5eb8-120">Authorization</span></span>  | <span data-ttu-id="a5eb8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5eb8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5eb8-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a5eb8-123">Request body</span></span>

<span data-ttu-id="a5eb8-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a5eb8-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a5eb8-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5eb8-127">Property</span></span>   | <span data-ttu-id="a5eb8-128">Тип</span><span class="sxs-lookup"><span data-stu-id="a5eb8-128">Type</span></span> |<span data-ttu-id="a5eb8-129">Описание</span><span class="sxs-lookup"><span data-stu-id="a5eb8-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5eb8-130">description</span><span class="sxs-lookup"><span data-stu-id="a5eb8-130">description</span></span>|<span data-ttu-id="a5eb8-131">строка</span><span class="sxs-lookup"><span data-stu-id="a5eb8-131">string</span></span>|<span data-ttu-id="a5eb8-132">Описание административной единицы.</span><span class="sxs-lookup"><span data-stu-id="a5eb8-132">Description for the administrative unit.</span></span>|
|<span data-ttu-id="a5eb8-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a5eb8-133">displayName</span></span>|<span data-ttu-id="a5eb8-134">string</span><span class="sxs-lookup"><span data-stu-id="a5eb8-134">string</span></span>|<span data-ttu-id="a5eb8-135">Отображаемое имя административной единицы.</span><span class="sxs-lookup"><span data-stu-id="a5eb8-135">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="a5eb8-136">visibility</span><span class="sxs-lookup"><span data-stu-id="a5eb8-136">visibility</span></span>|<span data-ttu-id="a5eb8-137">string</span><span class="sxs-lookup"><span data-stu-id="a5eb8-137">string</span></span>|<span data-ttu-id="a5eb8-138">Видимость административной единицы.</span><span class="sxs-lookup"><span data-stu-id="a5eb8-138">Visibility for the administrative unit.</span></span> <span data-ttu-id="a5eb8-139">Если не задано, то значение по умолчанию — "общедоступный".</span><span class="sxs-lookup"><span data-stu-id="a5eb8-139">If not set then the default is "public".</span></span> <span data-ttu-id="a5eb8-140">Может иметь значение "значение hiddenmembership", которое скрывает членство в группах, не являющихся участниками.</span><span class="sxs-lookup"><span data-stu-id="a5eb8-140">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="a5eb8-141">Так как ресурс **administrativeUnit** поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, зависящие от приложения, в пользовательских свойствах расширения в существующем экземпляре **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="a5eb8-141">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="a5eb8-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5eb8-142">Response</span></span>

<span data-ttu-id="a5eb8-143">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a5eb8-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a5eb8-144">Пример</span><span class="sxs-lookup"><span data-stu-id="a5eb8-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a5eb8-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5eb8-145">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a5eb8-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5eb8-146">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a5eb8-147">C#</span><span class="sxs-lookup"><span data-stu-id="a5eb8-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5eb8-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="a5eb8-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a5eb8-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a5eb8-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a5eb8-150">Java</span><span class="sxs-lookup"><span data-stu-id="a5eb8-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a5eb8-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="a5eb8-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="a5eb8-152">См. также</span><span class="sxs-lookup"><span data-stu-id="a5eb8-152">See also</span></span>

- [<span data-ttu-id="a5eb8-153">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="a5eb8-153">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a5eb8-154">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="a5eb8-154">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
