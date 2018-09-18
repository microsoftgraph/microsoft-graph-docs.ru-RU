# <a name="contact-resource-type"></a><span data-ttu-id="d55a5-101">Тип ресурса contact</span><span class="sxs-lookup"><span data-stu-id="d55a5-101">contact resource type</span></span>

<span data-ttu-id="d55a5-p101">Контакт — элемент в Outlook, в котором вы можете упорядочить и хранить сведения о людях и организациях, с которыми поддерживаете связь. Контакты содержатся в папках контактов.</span><span class="sxs-lookup"><span data-stu-id="d55a5-p101">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="d55a5-104">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="d55a5-104">This resource supports:</span></span>

- <span data-ttu-id="d55a5-105">Добавление собственных данных к настраиваемым свойствам в качестве [расширений](../../../concepts/extensibility_overview.md).</span><span class="sxs-lookup"><span data-stu-id="d55a5-105">Adding your own data to custom properties using [extensions](../../../concepts/extensibility_overview.md).</span></span>
- <span data-ttu-id="d55a5-106">Подписка на [уведомления об изменении](../../../concepts/webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="d55a5-106">Subscribing to [change notifications](../../../concepts/webhooks.md).</span></span>
- <span data-ttu-id="d55a5-107">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](../../../concepts/delta_query_overview.md) (функция [delta](../api/contact_delta.md)).</span><span class="sxs-lookup"><span data-stu-id="d55a5-107">Using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact_delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="d55a5-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d55a5-108">Methods</span></span>

