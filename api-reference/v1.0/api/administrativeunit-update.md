---
title: Обновление администрирования
description: Обновление свойств объекта administrativeUnit.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 195ae89d8f32659f975be172fcf586f0cc7a02eb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442574"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="dffa4-103">Обновление администрирования</span><span class="sxs-lookup"><span data-stu-id="dffa4-103">Update administrativeunit</span></span>

<span data-ttu-id="dffa4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dffa4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dffa4-105">Обновление свойств объекта [administrativeUnit.](../resources/administrativeunit.md)</span><span class="sxs-lookup"><span data-stu-id="dffa4-105">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dffa4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dffa4-106">Permissions</span></span>
<span data-ttu-id="dffa4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dffa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dffa4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dffa4-109">Permission type</span></span>      | <span data-ttu-id="dffa4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dffa4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dffa4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dffa4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dffa4-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dffa4-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dffa4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dffa4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dffa4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dffa4-114">Not supported.</span></span>    |
|<span data-ttu-id="dffa4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dffa4-115">Application</span></span> | <span data-ttu-id="dffa4-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dffa4-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dffa4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dffa4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /directory/administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dffa4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dffa4-118">Request headers</span></span>

| <span data-ttu-id="dffa4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dffa4-119">Name</span></span>      |<span data-ttu-id="dffa4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dffa4-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dffa4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dffa4-121">Authorization</span></span>  | <span data-ttu-id="dffa4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dffa4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dffa4-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dffa4-124">Request body</span></span>

<span data-ttu-id="dffa4-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="dffa4-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dffa4-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="dffa4-128">Property</span></span>   | <span data-ttu-id="dffa4-129">Тип</span><span class="sxs-lookup"><span data-stu-id="dffa4-129">Type</span></span> |<span data-ttu-id="dffa4-130">Описание</span><span class="sxs-lookup"><span data-stu-id="dffa4-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dffa4-131">description</span><span class="sxs-lookup"><span data-stu-id="dffa4-131">description</span></span>|<span data-ttu-id="dffa4-132">string</span><span class="sxs-lookup"><span data-stu-id="dffa4-132">string</span></span>|<span data-ttu-id="dffa4-133">Описание административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="dffa4-133">Description for the administrative unit.</span></span>|
|<span data-ttu-id="dffa4-134">displayName</span><span class="sxs-lookup"><span data-stu-id="dffa4-134">displayName</span></span>|<span data-ttu-id="dffa4-135">string</span><span class="sxs-lookup"><span data-stu-id="dffa4-135">string</span></span>|<span data-ttu-id="dffa4-136">Отображение имени административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="dffa4-136">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="dffa4-137">visibility</span><span class="sxs-lookup"><span data-stu-id="dffa4-137">visibility</span></span>|<span data-ttu-id="dffa4-138">string</span><span class="sxs-lookup"><span data-stu-id="dffa4-138">string</span></span>|<span data-ttu-id="dffa4-139">Видимость для административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="dffa4-139">Visibility for the administrative unit.</span></span> <span data-ttu-id="dffa4-140">Если не установить, то по умолчанию является "общедоступным".</span><span class="sxs-lookup"><span data-stu-id="dffa4-140">If not set then the default is "public".</span></span> <span data-ttu-id="dffa4-141">Можно установить "HiddenMembership", которое скрывает членство от нечленов.</span><span class="sxs-lookup"><span data-stu-id="dffa4-141">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="dffa4-142">Так как ресурс **administrativeUnit** поддерживает [расширения,](/graph/extensibility-overview)вы можете использовать операцию для добавления, обновления или удаления собственных данных, определенных для приложения, в настраиваемом свойстве расширения в существующем экземпляре `PATCH` **administrativeUnit.**</span><span class="sxs-lookup"><span data-stu-id="dffa4-142">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="dffa4-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="dffa4-143">Response</span></span>

<span data-ttu-id="dffa4-144">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dffa4-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dffa4-145">Пример</span><span class="sxs-lookup"><span data-stu-id="dffa4-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dffa4-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="dffa4-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dffa4-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="dffa4-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_administrativeunit"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}
Content-type: application/json
Content-length: 114

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value"
}
```
# <a name="c"></a>[<span data-ttu-id="dffa4-148">C#</span><span class="sxs-lookup"><span data-stu-id="dffa4-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dffa4-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dffa4-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dffa4-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dffa4-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dffa4-151">Java</span><span class="sxs-lookup"><span data-stu-id="dffa4-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


##### <a name="response"></a><span data-ttu-id="dffa4-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="dffa4-152">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="dffa4-153">См. также</span><span class="sxs-lookup"><span data-stu-id="dffa4-153">See also</span></span>

- [<span data-ttu-id="dffa4-154">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="dffa4-154">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="dffa4-155">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="dffa4-155">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
