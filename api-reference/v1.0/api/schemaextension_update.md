# <a name="update-schemaextension"></a><span data-ttu-id="19527-101">Обновление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="19527-101">Update schemaExtension</span></span>

<span data-ttu-id="19527-102">Обновление свойств в определении указанного ресурса [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="19527-102">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="19527-p101">Это обновление применяется ко всем ресурсам, включенным в свойство **targetTypes** расширения. Эти ресурсы входят в число [поддерживаемых](../../../concepts/extensibility_overview.md#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="19527-p101">The update applies to all the resources that are included in the **targetTypes** property of the extension. These resources are among the [supporting resource types](../../../concepts/extensibility_overview.md#supported-resources).</span></span>

<span data-ttu-id="19527-p102">Только приложение, которое создало расширение схемы (приложение-владелец), может внести дополнения в расширение, причем только тогда, когда расширение находится в состоянии **InDevelopment** или **Available**. Это означает, что приложению не удастся удалить настраиваемые свойства или целевые типы ресурсов из определения. Но приложение может изменить описание расширения.</span><span class="sxs-lookup"><span data-stu-id="19527-p102">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status. That means the app cannot remove custom properties or target resource types from the definition. The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="19527-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19527-108">Permissions</span></span>
<span data-ttu-id="19527-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="19527-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="19527-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19527-111">Permission type</span></span>      | <span data-ttu-id="19527-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19527-112">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="19527-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19527-113">Delegated (work or school account)</span></span> | <span data-ttu-id="19527-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19527-114">Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="19527-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19527-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19527-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19527-116">Not supported.</span></span>    | 
|<span data-ttu-id="19527-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19527-117">Application</span></span> | <span data-ttu-id="19527-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19527-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="19527-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19527-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="19527-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19527-120">Optional request headers</span></span>

| <span data-ttu-id="19527-121">Имя</span><span class="sxs-lookup"><span data-stu-id="19527-121">Name</span></span>      |<span data-ttu-id="19527-122">Описание</span><span class="sxs-lookup"><span data-stu-id="19527-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="19527-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19527-123">Authorization</span></span>  | <span data-ttu-id="19527-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19527-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19527-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19527-126">Content-Type</span></span>   | <span data-ttu-id="19527-127">application/json</span><span class="sxs-lookup"><span data-stu-id="19527-127">application/json</span></span> | 

## <a name="request-body"></a><span data-ttu-id="19527-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="19527-128">Request body</span></span>

<span data-ttu-id="19527-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="19527-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="19527-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="19527-132">Property</span></span>   | <span data-ttu-id="19527-133">Тип</span><span class="sxs-lookup"><span data-stu-id="19527-133">Type</span></span> |<span data-ttu-id="19527-134">Описание</span><span class="sxs-lookup"><span data-stu-id="19527-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19527-135">description</span><span class="sxs-lookup"><span data-stu-id="19527-135">description</span></span>|<span data-ttu-id="19527-136">String</span><span class="sxs-lookup"><span data-stu-id="19527-136">String</span></span>|<span data-ttu-id="19527-137">Описание расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="19527-137">Description for the schema extension.</span></span>|
|<span data-ttu-id="19527-138">properties</span><span class="sxs-lookup"><span data-stu-id="19527-138">properties</span></span>|<span data-ttu-id="19527-139">Коллекция [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="19527-139">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="19527-p106">Коллекция имен и типов свойств, составляющих определение расширения схемы. Разрешено вносить изменения только в виде дополнений.</span><span class="sxs-lookup"><span data-stu-id="19527-p106">The collection of property names and types that make up the schema extension definition. Only additive changes are permitted.</span></span> |
|<span data-ttu-id="19527-142">status</span><span class="sxs-lookup"><span data-stu-id="19527-142">status</span></span>|<span data-ttu-id="19527-143">String</span><span class="sxs-lookup"><span data-stu-id="19527-143">String</span></span>|<span data-ttu-id="19527-p107">Состояние жизненного цикла расширения схемы. Начальное состояние при создании расширения схемы: **InDevelopment**. Возможные варианты перехода: из состояния **InDevelopment** в состояние **Available**, из состояния **Available** в состояние **Deprecated** и из состояния **Deprecated** в состояние **Available**.</span><span class="sxs-lookup"><span data-stu-id="19527-p107">The lifecycle state of the schema extension. The initial state upon creation is **InDevelopment**. Possible states transitions are from **InDevelopment** to **Available**, **Available** to **Deprecated** and **Deprecated** to **Available**.</span></span>|
|<span data-ttu-id="19527-147">targetTypes</span><span class="sxs-lookup"><span data-stu-id="19527-147">targetTypes</span></span>|<span data-ttu-id="19527-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="19527-148">String collection</span></span>|<span data-ttu-id="19527-p108">Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.  Разрешено вносить изменения только в виде дополнений.</span><span class="sxs-lookup"><span data-stu-id="19527-p108">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="19527-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="19527-151">Response</span></span>

<span data-ttu-id="19527-152">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="19527-152">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="19527-153">Пример</span><span class="sxs-lookup"><span data-stu-id="19527-153">Example</span></span>

##### <a name="request"></a><span data-ttu-id="19527-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="19527-154">Request</span></span>

<span data-ttu-id="19527-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19527-155">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="19527-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="19527-156">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="19527-157">См. также</span><span class="sxs-lookup"><span data-stu-id="19527-157">See also</span></span>

- [<span data-ttu-id="19527-158">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="19527-158">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="19527-159">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="19527-159">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->