---
title: Обновление schemaExtension
description: Обновление свойств в определении указанного schemaExtension.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 3fd6ed535c2d6a30f85c8b46930a96c7cc8cee8f
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896583"
---
# <a name="update-schemaextension"></a><span data-ttu-id="3c705-103">Обновление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="3c705-103">Update schemaExtension</span></span>

<span data-ttu-id="3c705-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c705-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c705-105">Обновление свойств в определении указанного [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="3c705-105">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="3c705-106">Обновление применяется ко всем ресурсам, включенным в свойство **TargetType** расширения.</span><span class="sxs-lookup"><span data-stu-id="3c705-106">The update applies to all the resources that are included in the **targetTypes** property of the extension.</span></span> <span data-ttu-id="3c705-107">Эти ресурсы относятся к [типам вспомогательных ресурсов](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="3c705-107">These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="3c705-108">Только приложение, которое создало расширение схемы (приложение-владелец), может вносить добавочные обновления расширения, когда расширение находится в состоянии " **разрабатывает** " или " **доступно** ".</span><span class="sxs-lookup"><span data-stu-id="3c705-108">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status.</span></span> <span data-ttu-id="3c705-109">Это означает, что приложение не может удалять настраиваемые свойства или целевые типы ресурсов из определения.</span><span class="sxs-lookup"><span data-stu-id="3c705-109">That means the app cannot remove custom properties or target resource types from the definition.</span></span> <span data-ttu-id="3c705-110">Однако приложение может изменить описание расширения.</span><span class="sxs-lookup"><span data-stu-id="3c705-110">The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c705-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c705-111">Permissions</span></span>

<span data-ttu-id="3c705-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c705-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3c705-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c705-114">Permission type</span></span>      | <span data-ttu-id="3c705-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c705-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c705-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c705-116">Delegated (work or school account)</span></span> | <span data-ttu-id="3c705-117">Application. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="3c705-117">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3c705-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c705-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c705-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c705-119">Not supported.</span></span>    |
|<span data-ttu-id="3c705-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c705-120">Application</span></span> | <span data-ttu-id="3c705-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c705-121">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="3c705-122">Кроме того, для делегированного процесса вошедшего в систему пользователь может обновлять только schemaExtensions, которыми они владеют (где свойство **owner** объекта schemaExtension — это `appId` приложение, которому принадлежит вошедшего пользователь).</span><span class="sxs-lookup"><span data-stu-id="3c705-122">Additionally for the delegated flow, the signed-in user can only update schemaExtensions they own (where the **owner** property of the schemaExtension is the `appId` of an application the signed-in user owns).</span></span>

## <a name="http-request"></a><span data-ttu-id="3c705-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c705-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="3c705-124">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c705-124">Optional request headers</span></span>

| <span data-ttu-id="3c705-125">Имя</span><span class="sxs-lookup"><span data-stu-id="3c705-125">Name</span></span>      |<span data-ttu-id="3c705-126">Описание</span><span class="sxs-lookup"><span data-stu-id="3c705-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3c705-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c705-127">Authorization</span></span>  | <span data-ttu-id="3c705-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c705-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3c705-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3c705-130">Content-Type</span></span>   | <span data-ttu-id="3c705-131">application/json</span><span class="sxs-lookup"><span data-stu-id="3c705-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c705-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c705-132">Request body</span></span>

<span data-ttu-id="3c705-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3c705-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3c705-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c705-136">Property</span></span>   | <span data-ttu-id="3c705-137">Тип</span><span class="sxs-lookup"><span data-stu-id="3c705-137">Type</span></span> |<span data-ttu-id="3c705-138">Описание</span><span class="sxs-lookup"><span data-stu-id="3c705-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c705-139">description</span><span class="sxs-lookup"><span data-stu-id="3c705-139">description</span></span>|<span data-ttu-id="3c705-140">String</span><span class="sxs-lookup"><span data-stu-id="3c705-140">String</span></span>|<span data-ttu-id="3c705-141">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="3c705-141">Description for the schema extension.</span></span>|
|<span data-ttu-id="3c705-142">properties</span><span class="sxs-lookup"><span data-stu-id="3c705-142">properties</span></span>|<span data-ttu-id="3c705-143">Коллекция [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="3c705-143">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="3c705-144">Коллекция типов и имен свойств, составляющих определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="3c705-144">The collection of property names and types that make up the schema extension definition.</span></span> <span data-ttu-id="3c705-145">Разрешены только добавочные изменения.</span><span class="sxs-lookup"><span data-stu-id="3c705-145">Only additive changes are permitted.</span></span> |
|<span data-ttu-id="3c705-146">status</span><span class="sxs-lookup"><span data-stu-id="3c705-146">status</span></span>|<span data-ttu-id="3c705-147">String</span><span class="sxs-lookup"><span data-stu-id="3c705-147">String</span></span>|<span data-ttu-id="3c705-148">Состояние жизненного цикла расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="3c705-148">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="3c705-149">Начальное состояние при создании **разрабатывается**.</span><span class="sxs-lookup"><span data-stu-id="3c705-149">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="3c705-150">Переход между состояниями возможен из **разработки** в **доступном** и **доступном** для **устаревших**состояниях.</span><span class="sxs-lookup"><span data-stu-id="3c705-150">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="3c705-151">targetTypes</span><span class="sxs-lookup"><span data-stu-id="3c705-151">targetTypes</span></span>|<span data-ttu-id="3c705-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3c705-152">String collection</span></span>|<span data-ttu-id="3c705-153">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.</span><span class="sxs-lookup"><span data-stu-id="3c705-153">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span>  <span data-ttu-id="3c705-154">Разрешены только добавочные изменения.</span><span class="sxs-lookup"><span data-stu-id="3c705-154">Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="3c705-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c705-155">Response</span></span>

<span data-ttu-id="3c705-156">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3c705-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3c705-157">Пример</span><span class="sxs-lookup"><span data-stu-id="3c705-157">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3c705-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c705-158">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3c705-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c705-159">HTTP</span></span>](#tab/http)
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
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="3c705-160">C#</span><span class="sxs-lookup"><span data-stu-id="3c705-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c705-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c705-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c705-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c705-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3c705-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c705-163">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="3c705-164">См. также</span><span class="sxs-lookup"><span data-stu-id="3c705-164">See also</span></span>

- [<span data-ttu-id="3c705-165">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="3c705-165">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="3c705-166">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="3c705-166">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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
