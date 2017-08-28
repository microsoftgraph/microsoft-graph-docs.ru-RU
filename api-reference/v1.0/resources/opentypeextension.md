# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="02dc3-101">Тип ресурсов openTypeExtension (открытые расширения)</span><span class="sxs-lookup"><span data-stu-id="02dc3-101">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="02dc3-p101">Открытые расширения (ранее звались расширениями данных Office 365) позволяют легко добавлять нетипизированные свойства непосредственно в ресурс в Microsoft Graph. Открытые расширения представлены ресурсом **openTypeExtension**. Все открытые расширения, добавленные в ресурс, отображаются в свойстве навигации **extensions**, которое является производным от абстрактного типа [extension](extension.md).  Каждое расширение, помимо пользовательских данных, содержит свойство **extensionName** — единственное предопределенное записываемое свойство. Чтобы обеспечить уникальность имен расширений, можно использовать формат обратных записей DNS, который зависит от _принадлежащего вам домена_, например `Com.Contoso.ContactInfo`. Не используйте домен Майкрософт (`Com.Microsoft` или `Com.OnMicrosoft`) в имени расширения.</span><span class="sxs-lookup"><span data-stu-id="02dc3-p101">Open extensions (formerly known as Office 365 data extensions) gives you an easy way to directly add untyped properties to a resource in Microsoft Graph. Open extensions are represented by the **openTypeExtension** resource. Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.  Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data. One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`. Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="02dc3-108">Пример открытого расширения. [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](../../../concepts/extensibility_open_users.md).</span><span class="sxs-lookup"><span data-stu-id="02dc3-108">Open extension example: [Add custom data to users using open extensions](../../../concepts/extensibility_open_users.md)</span></span>

<span data-ttu-id="02dc3-109">Открытые расширения поддерживаются указанными ниже ресурсами в соответствующих версиях — общедоступной (1.0 или бета-версии) или предварительной (бета-версии).</span><span class="sxs-lookup"><span data-stu-id="02dc3-109">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

| <span data-ttu-id="02dc3-110">Ресурс</span><span class="sxs-lookup"><span data-stu-id="02dc3-110">Resource</span></span> | <span data-ttu-id="02dc3-111">Версия</span><span class="sxs-lookup"><span data-stu-id="02dc3-111">Version</span></span> |
|---------------|-------|
| [<span data-ttu-id="02dc3-112">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="02dc3-112">Administrative unit</span></span>](../../beta/resources/administrativeunit.md)  | <span data-ttu-id="02dc3-113">Только предварительная версия</span><span class="sxs-lookup"><span data-stu-id="02dc3-113">Preview only</span></span> |
| <span data-ttu-id="02dc3-114">[event](event.md) для календаря</span><span class="sxs-lookup"><span data-stu-id="02dc3-114">[Calendar event](event.md)</span></span> | <span data-ttu-id="02dc3-115">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="02dc3-115">GA</span></span> |
| <span data-ttu-id="02dc3-116">[event](event.md) для календаря группы</span><span class="sxs-lookup"><span data-stu-id="02dc3-116">[Group calendar event](event.md)</span></span> | <span data-ttu-id="02dc3-117">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="02dc3-117">GA</span></span> |
| <span data-ttu-id="02dc3-118">[post](post.md) цепочки беседы группы</span><span class="sxs-lookup"><span data-stu-id="02dc3-118">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="02dc3-119">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="02dc3-119">GA</span></span> |
| [<span data-ttu-id="02dc3-120">device</span><span class="sxs-lookup"><span data-stu-id="02dc3-120">device</span></span>](device.md) | <span data-ttu-id="02dc3-121">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="02dc3-121">GA</span></span> |
| [<span data-ttu-id="02dc3-122">group</span><span class="sxs-lookup"><span data-stu-id="02dc3-122">group</span></span>](group.md) | <span data-ttu-id="02dc3-123">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="02dc3-123">GA</span></span> |
| [<span data-ttu-id="02dc3-124">message</span><span class="sxs-lookup"><span data-stu-id="02dc3-124">message</span></span>](message.md) | <span data-ttu-id="02dc3-125">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="02dc3-125">GA</span></span> |
| [<span data-ttu-id="02dc3-126">organization</span><span class="sxs-lookup"><span data-stu-id="02dc3-126">organization</span></span>](organization.md) | <span data-ttu-id="02dc3-127">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="02dc3-127">GA</span></span> |
| [<span data-ttu-id="02dc3-128">contact</span><span class="sxs-lookup"><span data-stu-id="02dc3-128">Personal contact</span></span>](contact.md) (личный контакт) | <span data-ttu-id="02dc3-129">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="02dc3-129">GA</span></span> |
| [<span data-ttu-id="02dc3-130">user</span><span class="sxs-lookup"><span data-stu-id="02dc3-130">user</span></span>](user.md) | <span data-ttu-id="02dc3-131">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="02dc3-131">GA</span></span> |

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="02dc3-132">Что использовать — открытые расширения (для ресурсов Outlook) или расширенные свойства</span><span class="sxs-lookup"><span data-stu-id="02dc3-132">Use open extensions (for Outlook resources) or extended properties?</span></span>

