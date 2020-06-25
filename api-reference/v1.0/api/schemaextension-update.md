---
title: Обновление schemaExtension
description: Обновление свойств в определении указанного schemaExtension.
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 8cbf5264ad704dde5139f8915f9350ad189368a5
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864184"
---
# <a name="update-schemaextension"></a><span data-ttu-id="93e21-103">Обновление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="93e21-103">Update schemaExtension</span></span>

<span data-ttu-id="93e21-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93e21-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93e21-105">Обновление свойств в определении указанного [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="93e21-105">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="93e21-106">Обновление применяется ко всем ресурсам, включенным в свойство **TargetType** расширения.</span><span class="sxs-lookup"><span data-stu-id="93e21-106">The update applies to all the resources that are included in the **targetTypes** property of the extension.</span></span> <span data-ttu-id="93e21-107">Эти ресурсы относятся к [типам вспомогательных ресурсов](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="93e21-107">These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="93e21-108">Только приложение, которое создало расширение схемы (приложение-владелец), может вносить добавочные обновления расширения, когда расширение находится в состоянии " **разрабатывает** " или " **доступно** ".</span><span class="sxs-lookup"><span data-stu-id="93e21-108">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status.</span></span> <span data-ttu-id="93e21-109">Это означает, что приложение не может удалять настраиваемые свойства или целевые типы ресурсов из определения.</span><span class="sxs-lookup"><span data-stu-id="93e21-109">That means the app cannot remove custom properties or target resource types from the definition.</span></span> <span data-ttu-id="93e21-110">Однако приложение может изменить описание расширения.</span><span class="sxs-lookup"><span data-stu-id="93e21-110">The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="93e21-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93e21-111">Permissions</span></span>
<span data-ttu-id="93e21-112">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="93e21-112">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="93e21-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93e21-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="93e21-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93e21-114">Permission type</span></span>      | <span data-ttu-id="93e21-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93e21-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93e21-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93e21-116">Delegated (work or school account)</span></span> | <span data-ttu-id="93e21-117">Application. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="93e21-117">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="93e21-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93e21-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93e21-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93e21-119">Not supported.</span></span>    |
|<span data-ttu-id="93e21-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93e21-120">Application</span></span> | <span data-ttu-id="93e21-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93e21-121">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="93e21-122">Кроме того, для делегированного процесса вошедшего в систему пользователь может обновлять только schemaExtensions, которыми они владеют (где свойство **owner** объекта schemaExtension — это `appId` приложение, которому принадлежит вошедшего пользователь).</span><span class="sxs-lookup"><span data-stu-id="93e21-122">Additionally for the delegated flow, the signed-in user can only update schemaExtensions they own (where the **owner** property of the schemaExtension is the `appId` of an application the signed-in user owns).</span></span>

## <a name="http-request"></a><span data-ttu-id="93e21-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93e21-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="93e21-124">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93e21-124">Optional request headers</span></span>

| <span data-ttu-id="93e21-125">Имя</span><span class="sxs-lookup"><span data-stu-id="93e21-125">Name</span></span>      |<span data-ttu-id="93e21-126">Описание</span><span class="sxs-lookup"><span data-stu-id="93e21-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="93e21-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93e21-127">Authorization</span></span>  | <span data-ttu-id="93e21-128">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="93e21-128">Bearer {token}.</span></span> <span data-ttu-id="93e21-129">Required.</span><span class="sxs-lookup"><span data-stu-id="93e21-129">Required.</span></span> |
| <span data-ttu-id="93e21-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="93e21-130">Content-Type</span></span>   | <span data-ttu-id="93e21-131">application/json</span><span class="sxs-lookup"><span data-stu-id="93e21-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="93e21-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93e21-132">Request body</span></span>

<span data-ttu-id="93e21-133">In the request body, supply the values for relevant fields that should be updated.</span><span class="sxs-lookup"><span data-stu-id="93e21-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="93e21-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span><span class="sxs-lookup"><span data-stu-id="93e21-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="93e21-135">For best performance you shouldn't include existing values that haven't changed.</span><span class="sxs-lookup"><span data-stu-id="93e21-135">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="93e21-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="93e21-136">Property</span></span>   | <span data-ttu-id="93e21-137">Тип</span><span class="sxs-lookup"><span data-stu-id="93e21-137">Type</span></span> |<span data-ttu-id="93e21-138">Описание</span><span class="sxs-lookup"><span data-stu-id="93e21-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93e21-139">description</span><span class="sxs-lookup"><span data-stu-id="93e21-139">description</span></span>|<span data-ttu-id="93e21-140">String</span><span class="sxs-lookup"><span data-stu-id="93e21-140">String</span></span>|<span data-ttu-id="93e21-141">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="93e21-141">Description for the schema extension.</span></span>|
|<span data-ttu-id="93e21-142">properties</span><span class="sxs-lookup"><span data-stu-id="93e21-142">properties</span></span>|<span data-ttu-id="93e21-143">Коллекция [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="93e21-143">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="93e21-144">Коллекция типов и имен свойств, составляющих определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="93e21-144">The collection of property names and types that make up the schema extension definition.</span></span> <span data-ttu-id="93e21-145">Разрешены только добавочные изменения.</span><span class="sxs-lookup"><span data-stu-id="93e21-145">Only additive changes are permitted.</span></span> |
|<span data-ttu-id="93e21-146">status</span><span class="sxs-lookup"><span data-stu-id="93e21-146">status</span></span>|<span data-ttu-id="93e21-147">String</span><span class="sxs-lookup"><span data-stu-id="93e21-147">String</span></span>|<span data-ttu-id="93e21-148">Состояние жизненного цикла расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="93e21-148">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="93e21-149">Начальное состояние при создании **разрабатывается**.</span><span class="sxs-lookup"><span data-stu-id="93e21-149">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="93e21-150">Переход между состояниями возможен из **разработки** в **доступном** и **доступном** для **устаревших**состояниях.</span><span class="sxs-lookup"><span data-stu-id="93e21-150">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="93e21-151">targetTypes</span><span class="sxs-lookup"><span data-stu-id="93e21-151">targetTypes</span></span>|<span data-ttu-id="93e21-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="93e21-152">String collection</span></span>|<span data-ttu-id="93e21-153">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.</span><span class="sxs-lookup"><span data-stu-id="93e21-153">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span>  <span data-ttu-id="93e21-154">Разрешены только добавочные изменения.</span><span class="sxs-lookup"><span data-stu-id="93e21-154">Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="93e21-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="93e21-155">Response</span></span>

<span data-ttu-id="93e21-156">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="93e21-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="93e21-157">Пример</span><span class="sxs-lookup"><span data-stu-id="93e21-157">Example</span></span>

##### <a name="request"></a><span data-ttu-id="93e21-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="93e21-158">Request</span></span>

<span data-ttu-id="93e21-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93e21-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="93e21-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="93e21-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/schemaExtensions/{id}
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
# <a name="c"></a>[<span data-ttu-id="93e21-161">C#</span><span class="sxs-lookup"><span data-stu-id="93e21-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93e21-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93e21-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93e21-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93e21-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93e21-164">Java</span><span class="sxs-lookup"><span data-stu-id="93e21-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="93e21-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="93e21-165">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="93e21-166">См. также</span><span class="sxs-lookup"><span data-stu-id="93e21-166">See also</span></span>

- [<span data-ttu-id="93e21-167">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="93e21-167">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="93e21-168">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="93e21-168">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
