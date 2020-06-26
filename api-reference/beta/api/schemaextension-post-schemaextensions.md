---
title: Создание schemaExtension
description: Создайте новое определение schemaExtension, чтобы расширить поддерживаемый тип ресурса.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: e84c7408eb6924205e86059c969201d1c94dcd70
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896526"
---
# <a name="create-schemaextension"></a><span data-ttu-id="b59ea-103">Создание schemaExtension</span><span class="sxs-lookup"><span data-stu-id="b59ea-103">Create schemaExtension</span></span>

<span data-ttu-id="b59ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b59ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b59ea-105">Создайте новое определение [schemaExtension](../resources/schemaextension.md), чтобы расширить [поддерживаемый тип ресурса](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="b59ea-105">Create a new [schemaExtension](../resources/schemaextension.md) definition to extend a [supporting resource type](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="b59ea-106">Schema extensions let you add strongly-typed custom data to a resource.</span><span class="sxs-lookup"><span data-stu-id="b59ea-106">Schema extensions let you add strongly-typed custom data to a resource.</span></span> <span data-ttu-id="b59ea-107">The app that creates a schema extension is the owner app.</span><span class="sxs-lookup"><span data-stu-id="b59ea-107">The app that creates a schema extension is the owner app.</span></span> <span data-ttu-id="b59ea-108">Depending on the [state](/graph/extensibility-overview#schema-extensions-lifecycle) of the extension, the owner app, and only the owner app, may update or delete the extension.</span><span class="sxs-lookup"><span data-stu-id="b59ea-108">Depending on the [state](/graph/extensibility-overview#schema-extensions-lifecycle) of the extension, the owner app, and only the owner app, may update or delete the extension.</span></span> 

<span data-ttu-id="b59ea-109">Ознакомьтесь с примерами того, как [определить расширение схемы, описывающее учебный курс](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course), использовать определение расширения схемы для [создания группы с данными учебного курса](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data) и [добавить данные учебного курса в существующую группу](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group).</span><span class="sxs-lookup"><span data-stu-id="b59ea-109">See examples of how to [define a schema extension that describes a training course](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course), use the schema extension definition to [create a new group with training course data](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data), and [add training course data to an existing group](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group).</span></span>

## <a name="permissions"></a><span data-ttu-id="b59ea-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b59ea-110">Permissions</span></span>
<span data-ttu-id="b59ea-111">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b59ea-111">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b59ea-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b59ea-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b59ea-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b59ea-113">Permission type</span></span>      | <span data-ttu-id="b59ea-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b59ea-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b59ea-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b59ea-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b59ea-116">Application. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="b59ea-116">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b59ea-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b59ea-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b59ea-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b59ea-118">Not supported.</span></span>    |
|<span data-ttu-id="b59ea-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b59ea-119">Application</span></span> | <span data-ttu-id="b59ea-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b59ea-120">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="b59ea-121">Кроме того, для делегированного процесса вошедшего пользователь должен быть владельцем вызывающего приложения или владельцем (приложением с), `appId` используемым для задания свойства **owner** .</span><span class="sxs-lookup"><span data-stu-id="b59ea-121">Additionally for the delegated flow, the signed-in user must be the owner of the calling application OR the owner of the (application with the) `appId` used to set the **owner** property.</span></span>

## <a name="http-request"></a><span data-ttu-id="b59ea-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b59ea-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /schemaExtensions
```

## <a name="request-headers"></a><span data-ttu-id="b59ea-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b59ea-123">Request headers</span></span>
| <span data-ttu-id="b59ea-124">Имя</span><span class="sxs-lookup"><span data-stu-id="b59ea-124">Name</span></span>       | <span data-ttu-id="b59ea-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b59ea-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b59ea-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b59ea-126">Authorization</span></span>  | <span data-ttu-id="b59ea-127">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="b59ea-127">Bearer {token}.</span></span> <span data-ttu-id="b59ea-128">Required.</span><span class="sxs-lookup"><span data-stu-id="b59ea-128">Required.</span></span> |
| <span data-ttu-id="b59ea-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b59ea-129">Content-Type</span></span>  | <span data-ttu-id="b59ea-130">application/json</span><span class="sxs-lookup"><span data-stu-id="b59ea-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b59ea-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b59ea-131">Request body</span></span>
<span data-ttu-id="b59ea-132">В теле запроса должно быть представление объекта [schemaExtension](../resources/schemaextension.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b59ea-132">In the request body, supply a JSON representation of [schemaExtension](../resources/schemaextension.md) object.</span></span>

<span data-ttu-id="b59ea-133">В следующей таблице приведены свойства, доступные при создании расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="b59ea-133">The following table shows the properties that are available when you create a schema extension.</span></span>

| <span data-ttu-id="b59ea-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="b59ea-134">Parameter</span></span> | <span data-ttu-id="b59ea-135">Тип</span><span class="sxs-lookup"><span data-stu-id="b59ea-135">Type</span></span> | <span data-ttu-id="b59ea-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b59ea-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b59ea-137">description</span><span class="sxs-lookup"><span data-stu-id="b59ea-137">description</span></span>|<span data-ttu-id="b59ea-138">String</span><span class="sxs-lookup"><span data-stu-id="b59ea-138">String</span></span>|<span data-ttu-id="b59ea-139">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="b59ea-139">Description for the schema extension.</span></span>|
|<span data-ttu-id="b59ea-140">id</span><span class="sxs-lookup"><span data-stu-id="b59ea-140">id</span></span>|<span data-ttu-id="b59ea-141">Строка</span><span class="sxs-lookup"><span data-stu-id="b59ea-141">String</span></span>|<span data-ttu-id="b59ea-142">Уникальный идентификатор для определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="b59ea-142">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="b59ea-143">Значение можно присвоить одним из двух способов:</span><span class="sxs-lookup"><span data-stu-id="b59ea-143">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="b59ea-144">Сцепите имя одного из ваших проверенных доменов с именем расширения схемы и создайте уникальную строку такого формата: \{_&#65279;доменноеИмя_\}\_\{_&#65279;имяСхемы_\}.</span><span class="sxs-lookup"><span data-stu-id="b59ea-144">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span> <span data-ttu-id="b59ea-145">Пример: `contoso_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="b59ea-145">As an example, `contoso_mySchema`.</span></span> <span data-ttu-id="b59ea-146">ПРИМЕЧАНИЕ. Поддерживаются только проверенные домены в следующих доменах верхнего уровня: `.com`,`.net`, `.gov`, `.edu` или `.org`.</span><span class="sxs-lookup"><span data-stu-id="b59ea-146">NOTE: Only verified domains under the following top-level domains are supported: `.com`,`.net`, `.gov`, `.edu` or `.org`.</span></span> </li><li><span data-ttu-id="b59ea-147">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}.</span><span class="sxs-lookup"><span data-stu-id="b59ea-147">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}.</span></span> <span data-ttu-id="b59ea-148">An example would be `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="b59ea-148">An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="b59ea-149">После создания это свойство невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="b59ea-149">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="b59ea-150">owner</span><span class="sxs-lookup"><span data-stu-id="b59ea-150">owner</span></span>|<span data-ttu-id="b59ea-151">String</span><span class="sxs-lookup"><span data-stu-id="b59ea-151">String</span></span>|<span data-ttu-id="b59ea-152">(Необязательный параметр) Идентификатор `appId` приложения, которое является владельцем расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="b59ea-152">(Optional) The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="b59ea-153">Это свойство можно указать при создании, чтобы задать владельца.</span><span class="sxs-lookup"><span data-stu-id="b59ea-153">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="b59ea-154">Если оно не указано, то в качестве владельца будет задано вызывающее приложение `appId`.</span><span class="sxs-lookup"><span data-stu-id="b59ea-154">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="b59ea-155">Таким образом, например, при создании определения расширения схемы с помощью песочницы Graph вам **потребуется** указать свойство владельца.</span><span class="sxs-lookup"><span data-stu-id="b59ea-155">So, for example, if creating a new schema extension definition using Graph Explorer, you **must** supply the owner property.</span></span> <span data-ttu-id="b59ea-156">После задания свойства оно будет доступно только для чтения, и вам не удастся изменить его.</span><span class="sxs-lookup"><span data-stu-id="b59ea-156">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="b59ea-157">properties</span><span class="sxs-lookup"><span data-stu-id="b59ea-157">properties</span></span>|<span data-ttu-id="b59ea-158">Коллекция [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="b59ea-158">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="b59ea-159">Коллекция типов и имен свойств, составляющих определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="b59ea-159">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="b59ea-160">targetTypes</span><span class="sxs-lookup"><span data-stu-id="b59ea-160">targetTypes</span></span>|<span data-ttu-id="b59ea-161">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b59ea-161">String collection</span></span>|<span data-ttu-id="b59ea-162">Набор типов ресурсов Microsoft Graph, поддерживающих расширения схемы, к которым может быть применимо данное определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="b59ea-162">Set of Microsoft Graph resource types (that support schema extensions) that this schema extension definition can be applied to.</span></span>|

## <a name="response"></a><span data-ttu-id="b59ea-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="b59ea-163">Response</span></span>

<span data-ttu-id="b59ea-164">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [schemaExtension](../resources/schemaextension.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b59ea-164">If successful, this method returns `201 Created` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b59ea-165">Пример</span><span class="sxs-lookup"><span data-stu-id="b59ea-165">Example</span></span>

### <a name="example-1-creating-a-schema-extension-using-a-verified-domain"></a><span data-ttu-id="b59ea-166">Пример 1: создание расширения схемы с помощью проверенного домена</span><span class="sxs-lookup"><span data-stu-id="b59ea-166">Example 1: Creating a schema extension using a verified domain</span></span>

#### <a name="request"></a><span data-ttu-id="b59ea-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="b59ea-167">Request</span></span>

<span data-ttu-id="b59ea-168">В этом примере показано использование проверенного имени домена, `graphlearn` а также имени схемы `courses` для формирования уникальной строки для свойства **ID** определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="b59ea-168">This example shows using a verified domain name, `graphlearn`, and a schema name, `courses`, to form a unique string for the **id** property of the schema extension definition.</span></span> <span data-ttu-id="b59ea-169">Уникальная строка основана на этом формате, \{ _&#65279;имя_домена_ \} \_ \{ _&#65279;schemaName_ \} .</span><span class="sxs-lookup"><span data-stu-id="b59ea-169">The unique string is based on this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span>

<span data-ttu-id="b59ea-170">В теле запроса должно быть представление объекта [schemaExtension](../resources/schemaextension.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b59ea-170">In the request body, supply a JSON representation of the [schemaExtension](../resources/schemaextension.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="b59ea-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="b59ea-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_1"
}-->
```http
POST https://graph.microsoft.com/beta/schemaExtensions
Content-type: application/json

{
    "id":"graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="b59ea-172">C#</span><span class="sxs-lookup"><span data-stu-id="b59ea-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b59ea-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b59ea-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b59ea-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b59ea-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b59ea-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="b59ea-175">Response</span></span>

<span data-ttu-id="b59ea-176">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="b59ea-176">Here is an example of the response.</span></span> <span data-ttu-id="b59ea-177">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b59ea-177">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b59ea-178">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b59ea-178">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

### <a name="example-2-creating-a-schema-extension-using-just-a-name"></a><span data-ttu-id="b59ea-179">Пример 2: создание расширения схемы с использованием всего имени</span><span class="sxs-lookup"><span data-stu-id="b59ea-179">Example 2: Creating a schema extension using just a name</span></span>

#### <a name="request"></a><span data-ttu-id="b59ea-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="b59ea-180">Request</span></span>

<span data-ttu-id="b59ea-181">В этом примере показано, как указать только имя схемы, `courses` в свойстве **ID** в запросе, вместе с представлением в формате JSON остальных свойств объекта [schemaExtension](../resources/schemaextension.md) .</span><span class="sxs-lookup"><span data-stu-id="b59ea-181">This example shows specifying just a schema name, `courses`, in the **id** property in the request, together with the JSON representation of the rest of the properties in the [schemaExtension](../resources/schemaextension.md) object.</span></span> <span data-ttu-id="b59ea-182">Microsoft Graph присвоит и возвращает уникальное строковое значение в отклике.</span><span class="sxs-lookup"><span data-stu-id="b59ea-182">Microsoft Graph will assign and return a unique string value in the response.</span></span>


# <a name="http"></a>[<span data-ttu-id="b59ea-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="b59ea-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_2"
}-->
```http
POST https://graph.microsoft.com/beta/schemaExtensions
Content-type: application/json

{
    "id":"courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="b59ea-184">C#</span><span class="sxs-lookup"><span data-stu-id="b59ea-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b59ea-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b59ea-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b59ea-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b59ea-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b59ea-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="b59ea-187">Response</span></span>

<span data-ttu-id="b59ea-188">The response includes a unique string in the **id** property that is based on the schema name provided in the request, together with the rest of the newly created schema definition.</span><span class="sxs-lookup"><span data-stu-id="b59ea-188">The response includes a unique string in the **id** property that is based on the schema name provided in the request, together with the rest of the newly created schema definition.</span></span> <span data-ttu-id="b59ea-189">The value in **id** in the response is based on the format, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}.</span><span class="sxs-lookup"><span data-stu-id="b59ea-189">The value in **id** in the response is based on the format, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}.</span></span> <span data-ttu-id="b59ea-190">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b59ea-190">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b59ea-191">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b59ea-191">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "extk9eruy7c_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

### <a name="example-3-creating-a-schema-extension-setting-the-owner"></a><span data-ttu-id="b59ea-192">Пример 3: Создание параметра расширения схемы владелец</span><span class="sxs-lookup"><span data-stu-id="b59ea-192">Example 3: Creating a schema extension setting the owner</span></span>

#### <a name="request"></a><span data-ttu-id="b59ea-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="b59ea-193">Request</span></span>

<span data-ttu-id="b59ea-194">В этом примере показано, как создать параметр расширения схемы для **владельца**.</span><span class="sxs-lookup"><span data-stu-id="b59ea-194">This example shows how to create a schema extension setting the **owner**.</span></span>  <span data-ttu-id="b59ea-195">В этом сценарии пользователь приложения может не быть владельцем приложения (например, если используется обозреватель Microsoft Graph).</span><span class="sxs-lookup"><span data-stu-id="b59ea-195">In this scenario, the user of the application might not be the owner of the application (for example if you are using Microsoft Graph Explorer).</span></span>  <span data-ttu-id="b59ea-196">В этом случае необходимо задать для свойства **owner** **идентификатор AppID** приложения, в противном случае вы не будете иметь права на создание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="b59ea-196">In this case you should set the **owner** property to the **appId** of an application you own, otherwise you won't be authorized to create a schema extension.</span></span> <span data-ttu-id="b59ea-197">Задайте свойство **owner** в запросе вместе с представлением в формате JSON остальных свойств объекта [schemaExtension](../resources/schemaextension.md) .</span><span class="sxs-lookup"><span data-stu-id="b59ea-197">Set the **owner** property in the request, together with the JSON representation of the rest of the properties in the [schemaExtension](../resources/schemaextension.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="b59ea-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="b59ea-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_3"
}-->

```http
POST https://graph.microsoft.com/beta/schemaExtensions
Content-type: application/json

{
    "id":"courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "owner": "50897f70-a455-4adf-87bc-4cf17091d5ac",
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="b59ea-199">C#</span><span class="sxs-lookup"><span data-stu-id="b59ea-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b59ea-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b59ea-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b59ea-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b59ea-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b59ea-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="b59ea-202">Response</span></span>

<span data-ttu-id="b59ea-203">Ответ включает в себя **владельца** , которому присвоено указанное значение в запросе.</span><span class="sxs-lookup"><span data-stu-id="b59ea-203">The response includes the **owner** set to the supplied value in the request.</span></span> <span data-ttu-id="b59ea-204">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="b59ea-204">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b59ea-205">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b59ea-205">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "extk9eruy7c_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "50897f70-a455-4adf-87bc-4cf17091d5ac",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="b59ea-206">См. также</span><span class="sxs-lookup"><span data-stu-id="b59ea-206">See also</span></span>

- [<span data-ttu-id="b59ea-207">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="b59ea-207">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b59ea-208">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="b59ea-208">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