<span data-ttu-id="02dc3-p102">Открытые расширения — рекомендуемое решение для большинства сценариев, предполагающее хранение пользовательских данных и доступ к ним. Если вам нужно получить доступ к пользовательским данным для свойств MAPI Outlook, которые еще не предоставлены при помощи [метаданных API Microsoft Graph](http://developer.microsoft.com/en-us/graph/docs/overview/call_api), используйте [расширенные свойства и соответствующий REST API](extended-properties-overview.md). Вы можете проверить, какие свойства предоставляются с помощью метаданных, на странице https://graph.microsoft.com/v1.0/$metadata.</span><span class="sxs-lookup"><span data-stu-id="02dc3-p102">Open extensions is the recommended solution for most scenarios involving storing and accessing custom data. If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](http://developer.microsoft.com/en-us/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md). You can verify which properties the metadata exposes at https://graph.microsoft.com/v1.0/$metadata.</span></span>


## <a name="json-representation"></a><span data-ttu-id="02dc3-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="02dc3-136">JSON representation</span></span>

<span data-ttu-id="02dc3-137">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="02dc3-137">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.opentypeextension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```
## <a name="properties"></a><span data-ttu-id="02dc3-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="02dc3-138">Properties</span></span>
| <span data-ttu-id="02dc3-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="02dc3-139">Property</span></span>     | <span data-ttu-id="02dc3-140">Тип</span><span class="sxs-lookup"><span data-stu-id="02dc3-140">Type</span></span>   |<span data-ttu-id="02dc3-141">Описание</span><span class="sxs-lookup"><span data-stu-id="02dc3-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02dc3-142">extensionName</span><span class="sxs-lookup"><span data-stu-id="02dc3-142">extensionName</span></span>|<span data-ttu-id="02dc3-143">String</span><span class="sxs-lookup"><span data-stu-id="02dc3-143">String</span></span>|<span data-ttu-id="02dc3-p103">Уникальный текстовый идентификатор для открытых расширений открытого типа. Обязательно свойство.</span><span class="sxs-lookup"><span data-stu-id="02dc3-p103">A unique text identifier for an open type open extension. Required.</span></span>|
|<span data-ttu-id="02dc3-146">id</span><span class="sxs-lookup"><span data-stu-id="02dc3-146">id</span></span>|<span data-ttu-id="02dc3-147">Строка</span><span class="sxs-lookup"><span data-stu-id="02dc3-147">String</span></span>| <span data-ttu-id="02dc3-p104">Полный идентификатор, в котором сцеплены тип расширения и свойство **extensionName**. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="02dc3-p104">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02dc3-150">Отношения</span><span class="sxs-lookup"><span data-stu-id="02dc3-150">Relationships</span></span>
<span data-ttu-id="02dc3-151">Нет</span><span class="sxs-lookup"><span data-stu-id="02dc3-151">None</span></span>


## <a name="methods"></a><span data-ttu-id="02dc3-152">Методы</span><span class="sxs-lookup"><span data-stu-id="02dc3-152">Methods</span></span>

| <span data-ttu-id="02dc3-153">Метод</span><span class="sxs-lookup"><span data-stu-id="02dc3-153">Method</span></span>           | <span data-ttu-id="02dc3-154">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="02dc3-154">Return Type</span></span>    |<span data-ttu-id="02dc3-155">Описание</span><span class="sxs-lookup"><span data-stu-id="02dc3-155">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02dc3-156">Post</span><span class="sxs-lookup"><span data-stu-id="02dc3-156">Post</span></span>](../api/opentypeextension_post_opentypeextension.md) | <span data-ttu-id="02dc3-157">Объект [openTypeExtension](opentypeextension.md) (в существующем экземпляре ресурса) либо новый ресурс [contact](../resources/contact.md), [event](../resources/event.md) или [message](../resources/message.md), содержащий объект openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="02dc3-157">[openTypeExtension](opentypeextension.md) (in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object.</span></span> | <span data-ttu-id="02dc3-158">Создание объекта openTypeExtension в существующем или новом экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="02dc3-158">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="02dc3-159">Get</span><span class="sxs-lookup"><span data-stu-id="02dc3-159">Get</span></span>](../api/opentypeextension_get.md) | [<span data-ttu-id="02dc3-160">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="02dc3-160">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="02dc3-161">Чтение свойств и связей объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="02dc3-161">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="02dc3-162">Update</span><span class="sxs-lookup"><span data-stu-id="02dc3-162">Update</span></span>](../api/opentypeextension_update.md) | [<span data-ttu-id="02dc3-163">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="02dc3-163">openTypeExtension</span></span>](opentypeextension.md)   |<span data-ttu-id="02dc3-164">Обновление объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="02dc3-164">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="02dc3-165">Delete</span><span class="sxs-lookup"><span data-stu-id="02dc3-165">Delete</span></span>](../api/opentypeextension_delete.md) | <span data-ttu-id="02dc3-166">Нет</span><span class="sxs-lookup"><span data-stu-id="02dc3-166">None</span></span> |<span data-ttu-id="02dc3-167">Удаление объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="02dc3-167">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->