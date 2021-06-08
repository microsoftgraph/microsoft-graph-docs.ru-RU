---
title: Обновление schemaExtension
description: Обновление свойств в определении указанной схемыExtension.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 6e5bef7a1ac978ccde1c84a9ee074d7fc6d91c28
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787384"
---
# <a name="update-schemaextension"></a><span data-ttu-id="bd25c-103">Обновление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="bd25c-103">Update schemaExtension</span></span>

<span data-ttu-id="bd25c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd25c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd25c-105">Обновление свойств в определении указанной [схемыExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="bd25c-105">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span> <span data-ttu-id="bd25c-106">Присадки к расширению могут быть сделаны только в том случае, если расширение находится в состоянии **InDevelopment** или **Available.**</span><span class="sxs-lookup"><span data-stu-id="bd25c-106">Additive updates to the extension can only be made when the extension is in the **InDevelopment** or **Available** status.</span></span> <span data-ttu-id="bd25c-107">Это означает, что настраиваемые свойства или типы целевых ресурсов не могут быть удалены из определения, но можно добавить новые настраиваемые свойства и изменить описание расширения.</span><span class="sxs-lookup"><span data-stu-id="bd25c-107">This means custom properties or target resource types cannot be removed from the definition, but new custom properties can be added and the description of the extension changed.</span></span>

<span data-ttu-id="bd25c-108">Обновление применяется ко всем ресурсам, включенным в **свойство targetTypes** расширения.</span><span class="sxs-lookup"><span data-stu-id="bd25c-108">The update applies to all the resources that are included in the **targetTypes** property of the extension.</span></span> <span data-ttu-id="bd25c-109">Эти ресурсы являются одними из [вспомогательных типов ресурсов.](/graph/extensibility-overview#supported-resources)</span><span class="sxs-lookup"><span data-stu-id="bd25c-109">These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="bd25c-110">Для делегирования потоков подписанный пользователь может обновить расширение схемы  до тех пор, пока  свойство владельца расширения задано приложению, владельцем приложения, которое принадлежит подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bd25c-110">For delegated flows, the signed-in user can update a schema extension as long as the **owner** property of the extension is set to the **appId** of an application the signed-in user owns.</span></span> <span data-ttu-id="bd25c-111">Это приложение может быть тем, которое изначально создало расширение, или каким-либо другим приложением, которое принадлежит подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bd25c-111">That application can be the one that initially created the extension, or some other application owned by the signed-in user.</span></span> 

<span data-ttu-id="bd25c-112">Этот критерий  для свойства владельца позволяет подписанного пользователя делать обновления через другие приложения, которыми они не владеют, например Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="bd25c-112">This criteria for the **owner** property allows a signed-in user to make updates through other applications they don't own, such as Microsoft Graph Explorer.</span></span> <span data-ttu-id="bd25c-113">При использовании Graph Explorer для обновления ресурса **schemaExtension** включаем свойство владельца в тело запроса PATCH. </span><span class="sxs-lookup"><span data-stu-id="bd25c-113">When using Graph Explorer to update a **schemaExtension** resource, include the **owner** property in the PATCH request body.</span></span> <span data-ttu-id="bd25c-114">Дополнительные сведения см. в разделе [Расширения](/graph/known-issues#extensions) в [разделе Известные](/graph/known-issues)проблемы с Microsoft Graph .</span><span class="sxs-lookup"><span data-stu-id="bd25c-114">For more information, see the [Extensions](/graph/known-issues#extensions) section in [Known issues with Microsoft Graph](/graph/known-issues).</span></span>

## <a name="permissions"></a><span data-ttu-id="bd25c-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd25c-115">Permissions</span></span>

<span data-ttu-id="bd25c-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd25c-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bd25c-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd25c-118">Permission type</span></span>      | <span data-ttu-id="bd25c-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd25c-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd25c-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd25c-120">Delegated (work or school account)</span></span> | <span data-ttu-id="bd25c-121">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bd25c-121">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bd25c-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd25c-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd25c-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd25c-123">Not supported.</span></span>    |
|<span data-ttu-id="bd25c-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd25c-124">Application</span></span> | <span data-ttu-id="bd25c-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd25c-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd25c-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd25c-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="bd25c-127">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd25c-127">Optional request headers</span></span>

| <span data-ttu-id="bd25c-128">Имя</span><span class="sxs-lookup"><span data-stu-id="bd25c-128">Name</span></span>      |<span data-ttu-id="bd25c-129">Описание</span><span class="sxs-lookup"><span data-stu-id="bd25c-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bd25c-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd25c-130">Authorization</span></span>  | <span data-ttu-id="bd25c-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd25c-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bd25c-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bd25c-133">Content-Type</span></span>   | <span data-ttu-id="bd25c-134">application/json</span><span class="sxs-lookup"><span data-stu-id="bd25c-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd25c-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd25c-135">Request body</span></span>

<span data-ttu-id="bd25c-p107">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="bd25c-p107">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bd25c-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd25c-139">Property</span></span>   | <span data-ttu-id="bd25c-140">Тип</span><span class="sxs-lookup"><span data-stu-id="bd25c-140">Type</span></span> |<span data-ttu-id="bd25c-141">Описание</span><span class="sxs-lookup"><span data-stu-id="bd25c-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd25c-142">description</span><span class="sxs-lookup"><span data-stu-id="bd25c-142">description</span></span>|<span data-ttu-id="bd25c-143">String</span><span class="sxs-lookup"><span data-stu-id="bd25c-143">String</span></span>|<span data-ttu-id="bd25c-144">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="bd25c-144">Description for the schema extension.</span></span>|
|<span data-ttu-id="bd25c-145">properties</span><span class="sxs-lookup"><span data-stu-id="bd25c-145">properties</span></span>|<span data-ttu-id="bd25c-146">Коллекция [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="bd25c-146">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="bd25c-147">Коллекция типов и имен свойств, составляющих определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="bd25c-147">The collection of property names and types that make up the schema extension definition.</span></span> <span data-ttu-id="bd25c-148">Разрешены только изменения добавок.</span><span class="sxs-lookup"><span data-stu-id="bd25c-148">Only additive changes are permitted.</span></span> |
|<span data-ttu-id="bd25c-149">status</span><span class="sxs-lookup"><span data-stu-id="bd25c-149">status</span></span>|<span data-ttu-id="bd25c-150">String</span><span class="sxs-lookup"><span data-stu-id="bd25c-150">String</span></span>|<span data-ttu-id="bd25c-151">Состояние жизненного цикла расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="bd25c-151">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="bd25c-152">Начальное состояние при создании — **InDevelopment**.</span><span class="sxs-lookup"><span data-stu-id="bd25c-152">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="bd25c-153">Возможные переходы состояния из **InDevelopment** в **доступные и** **доступные** **для deprecated**.</span><span class="sxs-lookup"><span data-stu-id="bd25c-153">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="bd25c-154">targetTypes</span><span class="sxs-lookup"><span data-stu-id="bd25c-154">targetTypes</span></span>|<span data-ttu-id="bd25c-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bd25c-155">String collection</span></span>|<span data-ttu-id="bd25c-156">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.</span><span class="sxs-lookup"><span data-stu-id="bd25c-156">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span>  <span data-ttu-id="bd25c-157">Разрешены только изменения добавок.</span><span class="sxs-lookup"><span data-stu-id="bd25c-157">Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="bd25c-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd25c-158">Response</span></span>

<span data-ttu-id="bd25c-159">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bd25c-159">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bd25c-160">Пример</span><span class="sxs-lookup"><span data-stu-id="bd25c-160">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bd25c-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd25c-161">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="bd25c-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd25c-162">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bd25c-163">C#</span><span class="sxs-lookup"><span data-stu-id="bd25c-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd25c-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd25c-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd25c-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd25c-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd25c-166">Java</span><span class="sxs-lookup"><span data-stu-id="bd25c-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bd25c-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd25c-167">Response</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="bd25c-168">См. также</span><span class="sxs-lookup"><span data-stu-id="bd25c-168">See also</span></span>

- [<span data-ttu-id="bd25c-169">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="bd25c-169">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="bd25c-170">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="bd25c-170">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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


