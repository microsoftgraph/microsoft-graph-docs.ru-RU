---
title: Создание schemaExtension
description: Создайте новое определение schemaExtension, чтобы расширить поддерживаемый тип ресурса.
localization_priority: Priority
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: a498b23cc29c806f24cd620110ce731598ba2582
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054478"
---
# <a name="create-schemaextension"></a><span data-ttu-id="a5c03-103">Создание schemaExtension</span><span class="sxs-lookup"><span data-stu-id="a5c03-103">Create schemaExtension</span></span>

<span data-ttu-id="a5c03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5c03-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a5c03-105">Создайте новое определение [schemaExtension](../resources/schemaextension.md), чтобы расширить [поддерживаемый тип ресурса](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="a5c03-105">Create a new [schemaExtension](../resources/schemaextension.md) definition to extend a [supporting resource type](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="a5c03-p101">Расширения схемы позволяют добавлять в ресурс строго типизированные пользовательские данные. Приложение, которое создает расширение схемы, является приложением-владельцем. В зависимости от [состояния](/graph/extensibility-overview#schema-extensions-lifecycle) расширения, приложение-владелец может обновить или удалить расширение. Другие приложения такого не могут.</span><span class="sxs-lookup"><span data-stu-id="a5c03-p101">Schema extensions let you add strongly-typed custom data to a resource. The app that creates a schema extension is the owner app. Depending on the [state](/graph/extensibility-overview#schema-extensions-lifecycle) of the extension, the owner app, and only the owner app, may update or delete the extension.</span></span> 

<span data-ttu-id="a5c03-109">Ознакомьтесь с примерами того, как [определить расширение схемы, описывающее учебный курс](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course), использовать определение расширения схемы для [создания группы с данными учебного курса](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data) и [добавить данные учебного курса в существующую группу](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group).</span><span class="sxs-lookup"><span data-stu-id="a5c03-109">See examples of how to [define a schema extension that describes a training course](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course), use the schema extension definition to [create a new group with training course data](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data), and [add training course data to an existing group](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group).</span></span>

## <a name="permissions"></a><span data-ttu-id="a5c03-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5c03-110">Permissions</span></span>
<span data-ttu-id="a5c03-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5c03-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a5c03-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5c03-113">Permission type</span></span>      | <span data-ttu-id="a5c03-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5c03-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5c03-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5c03-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a5c03-116">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a5c03-116">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a5c03-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5c03-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5c03-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5c03-118">Not supported.</span></span>    |
|<span data-ttu-id="a5c03-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5c03-119">Application</span></span> | <span data-ttu-id="a5c03-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5c03-120">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="a5c03-121">Кроме того, при делегированном потоке вошедший в систему пользователь должен быть владелец вызывающего приложения ИЛИ владельцем (приложения с) `appId`, использованного для задания свойства **Владелец**.</span><span class="sxs-lookup"><span data-stu-id="a5c03-121">Additionally for the delegated flow, the signed-in user must be the owner of the calling application OR the owner of the (application with the) `appId` used to set the **owner** property.</span></span>

## <a name="http-request"></a><span data-ttu-id="a5c03-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5c03-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /schemaExtensions
```

## <a name="request-headers"></a><span data-ttu-id="a5c03-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5c03-123">Request headers</span></span>
| <span data-ttu-id="a5c03-124">Имя</span><span class="sxs-lookup"><span data-stu-id="a5c03-124">Name</span></span>       | <span data-ttu-id="a5c03-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a5c03-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a5c03-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5c03-126">Authorization</span></span>  | <span data-ttu-id="a5c03-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5c03-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a5c03-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5c03-129">Content-Type</span></span>  | <span data-ttu-id="a5c03-130">application/json</span><span class="sxs-lookup"><span data-stu-id="a5c03-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5c03-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a5c03-131">Request body</span></span>
<span data-ttu-id="a5c03-132">В теле запроса должно быть представление объекта [schemaExtension](../resources/schemaextension.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5c03-132">In the request body, supply a JSON representation of [schemaExtension](../resources/schemaextension.md) object.</span></span>

<span data-ttu-id="a5c03-133">В приведенной ниже таблице показаны свойства, которые обязательно указывать при создании расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="a5c03-133">The following table shows the properties that are required when you create a schema extension.</span></span>

| <span data-ttu-id="a5c03-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="a5c03-134">Parameter</span></span> | <span data-ttu-id="a5c03-135">Тип</span><span class="sxs-lookup"><span data-stu-id="a5c03-135">Type</span></span> | <span data-ttu-id="a5c03-136">Описание</span><span class="sxs-lookup"><span data-stu-id="a5c03-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5c03-137">description</span><span class="sxs-lookup"><span data-stu-id="a5c03-137">description</span></span>|<span data-ttu-id="a5c03-138">String</span><span class="sxs-lookup"><span data-stu-id="a5c03-138">String</span></span>|<span data-ttu-id="a5c03-139">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="a5c03-139">Description for the schema extension.</span></span>|
|<span data-ttu-id="a5c03-140">id</span><span class="sxs-lookup"><span data-stu-id="a5c03-140">id</span></span>|<span data-ttu-id="a5c03-141">String</span><span class="sxs-lookup"><span data-stu-id="a5c03-141">String</span></span>|<span data-ttu-id="a5c03-142">Уникальный идентификатор для определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="a5c03-142">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="a5c03-143">Значение можно присвоить одним из двух способов:</span><span class="sxs-lookup"><span data-stu-id="a5c03-143">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="a5c03-144">Сцепите имя одного из ваших проверенных доменов с именем расширения схемы и создайте уникальную строку такого формата: \{_&#65279;доменноеИмя_\}\_\{_&#65279;имяСхемы_\}.</span><span class="sxs-lookup"><span data-stu-id="a5c03-144">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span> <span data-ttu-id="a5c03-145">Пример: `contoso_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="a5c03-145">As an example, `contoso_mySchema`.</span></span> <span data-ttu-id="a5c03-146">ПРИМЕЧАНИЕ. Поддерживаются только проверенные домены в следующих доменах верхнего уровня: `.com`,`.net`, `.gov`, `.edu` или `.org`.</span><span class="sxs-lookup"><span data-stu-id="a5c03-146">NOTE: Only verified domains under the following top-level domains are supported: `.com`,`.net`, `.gov`, `.edu` or `.org`.</span></span> </li><li><span data-ttu-id="a5c03-p105">Укажите имя схемы и предоставьте Microsoft Graph возможность использовать его для назначения **id** в таком формате: ext\{_&#65279;8-случайных-букв-или-цифр_\}\_\{_&#65279;имя-схемы_\}. Например, `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="a5c03-p105">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="a5c03-149">После создания это свойство невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="a5c03-149">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="a5c03-150">owner</span><span class="sxs-lookup"><span data-stu-id="a5c03-150">owner</span></span>|<span data-ttu-id="a5c03-151">String</span><span class="sxs-lookup"><span data-stu-id="a5c03-151">String</span></span>|<span data-ttu-id="a5c03-152">(Необязательный параметр) Идентификатор `appId` приложения, которое является владельцем расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="a5c03-152">(Optional) The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="a5c03-153">По умолчанию владельцем становится `appId` вызывающего приложения.</span><span class="sxs-lookup"><span data-stu-id="a5c03-153">By default, the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="a5c03-154">Однако это свойство можно указать при создании, чтобы задать в качестве владельца appId другого приложения (не вызывающего).</span><span class="sxs-lookup"><span data-stu-id="a5c03-154">However, the property may be supplied on creation, to set the owner appId to something different from the calling app.</span></span> <span data-ttu-id="a5c03-155">Во всех случаях в делегированном потоке вошедший в систему пользователь **должен** быть владельцем приложения, которое задается в качестве владельца расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="a5c03-155">In all cases, in the delegated flow, the signed-in user **must** be the owner of the application being set as the schema extension's owner.</span></span> <span data-ttu-id="a5c03-156">Таким образом, например, при создании определения расширения схемы с помощью песочницы Graph вам **потребуется** указать свойство владельца.</span><span class="sxs-lookup"><span data-stu-id="a5c03-156">So, for example, if creating a new schema extension definition using Graph Explorer, you **must** supply the owner property, for an appId you own.</span></span> <span data-ttu-id="a5c03-157">После задания свойства оно будет доступно только для чтения, и вам не удастся изменить его.</span><span class="sxs-lookup"><span data-stu-id="a5c03-157">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="a5c03-158">properties</span><span class="sxs-lookup"><span data-stu-id="a5c03-158">properties</span></span>|<span data-ttu-id="a5c03-159">Коллекция [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="a5c03-159">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="a5c03-160">Коллекция типов и имен свойств, составляющих определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="a5c03-160">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="a5c03-161">targetTypes</span><span class="sxs-lookup"><span data-stu-id="a5c03-161">targetTypes</span></span>|<span data-ttu-id="a5c03-162">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a5c03-162">String collection</span></span>|<span data-ttu-id="a5c03-163">Набор типов ресурсов Microsoft Graph, поддерживающих расширения схемы, к которым может быть применимо данное определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="a5c03-163">Set of Microsoft Graph resource types (that support schema extensions) that this schema extension definition can be applied to.</span></span>|

## <a name="response"></a><span data-ttu-id="a5c03-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5c03-164">Response</span></span>

<span data-ttu-id="a5c03-165">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [schemaExtension](../resources/schemaextension.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a5c03-165">If successful, this method returns `201 Created` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5c03-166">Пример</span><span class="sxs-lookup"><span data-stu-id="a5c03-166">Example</span></span>

### <a name="example-1-creating-a-schema-extension-using-a-verified-domain"></a><span data-ttu-id="a5c03-167">Пример 1. Создание расширения схемы с помощью проверенного домена</span><span class="sxs-lookup"><span data-stu-id="a5c03-167">Example 1: Creating a schema extension using a verified domain</span></span>

#### <a name="request"></a><span data-ttu-id="a5c03-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5c03-168">Request</span></span>

<span data-ttu-id="a5c03-169">В этом примере мы создаем уникальную строку со свойством **id** для определения расширения схемы, используя проверенное доменное имя (`graphlearn`) и имя схемы (`courses`).</span><span class="sxs-lookup"><span data-stu-id="a5c03-169">This example shows using a verified domain name, `graphlearn`, and a schema name, `courses`, to form a unique string for the **id** property of the schema extension definition.</span></span> <span data-ttu-id="a5c03-170">Уникальная строка имеет такой формат: \{_&#65279;доменноеИмя_\}\_\{_&#65279;имяСхемы_\}.</span><span class="sxs-lookup"><span data-stu-id="a5c03-170">The unique string is based on this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5c03-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5c03-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
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
# <a name="c"></a>[<span data-ttu-id="a5c03-172">C#</span><span class="sxs-lookup"><span data-stu-id="a5c03-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5c03-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5c03-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5c03-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5c03-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5c03-175">Java</span><span class="sxs-lookup"><span data-stu-id="a5c03-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schemaextension-from-schemaextensions-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a5c03-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5c03-176">Response</span></span>

<span data-ttu-id="a5c03-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a5c03-177">Here is an example of the response.</span></span> <span data-ttu-id="a5c03-178">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a5c03-178">Note: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-creating-a-schema-extension-using-just-a-name"></a><span data-ttu-id="a5c03-179">Пример 2. Создание расширения схемы с помощью одного имени</span><span class="sxs-lookup"><span data-stu-id="a5c03-179">Example 2: Creating a schema extension using just a name</span></span>

#### <a name="request"></a><span data-ttu-id="a5c03-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5c03-180">Request</span></span>

<span data-ttu-id="a5c03-181">В данном примере мы указываем имя схемы (`courses`) в свойстве **id** тела запроса, а также остальные свойства в объекте [schemaExtension](../resources/schemaextension.md) как данные JSON.</span><span class="sxs-lookup"><span data-stu-id="a5c03-181">This example shows specifying just a schema name, `courses`, in the **id** property in the request, together with the JSON representation of the rest of the properties in the [schemaExtension](../resources/schemaextension.md) object.</span></span> <span data-ttu-id="a5c03-182">Microsoft Graph назначит и вернет в отклике уникальное строковое значение.</span><span class="sxs-lookup"><span data-stu-id="a5c03-182">Microsoft Graph will assign and return a unique string value in the response.</span></span>


# <a name="http"></a>[<span data-ttu-id="a5c03-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5c03-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
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
# <a name="c"></a>[<span data-ttu-id="a5c03-184">C#</span><span class="sxs-lookup"><span data-stu-id="a5c03-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5c03-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5c03-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5c03-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5c03-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5c03-187">Java</span><span class="sxs-lookup"><span data-stu-id="a5c03-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schemaextension-from-schemaextensions-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a5c03-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5c03-188">Response</span></span>

<span data-ttu-id="a5c03-189">Отклик включает уникальную строку в свойстве **id**, созданную на основе имени схемы, предоставленном в запросе, и прочее содержимое созданного определения схемы.</span><span class="sxs-lookup"><span data-stu-id="a5c03-189">The response includes a unique string in the **id** property that is based on the schema name provided in the request, together with the rest of the newly created schema definition.</span></span> <span data-ttu-id="a5c03-190">Значение **id** в отклике имеет формат ext\{_&#65279;8-случайных-букв-или-цифр_\}\_\{_&#65279;имя-схемы_\}.</span><span class="sxs-lookup"><span data-stu-id="a5c03-190">The value in **id** in the response is based on the format, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}.</span></span> <span data-ttu-id="a5c03-191">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a5c03-191">Note: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-3-creating-a-schema-extension-setting-the-owner"></a><span data-ttu-id="a5c03-192">Пример 3. Создание расширения схемы путем задания владельца</span><span class="sxs-lookup"><span data-stu-id="a5c03-192">Example 3: Creating a schema extension setting the owner</span></span>

#### <a name="request"></a><span data-ttu-id="a5c03-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5c03-193">Request</span></span>

<span data-ttu-id="a5c03-194">В этом примере показано, как создать расширение схемы, задав свойство **owner**.</span><span class="sxs-lookup"><span data-stu-id="a5c03-194">This example shows how to create a schema extension setting the **owner**.</span></span>  <span data-ttu-id="a5c03-195">В этом случае пользователь приложения может и быть владельцем приложения (например, при использовании песочницы Microsoft Graph).</span><span class="sxs-lookup"><span data-stu-id="a5c03-195">In this scenario, the user of the application might not be the owner of the application (for example if you are using Microsoft Graph Explorer).</span></span>  <span data-ttu-id="a5c03-196">В этом случае необходимо задать **appId** приложения, которым вы владеете, в качестве значения свойства **owner**, иначе у вас не будет прав на создание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="a5c03-196">In this case you should set the **owner** property to the **appId** of an application you own, otherwise you won't be authorized to create a schema extension.</span></span> <span data-ttu-id="a5c03-197">Задайте свойство **owner** в запросе, а также остальные свойства в объекте [schemaExtension](../resources/schemaextension.md) как данные JSON.</span><span class="sxs-lookup"><span data-stu-id="a5c03-197">Set the **owner** property in the request, together with the JSON representation of the rest of the properties in the [schemaExtension](../resources/schemaextension.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="a5c03-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5c03-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_3"
}-->

```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
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
# <a name="c"></a>[<span data-ttu-id="a5c03-199">C#</span><span class="sxs-lookup"><span data-stu-id="a5c03-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5c03-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5c03-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5c03-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5c03-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5c03-202">Java</span><span class="sxs-lookup"><span data-stu-id="a5c03-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schemaextension-from-schemaextensions-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a5c03-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5c03-203">Response</span></span>

<span data-ttu-id="a5c03-204">Отклик содержит **owner** со значением, указанным в запросе.</span><span class="sxs-lookup"><span data-stu-id="a5c03-204">The response includes the **owner** set to the supplied value in the request.</span></span> <span data-ttu-id="a5c03-205">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a5c03-205">Note: The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="a5c03-206">См. также</span><span class="sxs-lookup"><span data-stu-id="a5c03-206">See also</span></span>

- [<span data-ttu-id="a5c03-207">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="a5c03-207">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a5c03-208">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="a5c03-208">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

