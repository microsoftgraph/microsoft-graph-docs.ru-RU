# <a name="visualinfo-resource-type"></a><span data-ttu-id="848b7-101">Тип ресурса visualInfo</span><span class="sxs-lookup"><span data-stu-id="848b7-101">visualInfo resource type</span></span>

<span data-ttu-id="848b7-102">Сложный тип для представления свойства **visualElements** в объекте [activity](../resources/projectrome_activity.md).</span><span class="sxs-lookup"><span data-stu-id="848b7-102">A complex type for representing the **attribution** property in the [visualInfo part of the activity](../resources/projectrome_activity.md) object.</span></span>

<span data-ttu-id="848b7-103">Каждое действие пользователя отображаются на временной шкале как адаптивная карточка.</span><span class="sxs-lookup"><span data-stu-id="848b7-103">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="848b7-104">Разработчикам приложений рекомендуется предоставить настраиваемую карточку, которая записывает сущность действий, которые выполнялись в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="848b7-104">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="848b7-105">Это можно сделать с указанием настраиваемой карточки JSON в свойстве содержимого.</span><span class="sxs-lookup"><span data-stu-id="848b7-105">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="848b7-106">В дополнение к визуальным метаданным с адаптивной карточкой, приложение может указывать содержимое метаданных — данные, которые используются для формирования вывода действия пользователя, чтобы предложить новые действия для будущего повторного взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="848b7-106">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="848b7-107">Это можно осуществить с помощью действия свойства contentInfo для предоставления объекта JSON, который использует свойства schema.org для описания содержимого.</span><span class="sxs-lookup"><span data-stu-id="848b7-107">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="848b7-108">Если этот параметр не указан, простая настраиваемая карточка будет создаваться с использованием отображаемого текста и описания свойств.</span><span class="sxs-lookup"><span data-stu-id="848b7-108">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="848b7-109">Рекомендуется использовать настраиваемые карточки для демонстрации наилучшего содержимого в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="848b7-109">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="848b7-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="848b7-110">Properties</span></span>

|<span data-ttu-id="848b7-111">Имя</span><span class="sxs-lookup"><span data-stu-id="848b7-111">Name</span></span> | <span data-ttu-id="848b7-112">Тип</span><span class="sxs-lookup"><span data-stu-id="848b7-112">Type</span></span> | <span data-ttu-id="848b7-113">Описание</span><span class="sxs-lookup"><span data-stu-id="848b7-113">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="848b7-114">displayText</span><span class="sxs-lookup"><span data-stu-id="848b7-114">displayText</span></span> | <span data-ttu-id="848b7-115">String</span><span class="sxs-lookup"><span data-stu-id="848b7-115">String</span></span> | <span data-ttu-id="848b7-116">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="848b7-116">Required.</span></span> <span data-ttu-id="848b7-117">Короткое текстовое описание уникального действия пользователя (например, имя документа в тех случаях, где действие относится к созданию документов)</span><span class="sxs-lookup"><span data-stu-id="848b7-117">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="848b7-118">description</span><span class="sxs-lookup"><span data-stu-id="848b7-118">description</span></span> | <span data-ttu-id="848b7-119">String</span><span class="sxs-lookup"><span data-stu-id="848b7-119">String</span></span> | <span data-ttu-id="848b7-120">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="848b7-120">Optional.</span></span> <span data-ttu-id="848b7-121">Более длинное текстовое описание уникальный активности пользователя (пример: имя документа, первое предложение и/или метаданные)</span><span class="sxs-lookup"><span data-stu-id="848b7-121">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="848b7-122">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="848b7-122">background-color</span></span> | <span data-ttu-id="848b7-123">String</span><span class="sxs-lookup"><span data-stu-id="848b7-123">String</span></span> | <span data-ttu-id="848b7-124">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="848b7-124">Optional.</span></span> <span data-ttu-id="848b7-125">Цвет фона, используемого для преобразования для просмотра активности в пользовательском интерфейсе - цвет торговой марки для источника действия приложения.</span><span class="sxs-lookup"><span data-stu-id="848b7-125">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="848b7-126">Должен быть допустим шестнадцатеричный цвет</span><span class="sxs-lookup"><span data-stu-id="848b7-126">Must be a valid hex color</span></span>|
|<span data-ttu-id="848b7-127">content</span><span class="sxs-lookup"><span data-stu-id="848b7-127">content</span></span> | <span data-ttu-id="848b7-128">Нетипизированный объект JSON</span><span class="sxs-lookup"><span data-stu-id="848b7-128">Untyped JSON object</span></span> | <span data-ttu-id="848b7-129">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="848b7-129">Optional.</span></span> <span data-ttu-id="848b7-130">Настраиваемые части данных — объект JSON, используемый для предоставления настраиваемого содержимого для преобразования для просмотра активности в пользовательском интерфейсе оболочки Windows</span><span class="sxs-lookup"><span data-stu-id="848b7-130">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="848b7-131">attribution</span><span class="sxs-lookup"><span data-stu-id="848b7-131">attribution</span></span> | <span data-ttu-id="848b7-132">[imageInfo](../resources/projectrome_imageinfo.md)</span><span class="sxs-lookup"><span data-stu-id="848b7-132">Added [imageInfo](../resources/projectrome_imageinfo.md)</span></span> | <span data-ttu-id="848b7-133">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="848b7-133">Optional.</span></span> <span data-ttu-id="848b7-134">Объект JSON, используемый для представления значка, представляющего приложение, используемое для создания действия</span><span class="sxs-lookup"><span data-stu-id="848b7-134">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="848b7-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="848b7-135">JSON Representation</span></span>

<span data-ttu-id="848b7-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="848b7-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@odata.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
