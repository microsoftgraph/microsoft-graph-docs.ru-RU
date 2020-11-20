---
title: Обновление schemaExtension
description: Обновление свойств в определении указанного schemaExtension.
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: ac657ee517a11201cab50c8aa161ad20c9352ff8
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352447"
---
# <a name="update-schemaextension"></a><span data-ttu-id="d72da-103">Обновление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="d72da-103">Update schemaExtension</span></span>

<span data-ttu-id="d72da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d72da-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d72da-105">Обновление свойств в определении указанного [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="d72da-105">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span> 

<span data-ttu-id="d72da-106">Это означает, что пользовательские свойства или целевые типы ресурсов невозможно удалить из определения, но можно добавить новые настраиваемые свойства, а также изменить описание расширения.</span><span class="sxs-lookup"><span data-stu-id="d72da-106">This means custom properties or target resource types cannot be removed from the definition, but new custom properties can be added and the description of the extension changed.</span></span>

<span data-ttu-id="d72da-107">Добавочные обновления расширения можно выполнить только в том случае, если расширение находится в состоянии "в **разработке** " или " **доступно** ".</span><span class="sxs-lookup"><span data-stu-id="d72da-107">Additive updates to the extension can only be made when the extension is in the **InDevelopment** or **Available** status.</span></span> 

<span data-ttu-id="d72da-108">Обновление применяется ко всем ресурсам, включенным в свойство **TargetType** расширения.</span><span class="sxs-lookup"><span data-stu-id="d72da-108">The update applies to all the resources that are included in the **targetTypes** property of the extension.</span></span> <span data-ttu-id="d72da-109">Эти ресурсы относятся к [типам вспомогательных ресурсов](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="d72da-109">These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="d72da-110">Для делегированных потоков пользователь, вошедшего в систему, может обновить расширение схемы, если для свойства **owner** расширения задано значение **AppID** приложения, которому принадлежит вошедшего пользователь.</span><span class="sxs-lookup"><span data-stu-id="d72da-110">For delegated flows, the signed-in user can update a schema extension as long as the **owner** property of the extension is set to the **appId** of an application the signed-in user owns.</span></span> <span data-ttu-id="d72da-111">Это может быть приложение, которое изначально создало расширение, или другое приложение, принадлежащее пользователю, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="d72da-111">That application can be the one that initially created the extension, or some other application owned by the signed-in user.</span></span> 

<span data-ttu-id="d72da-112">Этот критерий для свойства **owner** позволяет вошедшего в систему пользователю вносить изменения в другие приложения, которыми они не владеет, например, Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="d72da-112">This criteria for the **owner** property allows a signed-in user to make updates through other applications they don't own, such as Microsoft Graph Explorer.</span></span> <span data-ttu-id="d72da-113">При использовании проводника Graph для обновления ресурса **schemaExtension** Включите свойство **owner** в текст запроса PATCH.</span><span class="sxs-lookup"><span data-stu-id="d72da-113">When using Graph Explorer to update a **schemaExtension** resource, include the **owner** property in the PATCH request body.</span></span> <span data-ttu-id="d72da-114">Для получения дополнительных сведений см раздел [Extensions](/graph/known-issues#extensions) in [Известные проблемы в Microsoft Graph](/graph/known-issues).</span><span class="sxs-lookup"><span data-stu-id="d72da-114">For more information, see the [Extensions](/graph/known-issues#extensions) section in [Known issues with Microsoft Graph](/graph/known-issues).</span></span>

## <a name="permissions"></a><span data-ttu-id="d72da-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d72da-115">Permissions</span></span>
<span data-ttu-id="d72da-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d72da-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d72da-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d72da-118">Permission type</span></span>      | <span data-ttu-id="d72da-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d72da-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d72da-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d72da-120">Delegated (work or school account)</span></span> | <span data-ttu-id="d72da-121">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d72da-121">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d72da-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d72da-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d72da-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d72da-123">Not supported.</span></span>    |
|<span data-ttu-id="d72da-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d72da-124">Application</span></span> | <span data-ttu-id="d72da-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d72da-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d72da-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d72da-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="d72da-127">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d72da-127">Optional request headers</span></span>

| <span data-ttu-id="d72da-128">Имя</span><span class="sxs-lookup"><span data-stu-id="d72da-128">Name</span></span>      |<span data-ttu-id="d72da-129">Описание</span><span class="sxs-lookup"><span data-stu-id="d72da-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d72da-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d72da-130">Authorization</span></span>  | <span data-ttu-id="d72da-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d72da-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d72da-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d72da-133">Content-Type</span></span>   | <span data-ttu-id="d72da-134">application/json</span><span class="sxs-lookup"><span data-stu-id="d72da-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d72da-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d72da-135">Request body</span></span>

<span data-ttu-id="d72da-p106">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d72da-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d72da-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="d72da-139">Property</span></span>   | <span data-ttu-id="d72da-140">Тип</span><span class="sxs-lookup"><span data-stu-id="d72da-140">Type</span></span> |<span data-ttu-id="d72da-141">Описание</span><span class="sxs-lookup"><span data-stu-id="d72da-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d72da-142">description</span><span class="sxs-lookup"><span data-stu-id="d72da-142">description</span></span>|<span data-ttu-id="d72da-143">String</span><span class="sxs-lookup"><span data-stu-id="d72da-143">String</span></span>|<span data-ttu-id="d72da-144">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="d72da-144">Description for the schema extension.</span></span>|
|<span data-ttu-id="d72da-145">properties</span><span class="sxs-lookup"><span data-stu-id="d72da-145">properties</span></span>|<span data-ttu-id="d72da-146">Коллекция [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="d72da-146">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="d72da-147">Коллекция типов и имен свойств, составляющих определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="d72da-147">The collection of property names and types that make up the schema extension definition.</span></span> <span data-ttu-id="d72da-148">Разрешены только добавочные изменения.</span><span class="sxs-lookup"><span data-stu-id="d72da-148">Only additive changes are permitted.</span></span> |
|<span data-ttu-id="d72da-149">status</span><span class="sxs-lookup"><span data-stu-id="d72da-149">status</span></span>|<span data-ttu-id="d72da-150">String</span><span class="sxs-lookup"><span data-stu-id="d72da-150">String</span></span>|<span data-ttu-id="d72da-151">Состояние жизненного цикла расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="d72da-151">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="d72da-152">Начальное состояние при создании **разрабатывается**.</span><span class="sxs-lookup"><span data-stu-id="d72da-152">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="d72da-153">Переход между состояниями возможен из **разработки** в **доступном** и **доступном** для **устаревших** состояниях.</span><span class="sxs-lookup"><span data-stu-id="d72da-153">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="d72da-154">targetTypes</span><span class="sxs-lookup"><span data-stu-id="d72da-154">targetTypes</span></span>|<span data-ttu-id="d72da-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d72da-155">String collection</span></span>|<span data-ttu-id="d72da-156">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.</span><span class="sxs-lookup"><span data-stu-id="d72da-156">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span>  <span data-ttu-id="d72da-157">Разрешены только добавочные изменения.</span><span class="sxs-lookup"><span data-stu-id="d72da-157">Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="d72da-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="d72da-158">Response</span></span>

<span data-ttu-id="d72da-159">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d72da-159">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d72da-160">Пример</span><span class="sxs-lookup"><span data-stu-id="d72da-160">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d72da-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="d72da-161">Request</span></span>

<span data-ttu-id="d72da-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d72da-162">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d72da-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="d72da-163">HTTP</span></span>](#tab/http)
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
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="d72da-164">C#</span><span class="sxs-lookup"><span data-stu-id="d72da-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d72da-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d72da-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d72da-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d72da-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d72da-167">Java</span><span class="sxs-lookup"><span data-stu-id="d72da-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d72da-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="d72da-168">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="d72da-169">См. также</span><span class="sxs-lookup"><span data-stu-id="d72da-169">See also</span></span>

- [<span data-ttu-id="d72da-170">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="d72da-170">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d72da-171">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="d72da-171">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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

