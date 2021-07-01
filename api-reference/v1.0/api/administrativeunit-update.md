---
title: Обновление администрирования
description: Обновление свойств объекта administrativeUnit.
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0921bc6366d34278d23701d11ddb21bf0793d219
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208213"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="06f89-103">Обновление администрирования</span><span class="sxs-lookup"><span data-stu-id="06f89-103">Update administrativeunit</span></span>

<span data-ttu-id="06f89-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06f89-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="06f89-105">Обновление свойств объекта [administrativeUnit.](../resources/administrativeunit.md)</span><span class="sxs-lookup"><span data-stu-id="06f89-105">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="06f89-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06f89-106">Permissions</span></span>
<span data-ttu-id="06f89-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06f89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="06f89-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06f89-109">Permission type</span></span>      | <span data-ttu-id="06f89-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06f89-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06f89-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06f89-111">Delegated (work or school account)</span></span> | <span data-ttu-id="06f89-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="06f89-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="06f89-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06f89-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06f89-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06f89-114">Not supported.</span></span>    |
|<span data-ttu-id="06f89-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="06f89-115">Application</span></span> | <span data-ttu-id="06f89-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06f89-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06f89-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06f89-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /directory/administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="06f89-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06f89-118">Request headers</span></span>

| <span data-ttu-id="06f89-119">Имя</span><span class="sxs-lookup"><span data-stu-id="06f89-119">Name</span></span>      |<span data-ttu-id="06f89-120">Описание</span><span class="sxs-lookup"><span data-stu-id="06f89-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="06f89-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06f89-121">Authorization</span></span>  | <span data-ttu-id="06f89-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06f89-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="06f89-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06f89-124">Content-type</span></span> | <span data-ttu-id="06f89-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06f89-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06f89-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06f89-127">Request body</span></span>

<span data-ttu-id="06f89-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="06f89-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="06f89-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="06f89-131">Property</span></span>   | <span data-ttu-id="06f89-132">Тип</span><span class="sxs-lookup"><span data-stu-id="06f89-132">Type</span></span> |<span data-ttu-id="06f89-133">Описание</span><span class="sxs-lookup"><span data-stu-id="06f89-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06f89-134">description</span><span class="sxs-lookup"><span data-stu-id="06f89-134">description</span></span>|<span data-ttu-id="06f89-135">строка</span><span class="sxs-lookup"><span data-stu-id="06f89-135">string</span></span>|<span data-ttu-id="06f89-136">Описание административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="06f89-136">Description for the administrative unit.</span></span>|
|<span data-ttu-id="06f89-137">displayName</span><span class="sxs-lookup"><span data-stu-id="06f89-137">displayName</span></span>|<span data-ttu-id="06f89-138">string</span><span class="sxs-lookup"><span data-stu-id="06f89-138">string</span></span>|<span data-ttu-id="06f89-139">Отображение имени административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="06f89-139">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="06f89-140">visibility</span><span class="sxs-lookup"><span data-stu-id="06f89-140">visibility</span></span>|<span data-ttu-id="06f89-141">string</span><span class="sxs-lookup"><span data-stu-id="06f89-141">string</span></span>|<span data-ttu-id="06f89-142">Видимость для административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="06f89-142">Visibility for the administrative unit.</span></span> <span data-ttu-id="06f89-143">Если не установить, то по умолчанию является "общедоступным".</span><span class="sxs-lookup"><span data-stu-id="06f89-143">If not set then the default is "public".</span></span> <span data-ttu-id="06f89-144">Можно установить "HiddenMembership", которое скрывает членство от нечленов.</span><span class="sxs-lookup"><span data-stu-id="06f89-144">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="06f89-145">Так как ресурс **administrativeUnit** поддерживает [расширения,](/graph/extensibility-overview)вы можете использовать операцию для добавления, обновления или удаления собственных данных, определенных для приложения, в настраиваемом свойстве расширения в существующем экземпляре `PATCH` **administrativeUnit.**</span><span class="sxs-lookup"><span data-stu-id="06f89-145">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="06f89-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="06f89-146">Response</span></span>

<span data-ttu-id="06f89-147">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="06f89-147">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="06f89-148">Пример</span><span class="sxs-lookup"><span data-stu-id="06f89-148">Example</span></span>

##### <a name="request"></a><span data-ttu-id="06f89-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="06f89-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="06f89-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="06f89-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="06f89-151">C#</span><span class="sxs-lookup"><span data-stu-id="06f89-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06f89-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06f89-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06f89-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06f89-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06f89-154">Java</span><span class="sxs-lookup"><span data-stu-id="06f89-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


##### <a name="response"></a><span data-ttu-id="06f89-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="06f89-155">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="06f89-156">См. также</span><span class="sxs-lookup"><span data-stu-id="06f89-156">See also</span></span>

- [<span data-ttu-id="06f89-157">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="06f89-157">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="06f89-158">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="06f89-158">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