| <span data-ttu-id="d55a5-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d55a5-109">Method</span></span>       | <span data-ttu-id="d55a5-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d55a5-110">Return Type</span></span>  |<span data-ttu-id="d55a5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d55a5-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d55a5-112">Получение контакта</span><span class="sxs-lookup"><span data-stu-id="d55a5-112">Get contact</span></span>](../api/contact_get.md) | [<span data-ttu-id="d55a5-113">contact</span><span class="sxs-lookup"><span data-stu-id="d55a5-113">contact</span></span>](contact.md) |<span data-ttu-id="d55a5-114">Считывание свойств и отношений объекта contact.</span><span class="sxs-lookup"><span data-stu-id="d55a5-114">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="d55a5-115">Создание</span><span class="sxs-lookup"><span data-stu-id="d55a5-115">Create</span></span>](../api/user_post_contacts.md) | [<span data-ttu-id="d55a5-116">contact</span><span class="sxs-lookup"><span data-stu-id="d55a5-116">contact</span></span>](contact.md) |<span data-ttu-id="d55a5-117">Добавление контакта в корневую папку с контактами или конечную точку контактов другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="d55a5-117">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="d55a5-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="d55a5-118">Update</span></span>](../api/contact_update.md) | [<span data-ttu-id="d55a5-119">contact</span><span class="sxs-lookup"><span data-stu-id="d55a5-119">contact</span></span>](contact.md) |<span data-ttu-id="d55a5-120">Обновление объекта contact.</span><span class="sxs-lookup"><span data-stu-id="d55a5-120">Update contact object.</span></span> |
|[<span data-ttu-id="d55a5-121">Удаление</span><span class="sxs-lookup"><span data-stu-id="d55a5-121">Delete</span></span>](../api/contact_delete.md) | <span data-ttu-id="d55a5-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d55a5-122">None</span></span> |<span data-ttu-id="d55a5-123">Удаление объекта contact.</span><span class="sxs-lookup"><span data-stu-id="d55a5-123">Delete contact object.</span></span> |
|[<span data-ttu-id="d55a5-124">delta</span><span class="sxs-lookup"><span data-stu-id="d55a5-124">delta</span></span>](../api/contact_delta.md)|<span data-ttu-id="d55a5-125">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="d55a5-125">[contact](contact.md) collection</span></span>| <span data-ttu-id="d55a5-126">Получение набора контактов, которые были добавлены в указанную папку, обновлены в ней или удалены из нее.</span><span class="sxs-lookup"><span data-stu-id="d55a5-126">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="d55a5-127">**Открытые расширения**</span><span class="sxs-lookup"><span data-stu-id="d55a5-127">**Open extensions**</span></span>| | |
|[<span data-ttu-id="d55a5-128">Создание открытого расширения</span><span class="sxs-lookup"><span data-stu-id="d55a5-128">Create open extension</span></span>](../api/opentypeextension_post_opentypeextension.md) |[<span data-ttu-id="d55a5-129">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="d55a5-129">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="d55a5-130">Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.</span><span class="sxs-lookup"><span data-stu-id="d55a5-130">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="d55a5-131">Получение открытого расширения</span><span class="sxs-lookup"><span data-stu-id="d55a5-131">Get open extension</span></span>](../api/opentypeextension_get.md) |<span data-ttu-id="d55a5-132">Коллекция [openTypeExtension](opentypeextension.md)</span><span class="sxs-lookup"><span data-stu-id="d55a5-132">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="d55a5-133">Получение объектов открытого расширения, которые определяются по имени или полному имени.</span><span class="sxs-lookup"><span data-stu-id="d55a5-133">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="d55a5-134">**Расширения схемы**</span><span class="sxs-lookup"><span data-stu-id="d55a5-134">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="d55a5-135">Добавление значений расширений для схемы</span><span class="sxs-lookup"><span data-stu-id="d55a5-135">Add schema extension values</span></span>](../../../concepts/extensibility_schema_groups.md) || <span data-ttu-id="d55a5-136">Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.</span><span class="sxs-lookup"><span data-stu-id="d55a5-136">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="d55a5-137">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="d55a5-137">**Extended properties**</span></span>| | |
|[<span data-ttu-id="d55a5-138">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="d55a5-138">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="d55a5-139">contact</span><span class="sxs-lookup"><span data-stu-id="d55a5-139">contact</span></span>](contact.md)  |<span data-ttu-id="d55a5-140">Создание одного или нескольких расширенных свойств с одним значением в новом или существующем контакте.</span><span class="sxs-lookup"><span data-stu-id="d55a5-140">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="d55a5-141">Получение контакта с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="d55a5-141">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="d55a5-142">contact</span><span class="sxs-lookup"><span data-stu-id="d55a5-142">contact</span></span>](contact.md) | <span data-ttu-id="d55a5-143">Получение контактов, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="d55a5-143">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="d55a5-144">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="d55a5-144">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="d55a5-145">contact</span><span class="sxs-lookup"><span data-stu-id="d55a5-145">contact</span></span>](contact.md) | <span data-ttu-id="d55a5-146">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем контакте.</span><span class="sxs-lookup"><span data-stu-id="d55a5-146">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="d55a5-147">Получение контакта с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="d55a5-147">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="d55a5-148">contact</span><span class="sxs-lookup"><span data-stu-id="d55a5-148">contact</span></span>](contact.md) | <span data-ttu-id="d55a5-149">Получение контакта, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`.</span><span class="sxs-lookup"><span data-stu-id="d55a5-149">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="d55a5-150">Свойства</span><span class="sxs-lookup"><span data-stu-id="d55a5-150">Properties</span></span>
| <span data-ttu-id="d55a5-151">Свойство</span><span class="sxs-lookup"><span data-stu-id="d55a5-151">Property</span></span>     | <span data-ttu-id="d55a5-152">Тип</span><span class="sxs-lookup"><span data-stu-id="d55a5-152">Type</span></span>   |<span data-ttu-id="d55a5-153">Описание</span><span class="sxs-lookup"><span data-stu-id="d55a5-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d55a5-154">assistantName</span><span class="sxs-lookup"><span data-stu-id="d55a5-154">assistantName</span></span>|<span data-ttu-id="d55a5-155">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-155">String</span></span>|<span data-ttu-id="d55a5-156">Имя помощника контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-156">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="d55a5-157">birthday</span><span class="sxs-lookup"><span data-stu-id="d55a5-157">birthday</span></span>|<span data-ttu-id="d55a5-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d55a5-158">DateTimeOffset</span></span>|<span data-ttu-id="d55a5-p102">Дата рождения контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d55a5-p102">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d55a5-162">businessAddress</span><span class="sxs-lookup"><span data-stu-id="d55a5-162">businessAddress</span></span>|[<span data-ttu-id="d55a5-163">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="d55a5-163">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="d55a5-164">Рабочий адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-164">The contact's business address.</span></span>|
|<span data-ttu-id="d55a5-165">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="d55a5-165">businessHomePage</span></span>|<span data-ttu-id="d55a5-166">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-166">String</span></span>|<span data-ttu-id="d55a5-167">Домашняя страница контакта (рабочая).</span><span class="sxs-lookup"><span data-stu-id="d55a5-167">The business home page of the contact.</span></span>|
|<span data-ttu-id="d55a5-168">businessPhones</span><span class="sxs-lookup"><span data-stu-id="d55a5-168">businessPhones</span></span>|<span data-ttu-id="d55a5-169">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d55a5-169">String collection</span></span>|<span data-ttu-id="d55a5-170">Рабочие номера телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-170">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="d55a5-171">categories</span><span class="sxs-lookup"><span data-stu-id="d55a5-171">categories</span></span>|<span data-ttu-id="d55a5-172">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d55a5-172">String collection</span></span>|<span data-ttu-id="d55a5-173">Категории, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="d55a5-173">The categories associated with the contact.</span></span>|
|<span data-ttu-id="d55a5-174">changeKey</span><span class="sxs-lookup"><span data-stu-id="d55a5-174">changeKey</span></span>|<span data-ttu-id="d55a5-175">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-175">String</span></span>|<span data-ttu-id="d55a5-p103">Указывает версию контакта. При каждом изменении контакта также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-p103">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="d55a5-179">children</span><span class="sxs-lookup"><span data-stu-id="d55a5-179">children</span></span>|<span data-ttu-id="d55a5-180">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d55a5-180">String collection</span></span>|<span data-ttu-id="d55a5-181">Имена детей контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-181">The names of the contact's children.</span></span>|
|<span data-ttu-id="d55a5-182">companyName</span><span class="sxs-lookup"><span data-stu-id="d55a5-182">companyName</span></span>|<span data-ttu-id="d55a5-183">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-183">String</span></span>|<span data-ttu-id="d55a5-184">Название компании контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-184">The name of the contact's company.</span></span>|
|<span data-ttu-id="d55a5-185">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d55a5-185">createdDateTime</span></span>|<span data-ttu-id="d55a5-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d55a5-186">DateTimeOffset</span></span>|<span data-ttu-id="d55a5-p104">Время создания контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d55a5-p104">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d55a5-190">отделу;</span><span class="sxs-lookup"><span data-stu-id="d55a5-190">department</span></span>|<span data-ttu-id="d55a5-191">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-191">String</span></span>|<span data-ttu-id="d55a5-192">Отдел контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-192">The contact's department.</span></span>|
|<span data-ttu-id="d55a5-193">displayName</span><span class="sxs-lookup"><span data-stu-id="d55a5-193">displayName</span></span>|<span data-ttu-id="d55a5-194">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-194">String</span></span>|<span data-ttu-id="d55a5-195">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-195">The contact's display name.</span></span>|
|<span data-ttu-id="d55a5-196">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="d55a5-196">emailAddresses</span></span>|<span data-ttu-id="d55a5-197">Коллекция [EmailAddress](emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="d55a5-197">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="d55a5-198">Электронные адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-198">The contact's email addresses.</span></span>|
|<span data-ttu-id="d55a5-199">flag</span><span class="sxs-lookup"><span data-stu-id="d55a5-199">flag</span></span>|[<span data-ttu-id="d55a5-200">followupFlag</span><span class="sxs-lookup"><span data-stu-id="d55a5-200">followUpFlag</span></span>](followupflag.md)|<span data-ttu-id="d55a5-201">Значение флага, которое указывает статус, дату начала, дату выполнения или дату завершения для сообщения.</span><span class="sxs-lookup"><span data-stu-id="d55a5-201">The flag value that indicates the status, start date, due date, or completion date for the message.</span></span>|
|<span data-ttu-id="d55a5-202">fileAs</span><span class="sxs-lookup"><span data-stu-id="d55a5-202">fileAs</span></span>|<span data-ttu-id="d55a5-203">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-203">String</span></span>|<span data-ttu-id="d55a5-204">Имя, под которым хранится контакт.</span><span class="sxs-lookup"><span data-stu-id="d55a5-204">The name the contact is filed under.</span></span>|
|<span data-ttu-id="d55a5-205">generation</span><span class="sxs-lookup"><span data-stu-id="d55a5-205">generation</span></span>|<span data-ttu-id="d55a5-206">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-206">String</span></span>|<span data-ttu-id="d55a5-207">Поколение контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-207">The contact's generation.</span></span>|
|<span data-ttu-id="d55a5-208">givenName</span><span class="sxs-lookup"><span data-stu-id="d55a5-208">givenName</span></span>|<span data-ttu-id="d55a5-209">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-209">String</span></span>|<span data-ttu-id="d55a5-210">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-210">The contact's given name.</span></span>|
|<span data-ttu-id="d55a5-211">homeAddress</span><span class="sxs-lookup"><span data-stu-id="d55a5-211">homeAddress</span></span>|[<span data-ttu-id="d55a5-212">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="d55a5-212">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="d55a5-213">Домашний адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-213">The contact's home address.</span></span>|
|<span data-ttu-id="d55a5-214">homePhones</span><span class="sxs-lookup"><span data-stu-id="d55a5-214">homePhones</span></span>|<span data-ttu-id="d55a5-215">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d55a5-215">String collection</span></span>|<span data-ttu-id="d55a5-216">Номера домашних телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-216">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="d55a5-217">id</span><span class="sxs-lookup"><span data-stu-id="d55a5-217">id</span></span>|<span data-ttu-id="d55a5-218">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-218">String</span></span>|<span data-ttu-id="d55a5-p105">Уникальный идентификатор контакта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d55a5-p105">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="d55a5-221">imAddresses</span><span class="sxs-lookup"><span data-stu-id="d55a5-221">imAddresses</span></span>|<span data-ttu-id="d55a5-222">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d55a5-222">String collection</span></span>|<span data-ttu-id="d55a5-223">Адреса контакта для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="d55a5-223">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="d55a5-224">initials</span><span class="sxs-lookup"><span data-stu-id="d55a5-224">initials</span></span>|<span data-ttu-id="d55a5-225">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-225">String</span></span>|<span data-ttu-id="d55a5-226">Инициалы контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-226">The contact's initials.</span></span>|
|<span data-ttu-id="d55a5-227">jobTitle</span><span class="sxs-lookup"><span data-stu-id="d55a5-227">jobTitle</span></span>|<span data-ttu-id="d55a5-228">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-228">String</span></span>|<span data-ttu-id="d55a5-229">Должность контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-229">The contact’s job title.</span></span>|
|<span data-ttu-id="d55a5-230">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d55a5-230">lastModifiedDateTime</span></span>|<span data-ttu-id="d55a5-231">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d55a5-231">DateTimeOffset</span></span>|<span data-ttu-id="d55a5-p106">Время изменения контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d55a5-p106">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d55a5-235">manager</span><span class="sxs-lookup"><span data-stu-id="d55a5-235">manager</span></span>|<span data-ttu-id="d55a5-236">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-236">String</span></span>|<span data-ttu-id="d55a5-237">Имя руководителя контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-237">The name of the contact's manager.</span></span>
|<span data-ttu-id="d55a5-238">middleName</span><span class="sxs-lookup"><span data-stu-id="d55a5-238">middleName</span></span>|<span data-ttu-id="d55a5-239">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-239">String</span></span>|<span data-ttu-id="d55a5-240">Отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-240">The contact's middle name.</span></span>|
|<span data-ttu-id="d55a5-241">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="d55a5-241">mobilePhone</span></span>|<span data-ttu-id="d55a5-242">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-242">String</span></span>|<span data-ttu-id="d55a5-243">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-243">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="d55a5-244">nickName</span><span class="sxs-lookup"><span data-stu-id="d55a5-244">nickName</span></span>|<span data-ttu-id="d55a5-245">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-245">String</span></span>|<span data-ttu-id="d55a5-246">Псевдоним контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-246">The contact's nickname.</span></span>|
|<span data-ttu-id="d55a5-247">officeLocation</span><span class="sxs-lookup"><span data-stu-id="d55a5-247">officeLocation</span></span>|<span data-ttu-id="d55a5-248">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-248">String</span></span>|<span data-ttu-id="d55a5-249">Расположение офиса контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-249">The location of the contact's office.</span></span>|
|<span data-ttu-id="d55a5-250">otherAddress</span><span class="sxs-lookup"><span data-stu-id="d55a5-250">otherAddress</span></span>|[<span data-ttu-id="d55a5-251">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="d55a5-251">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="d55a5-252">Другие адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-252">Other addresses for the contact.</span></span>|
|<span data-ttu-id="d55a5-253">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="d55a5-253">parentFolderId</span></span>|<span data-ttu-id="d55a5-254">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-254">String</span></span>|<span data-ttu-id="d55a5-255">Идентификатор родительской папки контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-255">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="d55a5-256">personalNotes</span><span class="sxs-lookup"><span data-stu-id="d55a5-256">personalNotes</span></span>|<span data-ttu-id="d55a5-257">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-257">String</span></span>|<span data-ttu-id="d55a5-258">Заметки пользователя о контакте.</span><span class="sxs-lookup"><span data-stu-id="d55a5-258">The user's notes about the contact.</span></span>|
|<span data-ttu-id="d55a5-259">profession</span><span class="sxs-lookup"><span data-stu-id="d55a5-259">profession</span></span>|<span data-ttu-id="d55a5-260">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-260">String</span></span>|<span data-ttu-id="d55a5-261">Профессия контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-261">The contact's profession.</span></span>|
|<span data-ttu-id="d55a5-262">spouseName</span><span class="sxs-lookup"><span data-stu-id="d55a5-262">spouseName</span></span>|<span data-ttu-id="d55a5-263">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-263">String</span></span>|<span data-ttu-id="d55a5-264">Имя супруга или супруги контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-264">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="d55a5-265">surname</span><span class="sxs-lookup"><span data-stu-id="d55a5-265">surname</span></span>|<span data-ttu-id="d55a5-266">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-266">String</span></span>|<span data-ttu-id="d55a5-267">Фамилия контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-267">The contact's surname.</span></span>|
|<span data-ttu-id="d55a5-268">title</span><span class="sxs-lookup"><span data-stu-id="d55a5-268">title</span></span>|<span data-ttu-id="d55a5-269">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-269">String</span></span>|<span data-ttu-id="d55a5-270">Звание контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-270">The contact's title.</span></span>|
|<span data-ttu-id="d55a5-271">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="d55a5-271">yomiCompanyName</span></span>|<span data-ttu-id="d55a5-272">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-272">String</span></span>|<span data-ttu-id="d55a5-273">Название компании контакта, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="d55a5-273">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="d55a5-274">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="d55a5-274">yomiGivenName</span></span>|<span data-ttu-id="d55a5-275">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-275">String</span></span>|<span data-ttu-id="d55a5-276">Имя контакта, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="d55a5-276">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="d55a5-277">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="d55a5-277">yomiSurname</span></span>|<span data-ttu-id="d55a5-278">Строка</span><span class="sxs-lookup"><span data-stu-id="d55a5-278">String</span></span>|<span data-ttu-id="d55a5-279">Фамилия контакта, записанная так, как она звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="d55a5-279">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d55a5-280">Отношения</span><span class="sxs-lookup"><span data-stu-id="d55a5-280">Relationships</span></span>
| <span data-ttu-id="d55a5-281">Связь</span><span class="sxs-lookup"><span data-stu-id="d55a5-281">Relationship</span></span> | <span data-ttu-id="d55a5-282">Тип</span><span class="sxs-lookup"><span data-stu-id="d55a5-282">Type</span></span>   |<span data-ttu-id="d55a5-283">Описание</span><span class="sxs-lookup"><span data-stu-id="d55a5-283">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d55a5-284">extensions</span><span class="sxs-lookup"><span data-stu-id="d55a5-284">extensions</span></span>|<span data-ttu-id="d55a5-285">Коллекция [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="d55a5-285">[extension](extension.md) collection</span></span>|<span data-ttu-id="d55a5-p107">Коллекция открытых расширений, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d55a5-p107">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d55a5-289">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d55a5-289">multiValueExtendedProperties</span></span>|<span data-ttu-id="d55a5-290">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="d55a5-290">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d55a5-p108">Коллекция расширенных свойств с несколькими значениями, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d55a5-p108">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d55a5-294">photo</span><span class="sxs-lookup"><span data-stu-id="d55a5-294">photo</span></span>|[<span data-ttu-id="d55a5-295">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="d55a5-295">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="d55a5-p109">Необязательное фото контакта. Можно получить или задать фото для контакта.</span><span class="sxs-lookup"><span data-stu-id="d55a5-p109">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="d55a5-298">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d55a5-298">singleValueExtendedProperties</span></span>|<span data-ttu-id="d55a5-299">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="d55a5-299">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d55a5-p110">Коллекция расширенных свойств с одним значением, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d55a5-p110">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d55a5-303">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d55a5-303">JSON representation</span></span>

<span data-ttu-id="d55a5-304">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d55a5-304">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.outlookItem",
  "openType": true,
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contact",
  "@odata.annotations": [
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "assistantName": "string",
  "birthday": "String (timestamp)",
  "businessAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "businessHomePage": "string",
  "businessPhones": ["string"],
  "categories": ["string"],
  "changeKey": "string",
  "children": ["string"],
  "companyName": "string",
  "createdDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.emailAddress"}],
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "fileAs": "string",
  "generation": "string",
  "givenName": "string",
  "homeAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "homePhones": ["string"],
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "initials": "string",
  "jobTitle": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "manager": "string",
  "middleName": "string",
  "mobilePhone": "string",
  "nickName": "string",
  "officeLocation": "string",
  "otherAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "parentFolderId": "string",
  "personalNotes": "string",
  "profession": "string",
  "spouseName": "string",
  "surname": "string",
  "title": "string",
  "yomiCompanyName": "string",
  "yomiGivenName": "string",
  "yomiSurname": "string",

  "photo": { "@odata.type": "microsoft.graph.profilePhoto" }
}

```

## <a name="see-also"></a><span data-ttu-id="d55a5-305">См. также</span><span class="sxs-lookup"><span data-stu-id="d55a5-305">See also</span></span>

- [<span data-ttu-id="d55a5-306">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="d55a5-306">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="d55a5-307">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="d55a5-307">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)
- [<span data-ttu-id="d55a5-308">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="d55a5-308">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="d55a5-309">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="d55a5-309">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="d55a5-310">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="d55a5-310">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
