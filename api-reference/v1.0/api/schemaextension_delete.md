# <a name="delete-schemaextension"></a><span data-ttu-id="c3d9a-101">Удаление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="c3d9a-101">Delete schemaExtension</span></span>

<span data-ttu-id="c3d9a-102">Удаление определения [расширения схемы](../resources/schemaExtension.md).</span><span class="sxs-lookup"><span data-stu-id="c3d9a-102">Delete the definition of a [schema extension](../resources/schemaExtension.md).</span></span>

<span data-ttu-id="c3d9a-p101">Только приложение, которое создало расширение схемы (приложение-владелец), может удалить определение расширения схемы, причем только тогда, когда расширение находится в состоянии **InDevelopment**. Удаление определения расширения схемы не влияет на доступ к пользовательским данным, добавленным в ресурс на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="c3d9a-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="c3d9a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3d9a-105">Permissions</span></span>
<span data-ttu-id="c3d9a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c3d9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="c3d9a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3d9a-108">Permission type</span></span>      | <span data-ttu-id="c3d9a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3d9a-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="c3d9a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3d9a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c3d9a-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c3d9a-111">Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="c3d9a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3d9a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3d9a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3d9a-113">Not supported.</span></span>    | 
|<span data-ttu-id="c3d9a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3d9a-114">Application</span></span> | <span data-ttu-id="c3d9a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3d9a-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c3d9a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3d9a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c3d9a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3d9a-117">Request headers</span></span>
| <span data-ttu-id="c3d9a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c3d9a-118">Name</span></span>      |<span data-ttu-id="c3d9a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c3d9a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c3d9a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3d9a-120">Authorization</span></span>  | <span data-ttu-id="c3d9a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3d9a-p103">Bearer {token}. Required.</span></span> |
 

## <a name="request-body"></a><span data-ttu-id="c3d9a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3d9a-123">Request body</span></span>
<span data-ttu-id="c3d9a-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3d9a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3d9a-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3d9a-125">Response</span></span>

<span data-ttu-id="c3d9a-p104">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c3d9a-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3d9a-128">Пример</span><span class="sxs-lookup"><span data-stu-id="c3d9a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3d9a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3d9a-129">Request</span></span>
<span data-ttu-id="c3d9a-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3d9a-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="c3d9a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3d9a-131">Response</span></span>
<span data-ttu-id="c3d9a-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c3d9a-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="c3d9a-133">См. также</span><span class="sxs-lookup"><span data-stu-id="c3d9a-133">See also</span></span>

- [<span data-ttu-id="c3d9a-134">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="c3d9a-134">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="c3d9a-135">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="c3d9a-135">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->