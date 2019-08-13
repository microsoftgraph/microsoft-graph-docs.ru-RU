---
title: Создание schemaExtension
description: Создайте новое определение schemaExtension, чтобы расширить поддерживаемый тип ресурса.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 84a5e689de794e6c9c030715544f186a9fe41868
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364413"
---
# <a name="create-schemaextension"></a><span data-ttu-id="edcfb-103">Создание schemaExtension</span><span class="sxs-lookup"><span data-stu-id="edcfb-103">Create schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edcfb-104">Создайте новое определение [schemaExtension](../resources/schemaextension.md), чтобы расширить [поддерживаемый тип ресурса](/graph/extensibility-overview#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="edcfb-104">Create a new [schemaExtension](../resources/schemaextension.md) definition to extend a [supporting resource type](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="edcfb-p101">Расширения схемы позволяют добавлять в ресурс строго типизированные пользовательские данные. Приложение, которое создает расширение схемы, является приложением-владельцем. В зависимости от [состояния](/graph/extensibility-overview#schema-extensions-lifecycle) расширения, приложение-владелец может обновить или удалить расширение. Другие приложения такого не могут.</span><span class="sxs-lookup"><span data-stu-id="edcfb-p101">Schema extensions let you add strongly-typed custom data to a resource. The app that creates a schema extension is the owner app. Depending on the [state](/graph/extensibility-overview#schema-extensions-lifecycle) of the extension, the owner app, and only the owner app, may update or delete the extension.</span></span> 

<span data-ttu-id="edcfb-108">Ознакомьтесь с примерами того, как [определить расширение схемы, описывающее учебный курс](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course), использовать определение расширения схемы для [создания группы с данными учебного курса](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data) и [добавить данные учебного курса в существующую группу](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group).</span><span class="sxs-lookup"><span data-stu-id="edcfb-108">See examples of how to [define a schema extension that describes a training course](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course), use the schema extension definition to [create a new group with training course data](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data), and [add training course data to an existing group](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group).</span></span>

