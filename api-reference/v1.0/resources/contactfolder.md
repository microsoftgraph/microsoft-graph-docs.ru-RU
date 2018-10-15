# <a name="contactfolder-resource-type"></a><span data-ttu-id="366a6-101">Тип ресурса contactFolder</span><span class="sxs-lookup"><span data-stu-id="366a6-101">contactFolder resource type</span></span>

<span data-ttu-id="366a6-102">Папка, содержащая контакты.</span><span class="sxs-lookup"><span data-stu-id="366a6-102">A folder that contains contacts.</span></span>

<span data-ttu-id="366a6-103">В этом ресурсе возможно использование [запроса изменений](../../../concepts/delta_query_overview.md) для отслеживания добавочных дополнений, удалений и обновлений благодаря функции [delta](../api/contactfolder_delta.md).</span><span class="sxs-lookup"><span data-stu-id="366a6-103">This resource supports using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder_delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="366a6-104">Методы</span><span class="sxs-lookup"><span data-stu-id="366a6-104">Methods</span></span>

| <span data-ttu-id="366a6-105">Метод</span><span class="sxs-lookup"><span data-stu-id="366a6-105">Method</span></span>       | <span data-ttu-id="366a6-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="366a6-106">Return Type</span></span>  |<span data-ttu-id="366a6-107">Описание</span><span class="sxs-lookup"><span data-stu-id="366a6-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="366a6-108">Получение contactFolder</span><span class="sxs-lookup"><span data-stu-id="366a6-108">Get contactFolder</span></span>](../api/contactfolder_get.md) | [<span data-ttu-id="366a6-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="366a6-109">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="366a6-110">Получение папки с контактами с помощью идентификатора папки контактов.</span><span class="sxs-lookup"><span data-stu-id="366a6-110">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="366a6-111">Обновление</span><span class="sxs-lookup"><span data-stu-id="366a6-111">Update</span></span>](../api/contactfolder_update.md) | [<span data-ttu-id="366a6-112">contactFolder</span><span class="sxs-lookup"><span data-stu-id="366a6-112">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="366a6-113">Обновление объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="366a6-113">Update contactFolder object.</span></span> |
|[<span data-ttu-id="366a6-114">Удаление</span><span class="sxs-lookup"><span data-stu-id="366a6-114">Delete</span></span>](../api/contactfolder_delete.md) | <span data-ttu-id="366a6-115">Нет</span><span class="sxs-lookup"><span data-stu-id="366a6-115">None</span></span> |<span data-ttu-id="366a6-116">Удаление объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="366a6-116">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="366a6-117">Список экземпляров childFolders</span><span class="sxs-lookup"><span data-stu-id="366a6-117">List childFolders</span></span>](../api/contactfolder_list_childfolders.md) |<span data-ttu-id="366a6-118">Коллекция [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="366a6-118">[ContactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="366a6-119">Получение коллекции дочерних папок для указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="366a6-119">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="366a6-120">Создание дочернего элемента contactFolder</span><span class="sxs-lookup"><span data-stu-id="366a6-120">Create child contactFolder</span></span>](../api/contactfolder_post_childfolders.md) |[<span data-ttu-id="366a6-121">ContactFolder</span><span class="sxs-lookup"><span data-stu-id="366a6-121">ContactFolder</span></span>](contactfolder.md)| <span data-ttu-id="366a6-122">Создание дочернего элемента contactFolder для указанной папки.</span><span class="sxs-lookup"><span data-stu-id="366a6-122">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="366a6-123">delta</span><span class="sxs-lookup"><span data-stu-id="366a6-123">delta</span></span>](../api/contact_delta.md)|<span data-ttu-id="366a6-124">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="366a6-124">[contact](contact.md) collection</span></span>| <span data-ttu-id="366a6-125">Получение набора папок контактов, которые были добавлены в почтовый ящик пользователя или удалены из него.</span><span class="sxs-lookup"><span data-stu-id="366a6-125">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="366a6-126">Список контактов в папке</span><span class="sxs-lookup"><span data-stu-id="366a6-126">List contacts in folder</span></span>](../api/contactfolder_list_contacts.md) |<span data-ttu-id="366a6-127">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="366a6-127">[Contact](contact.md) collection</span></span>| <span data-ttu-id="366a6-128">Получение коллекции контактов из стандартной папки с контактами для пользователя, выполнившего вход (`.../me/contacts`), или из указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="366a6-128">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="366a6-129">Создание контакта в папке</span><span class="sxs-lookup"><span data-stu-id="366a6-129">Create contact in folder</span></span>](../api/contactfolder_post_contacts.md) |[<span data-ttu-id="366a6-130">Contact</span><span class="sxs-lookup"><span data-stu-id="366a6-130">Contact</span></span>](contact.md)| <span data-ttu-id="366a6-131">Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="366a6-131">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="366a6-132">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="366a6-132">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="366a6-133">contactFolder</span><span class="sxs-lookup"><span data-stu-id="366a6-133">contactFolder</span></span>](contactFolder.md)  |<span data-ttu-id="366a6-134">Создание одного или несколько расширенных свойств с одним значением в новом или существующем экземпляре contactFolder.</span><span class="sxs-lookup"><span data-stu-id="366a6-134">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="366a6-135">Получение contactFolder с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="366a6-135">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="366a6-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="366a6-136">contactFolder</span></span>](contactFolder.md) | <span data-ttu-id="366a6-137">Получение экземпляров contactFolder, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="366a6-137">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="366a6-138">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="366a6-138">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="366a6-139">contactFolder</span><span class="sxs-lookup"><span data-stu-id="366a6-139">contactFolder</span></span>](contactFolder.md) | <span data-ttu-id="366a6-140">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем экземпляре contactFolder.</span><span class="sxs-lookup"><span data-stu-id="366a6-140">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="366a6-141">Получение contactFolder с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="366a6-141">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="366a6-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="366a6-142">contactFolder</span></span>](contactFolder.md) | <span data-ttu-id="366a6-143">Получение экземпляра contactFolder, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`.</span><span class="sxs-lookup"><span data-stu-id="366a6-143">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="366a6-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="366a6-144">Properties</span></span>
| <span data-ttu-id="366a6-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="366a6-145">Property</span></span>     | <span data-ttu-id="366a6-146">Тип</span><span class="sxs-lookup"><span data-stu-id="366a6-146">Type</span></span>   |<span data-ttu-id="366a6-147">Описание</span><span class="sxs-lookup"><span data-stu-id="366a6-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="366a6-148">displayName</span><span class="sxs-lookup"><span data-stu-id="366a6-148">displayName</span></span>|<span data-ttu-id="366a6-149">Строка</span><span class="sxs-lookup"><span data-stu-id="366a6-149">String</span></span>|<span data-ttu-id="366a6-150">Отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="366a6-150">The folder's display name.</span></span>|
|<span data-ttu-id="366a6-151">id</span><span class="sxs-lookup"><span data-stu-id="366a6-151">id</span></span>|<span data-ttu-id="366a6-152">Строка</span><span class="sxs-lookup"><span data-stu-id="366a6-152">String</span></span>|<span data-ttu-id="366a6-p101">Уникальный идентификатор папки с контактами. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="366a6-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="366a6-155">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="366a6-155">parentFolderId</span></span>|<span data-ttu-id="366a6-156">Строка</span><span class="sxs-lookup"><span data-stu-id="366a6-156">String</span></span>|<span data-ttu-id="366a6-157">Идентификатор родительской папки для папки.</span><span class="sxs-lookup"><span data-stu-id="366a6-157">The ID of the folder's parent folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="366a6-158">Отношения</span><span class="sxs-lookup"><span data-stu-id="366a6-158">Relationships</span></span>
| <span data-ttu-id="366a6-159">Связь</span><span class="sxs-lookup"><span data-stu-id="366a6-159">Relationship</span></span> | <span data-ttu-id="366a6-160">Тип</span><span class="sxs-lookup"><span data-stu-id="366a6-160">Type</span></span>   |<span data-ttu-id="366a6-161">Описание</span><span class="sxs-lookup"><span data-stu-id="366a6-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="366a6-162">childFolders</span><span class="sxs-lookup"><span data-stu-id="366a6-162">childFolders</span></span>|<span data-ttu-id="366a6-163">Коллекция [ContactFolder](contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="366a6-163">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="366a6-p102">Коллекция дочерних папок в папке. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="366a6-p102">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="366a6-168">contacts</span><span class="sxs-lookup"><span data-stu-id="366a6-168">contacts</span></span>|<span data-ttu-id="366a6-169">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="366a6-169">[Contact](contact.md) collection</span></span>|<span data-ttu-id="366a6-p103">Контакты в папке. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="366a6-p103">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="366a6-174">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="366a6-174">multiValueExtendedProperties</span></span>|<span data-ttu-id="366a6-175">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="366a6-175">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="366a6-p104">Коллекция расширенных свойств с несколькими значениями, определенных для contactFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="366a6-p104">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="366a6-179">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="366a6-179">singleValueExtendedProperties</span></span>|<span data-ttu-id="366a6-180">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="366a6-180">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="366a6-p105">Коллекция расширенных свойств с одним значением, определенных для contactFolder. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="366a6-p105">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="366a6-184">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="366a6-184">JSON representation</span></span>

<span data-ttu-id="366a6-185">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="366a6-185">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.contactFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "navigability": "single",
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string"
}

```

## <a name="see-also"></a><span data-ttu-id="366a6-186">См. также</span><span class="sxs-lookup"><span data-stu-id="366a6-186">See also</span></span>

- [<span data-ttu-id="366a6-187">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="366a6-187">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="366a6-188">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="366a6-188">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
