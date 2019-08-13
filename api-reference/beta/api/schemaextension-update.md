---
title: Обновление schemaExtension
description: Обновление свойств в определении указанного schemaExtension.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 7c8cdcec64d8d0e65f069df3daa8af2fa4670066
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364385"
---
# <a name="update-schemaextension"></a><span data-ttu-id="4dba9-103">Обновление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="4dba9-103">Update schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dba9-104">Обновление свойств в определении указанного [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="4dba9-104">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="4dba9-105">Обновление применяется ко всем ресурсам, включенным в свойство **TargetType** расширения.</span><span class="sxs-lookup"><span data-stu-id="4dba9-105">The update applies to all the resources that are included in the **targetTypes** property of the extension.</span></span> <span data-ttu-id="4dba9-106">Эти ресурсы относятся к [типам вспомогательных ресурсов](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="4dba9-106">These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="4dba9-107">Только приложение, которое создало расширение схемы (приложение-владелец), может вносить добавочные обновления расширения, когда расширение находится в \*\*\*\* состоянии "разрабатывает" или " **доступно** ".</span><span class="sxs-lookup"><span data-stu-id="4dba9-107">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status.</span></span> <span data-ttu-id="4dba9-108">Это означает, что приложение не может удалять настраиваемые свойства или целевые типы ресурсов из определения.</span><span class="sxs-lookup"><span data-stu-id="4dba9-108">That means the app cannot remove custom properties or target resource types from the definition.</span></span> <span data-ttu-id="4dba9-109">Однако приложение может изменить описание расширения.</span><span class="sxs-lookup"><span data-stu-id="4dba9-109">The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="4dba9-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4dba9-110">Permissions</span></span>

<span data-ttu-id="4dba9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dba9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4dba9-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4dba9-113">Permission type</span></span>      | <span data-ttu-id="4dba9-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4dba9-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4dba9-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4dba9-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4dba9-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4dba9-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4dba9-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4dba9-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4dba9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dba9-118">Not supported.</span></span>    |
|<span data-ttu-id="4dba9-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4dba9-119">Application</span></span> | <span data-ttu-id="4dba9-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dba9-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4dba9-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4dba9-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="4dba9-122">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4dba9-122">Optional request headers</span></span>

| <span data-ttu-id="4dba9-123">Имя</span><span class="sxs-lookup"><span data-stu-id="4dba9-123">Name</span></span>      |<span data-ttu-id="4dba9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4dba9-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4dba9-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4dba9-125">Authorization</span></span>  | <span data-ttu-id="4dba9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4dba9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4dba9-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4dba9-128">Content-Type</span></span>   | <span data-ttu-id="4dba9-129">application/json</span><span class="sxs-lookup"><span data-stu-id="4dba9-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4dba9-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4dba9-130">Request body</span></span>

<span data-ttu-id="4dba9-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4dba9-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4dba9-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="4dba9-134">Property</span></span>   | <span data-ttu-id="4dba9-135">Тип</span><span class="sxs-lookup"><span data-stu-id="4dba9-135">Type</span></span> |<span data-ttu-id="4dba9-136">Описание</span><span class="sxs-lookup"><span data-stu-id="4dba9-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4dba9-137">description</span><span class="sxs-lookup"><span data-stu-id="4dba9-137">description</span></span>|<span data-ttu-id="4dba9-138">String</span><span class="sxs-lookup"><span data-stu-id="4dba9-138">String</span></span>|<span data-ttu-id="4dba9-139">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="4dba9-139">Description for the schema extension.</span></span>|
|<span data-ttu-id="4dba9-140">properties</span><span class="sxs-lookup"><span data-stu-id="4dba9-140">properties</span></span>|<span data-ttu-id="4dba9-141">Коллекция [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="4dba9-141">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="4dba9-142">Коллекция типов и имен свойств, составляющих определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="4dba9-142">The collection of property names and types that make up the schema extension definition.</span></span> <span data-ttu-id="4dba9-143">Разрешены только добавочные изменения.</span><span class="sxs-lookup"><span data-stu-id="4dba9-143">Only additive changes are permitted.</span></span> |
|<span data-ttu-id="4dba9-144">status</span><span class="sxs-lookup"><span data-stu-id="4dba9-144">status</span></span>|<span data-ttu-id="4dba9-145">String</span><span class="sxs-lookup"><span data-stu-id="4dba9-145">String</span></span>|<span data-ttu-id="4dba9-146">Состояние жизненного цикла расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="4dba9-146">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="4dba9-147">Начальное состояние при создании разрабатывается. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="4dba9-147">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="4dba9-148">Переход между состояниями возможен из **разработки** в **доступном** и **доступном** для **устаревших**состояниях.</span><span class="sxs-lookup"><span data-stu-id="4dba9-148">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="4dba9-149">targetTypes</span><span class="sxs-lookup"><span data-stu-id="4dba9-149">targetTypes</span></span>|<span data-ttu-id="4dba9-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4dba9-150">String collection</span></span>|<span data-ttu-id="4dba9-151">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.</span><span class="sxs-lookup"><span data-stu-id="4dba9-151">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span>  <span data-ttu-id="4dba9-152">Разрешены только добавочные изменения.</span><span class="sxs-lookup"><span data-stu-id="4dba9-152">Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="4dba9-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dba9-153">Response</span></span>

<span data-ttu-id="4dba9-154">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4dba9-154">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4dba9-155">Пример</span><span class="sxs-lookup"><span data-stu-id="4dba9-155">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4dba9-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dba9-156">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4dba9-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="4dba9-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/beta/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ],
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4dba9-158">C#</span><span class="sxs-lookup"><span data-stu-id="4dba9-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4dba9-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4dba9-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4dba9-160">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4dba9-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4dba9-161">Java</span><span class="sxs-lookup"><span data-stu-id="4dba9-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4dba9-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="4dba9-162">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="4dba9-163">См. также</span><span class="sxs-lookup"><span data-stu-id="4dba9-163">See also</span></span>

- [<span data-ttu-id="4dba9-164">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="4dba9-164">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4dba9-165">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="4dba9-165">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