## <a name="permissions"></a><span data-ttu-id="edcfb-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="edcfb-109">Permissions</span></span>
<span data-ttu-id="edcfb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edcfb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="edcfb-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edcfb-112">Permission type</span></span>      | <span data-ttu-id="edcfb-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="edcfb-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edcfb-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edcfb-114">Delegated (work or school account)</span></span> | <span data-ttu-id="edcfb-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="edcfb-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="edcfb-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edcfb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edcfb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edcfb-117">Not supported.</span></span>    |
|<span data-ttu-id="edcfb-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edcfb-118">Application</span></span> | <span data-ttu-id="edcfb-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edcfb-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="edcfb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edcfb-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /schemaExtensions
```

## <a name="request-headers"></a><span data-ttu-id="edcfb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="edcfb-121">Request headers</span></span>
| <span data-ttu-id="edcfb-122">Имя</span><span class="sxs-lookup"><span data-stu-id="edcfb-122">Name</span></span>       | <span data-ttu-id="edcfb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="edcfb-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="edcfb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="edcfb-124">Authorization</span></span>  | <span data-ttu-id="edcfb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="edcfb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="edcfb-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="edcfb-127">Content-Type</span></span>  | <span data-ttu-id="edcfb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="edcfb-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="edcfb-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="edcfb-129">Request body</span></span>
<span data-ttu-id="edcfb-130">В теле запроса должно быть представление объекта [schemaExtension](../resources/schemaextension.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edcfb-130">In the request body, supply a JSON representation of [schemaExtension](../resources/schemaextension.md) object.</span></span>

<span data-ttu-id="edcfb-131">В следующей таблице приведены свойства, доступные при создании расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="edcfb-131">The following table shows the properties that are available when you create a schema extension.</span></span>

| <span data-ttu-id="edcfb-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="edcfb-132">Parameter</span></span> | <span data-ttu-id="edcfb-133">Тип</span><span class="sxs-lookup"><span data-stu-id="edcfb-133">Type</span></span> | <span data-ttu-id="edcfb-134">Описание</span><span class="sxs-lookup"><span data-stu-id="edcfb-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edcfb-135">description</span><span class="sxs-lookup"><span data-stu-id="edcfb-135">description</span></span>|<span data-ttu-id="edcfb-136">String</span><span class="sxs-lookup"><span data-stu-id="edcfb-136">String</span></span>|<span data-ttu-id="edcfb-137">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="edcfb-137">Description for the schema extension.</span></span>|
|<span data-ttu-id="edcfb-138">id</span><span class="sxs-lookup"><span data-stu-id="edcfb-138">id</span></span>|<span data-ttu-id="edcfb-139">String</span><span class="sxs-lookup"><span data-stu-id="edcfb-139">String</span></span>|<span data-ttu-id="edcfb-140">Уникальный идентификатор для определения расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="edcfb-140">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="edcfb-141">Значение можно присвоить одним из двух способов:</span><span class="sxs-lookup"><span data-stu-id="edcfb-141">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="edcfb-142">Сцепите имя одного из ваших проверенных доменов с именем расширения схемы и создайте уникальную строку такого формата: \{_&#65279;доменноеИмя_\}\_\{_&#65279;имяСхемы_\}.</span><span class="sxs-lookup"><span data-stu-id="edcfb-142">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span> <span data-ttu-id="edcfb-143">Пример: `contoso_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="edcfb-143">As an example, `contoso_mySchema`.</span></span> <span data-ttu-id="edcfb-144">ПРИМЕЧАНИЕ. Поддерживаются только проверенные домены в следующих доменах верхнего уровня: `.com`,`.net`, `.gov`, `.edu` или `.org`.</span><span class="sxs-lookup"><span data-stu-id="edcfb-144">NOTE: Only verified domains under the following top-level domains are supported: `.com`,`.net`, `.gov`, `.edu` or `.org`.</span></span> </li><li><span data-ttu-id="edcfb-p105">Укажите имя схемы и предоставьте Microsoft Graph возможность использовать его для назначения **id** в таком формате: ext\{_&#65279;8-случайных-букв-или-цифр_\}\_\{_&#65279;имя-схемы_\}. Например, `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="edcfb-p105">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="edcfb-147">После создания это свойство невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="edcfb-147">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="edcfb-148">owner</span><span class="sxs-lookup"><span data-stu-id="edcfb-148">owner</span></span>|<span data-ttu-id="edcfb-149">String</span><span class="sxs-lookup"><span data-stu-id="edcfb-149">String</span></span>|<span data-ttu-id="edcfb-150">(Необязательный параметр) Идентификатор `appId` приложения, которое является владельцем расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="edcfb-150">(Optional) The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="edcfb-151">Это свойство можно указать при создании, чтобы задать владельца.</span><span class="sxs-lookup"><span data-stu-id="edcfb-151">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="edcfb-152">Если оно не указано, то в качестве владельца будет задано вызывающее приложение `appId`.</span><span class="sxs-lookup"><span data-stu-id="edcfb-152">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="edcfb-153">Таким образом, например, при создании определения расширения схемы с помощью песочницы Graph вам **потребуется** указать свойство владельца.</span><span class="sxs-lookup"><span data-stu-id="edcfb-153">So, for example, if creating a new schema extension definition using Graph Explorer, you **must** supply the owner property.</span></span> <span data-ttu-id="edcfb-154">После задания свойства оно будет доступно только для чтения, и вам не удастся изменить его.</span><span class="sxs-lookup"><span data-stu-id="edcfb-154">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="edcfb-155">properties</span><span class="sxs-lookup"><span data-stu-id="edcfb-155">properties</span></span>|<span data-ttu-id="edcfb-156">Коллекция [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="edcfb-156">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="edcfb-157">Коллекция типов и имен свойств, составляющих определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="edcfb-157">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="edcfb-158">targetTypes</span><span class="sxs-lookup"><span data-stu-id="edcfb-158">targetTypes</span></span>|<span data-ttu-id="edcfb-159">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="edcfb-159">String collection</span></span>|<span data-ttu-id="edcfb-160">Набор типов ресурсов Microsoft Graph, поддерживающих расширения схемы, к которым может быть применимо данное определение расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="edcfb-160">Set of Microsoft Graph resource types (that support schema extensions) that this schema extension definition can be applied to.</span></span>|

## <a name="response"></a><span data-ttu-id="edcfb-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="edcfb-161">Response</span></span>

<span data-ttu-id="edcfb-162">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [schemaExtension](../resources/schemaextension.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="edcfb-162">If successful, this method returns `201 Created` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edcfb-163">Пример</span><span class="sxs-lookup"><span data-stu-id="edcfb-163">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="edcfb-164">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="edcfb-164">Request 1</span></span>

<span data-ttu-id="edcfb-p107">В первом примере мы создаем уникальную строку со свойством **id** для определения расширения схемы, используя проверенное доменное имя (`graphlearn`) и имя схемы (`courses`). Уникальная строка имеет такой формат: \{_&#65279;доменноеИмя_\}\_\{_&#65279;имяСхемы_\}.</span><span class="sxs-lookup"><span data-stu-id="edcfb-p107">The first example shows using a verified domain name, `graphlearn`, and a schema name, `courses`, to form a unique string for the **id** property of the schema extension definition. The unique string is based on this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span>

<span data-ttu-id="edcfb-167">В теле запроса должно быть представление объекта [schemaExtension](../resources/schemaextension.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edcfb-167">In the request body, supply a JSON representation of the [schemaExtension](../resources/schemaextension.md) object.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="edcfb-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="edcfb-168">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="edcfb-169">C#</span><span class="sxs-lookup"><span data-stu-id="edcfb-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="edcfb-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edcfb-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="edcfb-171">Цель — C</span><span class="sxs-lookup"><span data-stu-id="edcfb-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="edcfb-172">Java</span><span class="sxs-lookup"><span data-stu-id="edcfb-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schemaextension-from-schemaextensions-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="edcfb-173">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="edcfb-173">Response 1</span></span>

<span data-ttu-id="edcfb-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="edcfb-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="edcfb-177">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="edcfb-177">Request 2</span></span>

<span data-ttu-id="edcfb-p109">Во втором примере мы указываем имя схемы (`courses`) в свойстве **id** тела запроса, а также остальные свойства в объекте [schemaExtension](../resources/schemaextension.md) как данные JSON. Microsoft Graph назначит и вернет в отклике уникальное строковое значение.</span><span class="sxs-lookup"><span data-stu-id="edcfb-p109">The second example shows specifying just a schema name, `courses`, in the **id** property in the request, together with the JSON representation of the rest of the properties in the [schemaExtension](../resources/schemaextension.md) object. Microsoft Graph will assign and return a unique string value in the response.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="edcfb-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="edcfb-180">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="edcfb-181">C#</span><span class="sxs-lookup"><span data-stu-id="edcfb-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="edcfb-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edcfb-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="edcfb-183">Цель — C</span><span class="sxs-lookup"><span data-stu-id="edcfb-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="edcfb-184">Java</span><span class="sxs-lookup"><span data-stu-id="edcfb-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schemaextension-from-schemaextensions-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="edcfb-185">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="edcfb-185">Response 2</span></span>

<span data-ttu-id="edcfb-p110">Отклик включает уникальную строку в свойстве **id**, созданную на основе имени схемы, предоставленном в запросе, и прочее содержимое созданного определения схемы. Значение **id** в отклике имеет формат ext\{_&#65279;8-случайных-букв-или-цифр_\}\_\{_&#65279;имя-схемы_\}. Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="edcfb-p110">The response includes a unique string in the **id** property that is based on the schema name provided in the request, together with the rest of the newly created schema definition. The value in **id** in the response is based on the format, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="edcfb-190">См. также</span><span class="sxs-lookup"><span data-stu-id="edcfb-190">See also</span></span>

- [<span data-ttu-id="edcfb-191">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="edcfb-191">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="edcfb-192">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="edcfb-192">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
