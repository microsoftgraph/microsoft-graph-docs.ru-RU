# <a name="imageinfo-resource-type"></a><span data-ttu-id="de8c3-101">тип ресурса imageInfo</span><span class="sxs-lookup"><span data-stu-id="de8c3-101">imageInfo resource type</span></span>

<span data-ttu-id="de8c3-102">Сложный тип для представления свойства **атрибуция** в части [visualInfo](../resources/projectrome_visualinfo.md) объекта [активности](../resources/projectrome_activity.md).</span><span class="sxs-lookup"><span data-stu-id="de8c3-102">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome_visualinfo.md) part of the [activity](../resources/projectrome_activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="de8c3-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="de8c3-103">Properties</span></span>

|<span data-ttu-id="de8c3-104">Имя</span><span class="sxs-lookup"><span data-stu-id="de8c3-104">Name</span></span> | <span data-ttu-id="de8c3-105">Тип</span><span class="sxs-lookup"><span data-stu-id="de8c3-105">Type</span></span> | <span data-ttu-id="de8c3-106">Описание</span><span class="sxs-lookup"><span data-stu-id="de8c3-106">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="de8c3-107">IconUrl</span><span class="sxs-lookup"><span data-stu-id="de8c3-107">iconurl</span></span> | <span data-ttu-id="de8c3-108">Строка</span><span class="sxs-lookup"><span data-stu-id="de8c3-108">String</span></span> | <span data-ttu-id="de8c3-109">Необязательный параметр; URI-адрес, указывающий на значок, который представляет приложение, используемое для создания действия</span><span class="sxs-lookup"><span data-stu-id="de8c3-109">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="de8c3-110">alternateText</span><span class="sxs-lookup"><span data-stu-id="de8c3-110">alternateText</span></span> | <span data-ttu-id="de8c3-111">Строка</span><span class="sxs-lookup"><span data-stu-id="de8c3-111">String</span></span> | <span data-ttu-id="de8c3-112">Необязательный параметр; замещающий текст доступного содержимого для изображения</span><span class="sxs-lookup"><span data-stu-id="de8c3-112">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="de8c3-113">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="de8c3-113">addImageQuery</span></span> | <span data-ttu-id="de8c3-114">Логический</span><span class="sxs-lookup"><span data-stu-id="de8c3-114">Boolean</span></span> | <span data-ttu-id="de8c3-115">Необязательный параметр; предназначенный для указания сервера, может динамически преобразовать изображение для просмотра в ответ на параметризацию.</span><span class="sxs-lookup"><span data-stu-id="de8c3-115">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="de8c3-116">Например, изображение высокой контрастности</span><span class="sxs-lookup"><span data-stu-id="de8c3-116">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de8c3-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de8c3-117">JSON Representation</span></span>

<span data-ttu-id="de8c3-118">Ниже представлено описание ресурса в формате JSON</span><span class="sxs-lookup"><span data-stu-id="de8c3-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->