# <a name="update-worksheet"></a><span data-ttu-id="44766-101">Обновление листа</span><span class="sxs-lookup"><span data-stu-id="44766-101">Update worksheet</span></span>

<span data-ttu-id="44766-102">Обновление свойств объекта листа.</span><span class="sxs-lookup"><span data-stu-id="44766-102">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="44766-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44766-103">Permissions</span></span>
<span data-ttu-id="44766-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="44766-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="44766-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44766-106">Permission type</span></span>      | <span data-ttu-id="44766-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44766-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44766-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44766-108">Delegated (work or school account)</span></span> | <span data-ttu-id="44766-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44766-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="44766-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44766-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44766-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44766-111">Not supported.</span></span>    |
|<span data-ttu-id="44766-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44766-112">Application</span></span> | <span data-ttu-id="44766-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44766-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44766-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44766-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="44766-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44766-115">Optional request headers</span></span>
| <span data-ttu-id="44766-116">Имя</span><span class="sxs-lookup"><span data-stu-id="44766-116">Name</span></span>       | <span data-ttu-id="44766-117">Описание</span><span class="sxs-lookup"><span data-stu-id="44766-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="44766-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44766-118">Authorization</span></span>  | <span data-ttu-id="44766-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44766-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44766-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44766-121">Request body</span></span>
<span data-ttu-id="44766-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="44766-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="44766-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="44766-125">Property</span></span>     | <span data-ttu-id="44766-126">Тип</span><span class="sxs-lookup"><span data-stu-id="44766-126">Type</span></span>   |<span data-ttu-id="44766-127">Описание</span><span class="sxs-lookup"><span data-stu-id="44766-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44766-128">name</span><span class="sxs-lookup"><span data-stu-id="44766-128">name</span></span>|<span data-ttu-id="44766-129">string</span><span class="sxs-lookup"><span data-stu-id="44766-129">string</span></span>|<span data-ttu-id="44766-130">Отображаемое имя листа.</span><span class="sxs-lookup"><span data-stu-id="44766-130">The display name of the worksheet.</span></span>|
|<span data-ttu-id="44766-131">position</span><span class="sxs-lookup"><span data-stu-id="44766-131">position</span></span>|<span data-ttu-id="44766-132">int</span><span class="sxs-lookup"><span data-stu-id="44766-132">int</span></span>|<span data-ttu-id="44766-133">Положение листа (начиная с нуля) в книге.</span><span class="sxs-lookup"><span data-stu-id="44766-133">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="44766-134">visibility</span><span class="sxs-lookup"><span data-stu-id="44766-134">visibility</span></span>|<span data-ttu-id="44766-135">string</span><span class="sxs-lookup"><span data-stu-id="44766-135">string</span></span>|<span data-ttu-id="44766-p104">Видимость листа. Возможные значения: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="44766-p104">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="44766-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="44766-138">Response</span></span>

<span data-ttu-id="44766-139">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [Worksheet](../resources/worksheet.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44766-139">If successful, this method returns a `200 OK` response code and updated [Worksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="44766-140">Пример</span><span class="sxs-lookup"><span data-stu-id="44766-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44766-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="44766-141">Request</span></span>
<span data-ttu-id="44766-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44766-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
##### <a name="response"></a><span data-ttu-id="44766-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="44766-143">Response</span></span>
<span data-ttu-id="44766-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="44766-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->