# <a name="contact-resource-type"></a><span data-ttu-id="b5cd7-101">Тип ресурса contact</span><span class="sxs-lookup"><span data-stu-id="b5cd7-101">contact resource type</span></span>

<span data-ttu-id="b5cd7-p101">Контакт — элемент в Outlook, в котором вы можете упорядочить и хранить сведения о людях и организациях, с которыми поддерживаете связь. Контакты содержатся в папках контактов.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-p101">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="b5cd7-104">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="b5cd7-104">This resource supports:</span></span>

- <span data-ttu-id="b5cd7-105">добавление собственных данных к настраиваемым свойствам с помощью [расширений](../../../concepts/extensibility_overview.md);</span><span class="sxs-lookup"><span data-stu-id="b5cd7-105">Adding your own data to custom properties using [extensions](../../../concepts/extensibility_overview.md).</span></span>
- <span data-ttu-id="b5cd7-106">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](../../../concepts/delta_query_overview.md) (функция [delta](../api/contact_delta.md)).</span><span class="sxs-lookup"><span data-stu-id="b5cd7-106">Using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact_delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="b5cd7-107">Методы</span><span class="sxs-lookup"><span data-stu-id="b5cd7-107">Methods</span></span>

| <span data-ttu-id="b5cd7-108">Метод</span><span class="sxs-lookup"><span data-stu-id="b5cd7-108">Method</span></span>       | <span data-ttu-id="b5cd7-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b5cd7-109">Return Type</span></span>  |<span data-ttu-id="b5cd7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b5cd7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b5cd7-111">Получение контакта</span><span class="sxs-lookup"><span data-stu-id="b5cd7-111">Get contact</span></span>](../api/contact_get.md) | [<span data-ttu-id="b5cd7-112">contact</span><span class="sxs-lookup"><span data-stu-id="b5cd7-112">contact</span></span>](contact.md) |<span data-ttu-id="b5cd7-113">Считывание свойств и отношений объекта contact.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-113">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="b5cd7-114">Создание</span><span class="sxs-lookup"><span data-stu-id="b5cd7-114">Create</span></span>](../api/user_post_contacts.md) | [<span data-ttu-id="b5cd7-115">contact</span><span class="sxs-lookup"><span data-stu-id="b5cd7-115">contact</span></span>](contact.md) |<span data-ttu-id="b5cd7-116">Добавление контакта в корневую папку с контактами или конечную точку контактов другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-116">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="b5cd7-117">Обновление</span><span class="sxs-lookup"><span data-stu-id="b5cd7-117">Update</span></span>](../api/contact_update.md) | [<span data-ttu-id="b5cd7-118">contact</span><span class="sxs-lookup"><span data-stu-id="b5cd7-118">contact</span></span>](contact.md) |<span data-ttu-id="b5cd7-119">Обновление объекта contact.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-119">Update contact object.</span></span> |
|[<span data-ttu-id="b5cd7-120">Удаление</span><span class="sxs-lookup"><span data-stu-id="b5cd7-120">Delete</span></span>](../api/contact_delete.md) | <span data-ttu-id="b5cd7-121">Нет</span><span class="sxs-lookup"><span data-stu-id="b5cd7-121">None</span></span> |<span data-ttu-id="b5cd7-122">Удаление объекта contact.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-122">Delete contact object.</span></span> |
|[<span data-ttu-id="b5cd7-123">delta</span><span class="sxs-lookup"><span data-stu-id="b5cd7-123">delta</span></span>](../api/contact_delta.md)|<span data-ttu-id="b5cd7-124">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="b5cd7-124">[contact](contact.md) collection</span></span>| <span data-ttu-id="b5cd7-125">Получение набора контактов, которые были добавлены в указанную папку, обновлены в ней или удалены из нее.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-125">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="b5cd7-126">**Открытые расширения**</span><span class="sxs-lookup"><span data-stu-id="b5cd7-126">**Open extensions**</span></span>| | |
|[<span data-ttu-id="b5cd7-127">Создание открытого расширения</span><span class="sxs-lookup"><span data-stu-id="b5cd7-127">Create open extension</span></span>](../api/opentypeextension_post_opentypeextension.md) |[<span data-ttu-id="b5cd7-128">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="b5cd7-128">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="b5cd7-129">Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-129">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="b5cd7-130">Получение открытого расширения</span><span class="sxs-lookup"><span data-stu-id="b5cd7-130">Get open extension</span></span>](../api/opentypeextension_get.md) |<span data-ttu-id="b5cd7-131">Коллекция [openTypeExtension](opentypeextension.md)</span><span class="sxs-lookup"><span data-stu-id="b5cd7-131">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="b5cd7-132">Получение объектов открытого расширения, которые определяются по имени или полному имени.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-132">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="b5cd7-133">**Расширения схемы**</span><span class="sxs-lookup"><span data-stu-id="b5cd7-133">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="b5cd7-134">Добавление значений расширений для схемы</span><span class="sxs-lookup"><span data-stu-id="b5cd7-134">Add schema extension values</span></span>](../../../concepts/extensibility_schema_groups.md) || <span data-ttu-id="b5cd7-135">Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-135">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="b5cd7-136">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="b5cd7-136">**Extended properties**</span></span>| | |
|[<span data-ttu-id="b5cd7-137">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="b5cd7-137">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="b5cd7-138">contact</span><span class="sxs-lookup"><span data-stu-id="b5cd7-138">contact</span></span>](contact.md)  |<span data-ttu-id="b5cd7-139">Создание одного или нескольких расширенных свойств с одним значением в новом или существующем контакте.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-139">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="b5cd7-140">Получение контакта с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="b5cd7-140">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="b5cd7-141">contact</span><span class="sxs-lookup"><span data-stu-id="b5cd7-141">contact</span></span>](contact.md) | <span data-ttu-id="b5cd7-142">Получение контактов, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-142">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="b5cd7-143">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="b5cd7-143">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="b5cd7-144">contact</span><span class="sxs-lookup"><span data-stu-id="b5cd7-144">contact</span></span>](contact.md) | <span data-ttu-id="b5cd7-145">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем контакте.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-145">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="b5cd7-146">Получение контакта с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="b5cd7-146">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="b5cd7-147">contact</span><span class="sxs-lookup"><span data-stu-id="b5cd7-147">contact</span></span>](contact.md) | <span data-ttu-id="b5cd7-148">Получение контакта, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-148">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="b5cd7-149">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5cd7-149">Properties</span></span>
| <span data-ttu-id="b5cd7-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5cd7-150">Property</span></span>     | <span data-ttu-id="b5cd7-151">Тип</span><span class="sxs-lookup"><span data-stu-id="b5cd7-151">Type</span></span>   |<span data-ttu-id="b5cd7-152">Описание</span><span class="sxs-lookup"><span data-stu-id="b5cd7-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5cd7-153">assistantName</span><span class="sxs-lookup"><span data-stu-id="b5cd7-153">assistantName</span></span>|<span data-ttu-id="b5cd7-154">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-154">String</span></span>|<span data-ttu-id="b5cd7-155">Имя помощника контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-155">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="b5cd7-156">birthday</span><span class="sxs-lookup"><span data-stu-id="b5cd7-156">birthday</span></span>|<span data-ttu-id="b5cd7-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5cd7-157">DateTimeOffset</span></span>|<span data-ttu-id="b5cd7-p102">Дата рождения контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b5cd7-p102">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b5cd7-161">businessAddress</span><span class="sxs-lookup"><span data-stu-id="b5cd7-161">businessAddress</span></span>|[<span data-ttu-id="b5cd7-162">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="b5cd7-162">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="b5cd7-163">Рабочий адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-163">The contact's business address.</span></span>|
|<span data-ttu-id="b5cd7-164">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="b5cd7-164">businessHomePage</span></span>|<span data-ttu-id="b5cd7-165">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-165">String</span></span>|<span data-ttu-id="b5cd7-166">Домашняя страница контакта (рабочая).</span><span class="sxs-lookup"><span data-stu-id="b5cd7-166">The business home page of the contact.</span></span>|
|<span data-ttu-id="b5cd7-167">businessPhones</span><span class="sxs-lookup"><span data-stu-id="b5cd7-167">businessPhones</span></span>|<span data-ttu-id="b5cd7-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b5cd7-168">String collection</span></span>|<span data-ttu-id="b5cd7-169">Рабочие номера телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-169">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="b5cd7-170">categories</span><span class="sxs-lookup"><span data-stu-id="b5cd7-170">categories</span></span>|<span data-ttu-id="b5cd7-171">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b5cd7-171">String collection</span></span>|<span data-ttu-id="b5cd7-172">Категории, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-172">The categories associated with the contact.</span></span>|
|<span data-ttu-id="b5cd7-173">changeKey</span><span class="sxs-lookup"><span data-stu-id="b5cd7-173">changeKey</span></span>|<span data-ttu-id="b5cd7-174">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-174">String</span></span>|<span data-ttu-id="b5cd7-p103">Указывает версию контакта. При каждом изменении контакта также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-p103">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="b5cd7-178">children</span><span class="sxs-lookup"><span data-stu-id="b5cd7-178">children</span></span>|<span data-ttu-id="b5cd7-179">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b5cd7-179">String collection</span></span>|<span data-ttu-id="b5cd7-180">Имена детей контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-180">The names of the contact's children.</span></span>|
|<span data-ttu-id="b5cd7-181">companyName</span><span class="sxs-lookup"><span data-stu-id="b5cd7-181">companyName</span></span>|<span data-ttu-id="b5cd7-182">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-182">String</span></span>|<span data-ttu-id="b5cd7-183">Название компании контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-183">The name of the contact's company.</span></span>|
|<span data-ttu-id="b5cd7-184">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5cd7-184">createdDateTime</span></span>|<span data-ttu-id="b5cd7-185">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5cd7-185">DateTimeOffset</span></span>|<span data-ttu-id="b5cd7-p104">Время создания контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b5cd7-p104">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b5cd7-189">отделу;</span><span class="sxs-lookup"><span data-stu-id="b5cd7-189">department</span></span>|<span data-ttu-id="b5cd7-190">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-190">String</span></span>|<span data-ttu-id="b5cd7-191">Отдел контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-191">The contact's department.</span></span>|
|<span data-ttu-id="b5cd7-192">displayName</span><span class="sxs-lookup"><span data-stu-id="b5cd7-192">displayName</span></span>|<span data-ttu-id="b5cd7-193">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-193">String</span></span>|<span data-ttu-id="b5cd7-194">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-194">The contact's display name.</span></span>|
|<span data-ttu-id="b5cd7-195">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="b5cd7-195">emailAddresses</span></span>|<span data-ttu-id="b5cd7-196">Коллекция [EmailAddress](emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="b5cd7-196">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="b5cd7-197">Электронные адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-197">The contact's email addresses.</span></span>|
|<span data-ttu-id="b5cd7-198">flag</span><span class="sxs-lookup"><span data-stu-id="b5cd7-198">flag</span></span>|[<span data-ttu-id="b5cd7-199">followupFlag</span><span class="sxs-lookup"><span data-stu-id="b5cd7-199">followUpFlag</span></span>](followupflag.md)|<span data-ttu-id="b5cd7-200">Значение флага, которое указывает статус, дату начала, дату выполнения или дату завершения для сообщения.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-200">The flag value that indicates the status, start date, due date, or completion date for the message.</span></span>|
|<span data-ttu-id="b5cd7-201">fileAs</span><span class="sxs-lookup"><span data-stu-id="b5cd7-201">fileAs</span></span>|<span data-ttu-id="b5cd7-202">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-202">String</span></span>|<span data-ttu-id="b5cd7-203">Имя, под которым хранится контакт.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-203">The name the contact is filed under.</span></span>|
|<span data-ttu-id="b5cd7-204">generation</span><span class="sxs-lookup"><span data-stu-id="b5cd7-204">generation</span></span>|<span data-ttu-id="b5cd7-205">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-205">String</span></span>|<span data-ttu-id="b5cd7-206">Поколение контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-206">The contact's generation.</span></span>|
|<span data-ttu-id="b5cd7-207">givenName</span><span class="sxs-lookup"><span data-stu-id="b5cd7-207">givenName</span></span>|<span data-ttu-id="b5cd7-208">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-208">String</span></span>|<span data-ttu-id="b5cd7-209">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-209">The contact's given name.</span></span>|
|<span data-ttu-id="b5cd7-210">homeAddress</span><span class="sxs-lookup"><span data-stu-id="b5cd7-210">homeAddress</span></span>|[<span data-ttu-id="b5cd7-211">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="b5cd7-211">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="b5cd7-212">Домашний адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-212">The contact's home address.</span></span>|
|<span data-ttu-id="b5cd7-213">homePhones</span><span class="sxs-lookup"><span data-stu-id="b5cd7-213">homePhones</span></span>|<span data-ttu-id="b5cd7-214">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b5cd7-214">String collection</span></span>|<span data-ttu-id="b5cd7-215">Номера домашних телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-215">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="b5cd7-216">id</span><span class="sxs-lookup"><span data-stu-id="b5cd7-216">id</span></span>|<span data-ttu-id="b5cd7-217">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-217">String</span></span>|<span data-ttu-id="b5cd7-p105">Уникальный идентификатор контакта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-p105">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="b5cd7-220">imAddresses</span><span class="sxs-lookup"><span data-stu-id="b5cd7-220">imAddresses</span></span>|<span data-ttu-id="b5cd7-221">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b5cd7-221">String collection</span></span>|<span data-ttu-id="b5cd7-222">Адреса контакта для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-222">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="b5cd7-223">initials</span><span class="sxs-lookup"><span data-stu-id="b5cd7-223">initials</span></span>|<span data-ttu-id="b5cd7-224">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-224">String</span></span>|<span data-ttu-id="b5cd7-225">Инициалы контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-225">The contact's initials.</span></span>|
|<span data-ttu-id="b5cd7-226">jobTitle</span><span class="sxs-lookup"><span data-stu-id="b5cd7-226">jobTitle</span></span>|<span data-ttu-id="b5cd7-227">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-227">String</span></span>|<span data-ttu-id="b5cd7-228">Должность контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-228">The contact’s job title.</span></span>|
|<span data-ttu-id="b5cd7-229">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5cd7-229">lastModifiedDateTime</span></span>|<span data-ttu-id="b5cd7-230">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5cd7-230">DateTimeOffset</span></span>|<span data-ttu-id="b5cd7-p106">Время изменения контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b5cd7-p106">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b5cd7-234">manager</span><span class="sxs-lookup"><span data-stu-id="b5cd7-234">manager</span></span>|<span data-ttu-id="b5cd7-235">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-235">String</span></span>|<span data-ttu-id="b5cd7-236">Имя руководителя контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-236">The name of the contact's manager.</span></span>
|<span data-ttu-id="b5cd7-237">middleName</span><span class="sxs-lookup"><span data-stu-id="b5cd7-237">middleName</span></span>|<span data-ttu-id="b5cd7-238">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-238">String</span></span>|<span data-ttu-id="b5cd7-239">Отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-239">The contact's middle name.</span></span>|
|<span data-ttu-id="b5cd7-240">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="b5cd7-240">mobilePhone</span></span>|<span data-ttu-id="b5cd7-241">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-241">String</span></span>|<span data-ttu-id="b5cd7-242">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-242">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="b5cd7-243">nickName</span><span class="sxs-lookup"><span data-stu-id="b5cd7-243">nickName</span></span>|<span data-ttu-id="b5cd7-244">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-244">String</span></span>|<span data-ttu-id="b5cd7-245">Псевдоним контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-245">The contact's nickname.</span></span>|
|<span data-ttu-id="b5cd7-246">officeLocation</span><span class="sxs-lookup"><span data-stu-id="b5cd7-246">officeLocation</span></span>|<span data-ttu-id="b5cd7-247">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-247">String</span></span>|<span data-ttu-id="b5cd7-248">Расположение офиса контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-248">The location of the contact's office.</span></span>|
|<span data-ttu-id="b5cd7-249">otherAddress</span><span class="sxs-lookup"><span data-stu-id="b5cd7-249">otherAddress</span></span>|[<span data-ttu-id="b5cd7-250">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="b5cd7-250">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="b5cd7-251">Другие адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-251">Other addresses for the contact.</span></span>|
|<span data-ttu-id="b5cd7-252">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="b5cd7-252">parentFolderId</span></span>|<span data-ttu-id="b5cd7-253">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-253">String</span></span>|<span data-ttu-id="b5cd7-254">Идентификатор родительской папки контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-254">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="b5cd7-255">personalNotes</span><span class="sxs-lookup"><span data-stu-id="b5cd7-255">personalNotes</span></span>|<span data-ttu-id="b5cd7-256">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-256">String</span></span>|<span data-ttu-id="b5cd7-257">Заметки пользователя о контакте.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-257">The user's notes about the contact.</span></span>|
|<span data-ttu-id="b5cd7-258">profession</span><span class="sxs-lookup"><span data-stu-id="b5cd7-258">profession</span></span>|<span data-ttu-id="b5cd7-259">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-259">String</span></span>|<span data-ttu-id="b5cd7-260">Профессия контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-260">The contact's profession.</span></span>|
|<span data-ttu-id="b5cd7-261">spouseName</span><span class="sxs-lookup"><span data-stu-id="b5cd7-261">spouseName</span></span>|<span data-ttu-id="b5cd7-262">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-262">String</span></span>|<span data-ttu-id="b5cd7-263">Имя супруга или супруги контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-263">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="b5cd7-264">surname</span><span class="sxs-lookup"><span data-stu-id="b5cd7-264">surname</span></span>|<span data-ttu-id="b5cd7-265">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-265">String</span></span>|<span data-ttu-id="b5cd7-266">Фамилия контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-266">The contact's surname.</span></span>|
|<span data-ttu-id="b5cd7-267">title</span><span class="sxs-lookup"><span data-stu-id="b5cd7-267">title</span></span>|<span data-ttu-id="b5cd7-268">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-268">String</span></span>|<span data-ttu-id="b5cd7-269">Звание контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-269">The contact's title.</span></span>|
|<span data-ttu-id="b5cd7-270">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="b5cd7-270">yomiCompanyName</span></span>|<span data-ttu-id="b5cd7-271">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-271">String</span></span>|<span data-ttu-id="b5cd7-272">Название компании контакта, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-272">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="b5cd7-273">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="b5cd7-273">yomiGivenName</span></span>|<span data-ttu-id="b5cd7-274">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-274">String</span></span>|<span data-ttu-id="b5cd7-275">Имя контакта, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-275">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="b5cd7-276">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="b5cd7-276">yomiSurname</span></span>|<span data-ttu-id="b5cd7-277">Строка​</span><span class="sxs-lookup"><span data-stu-id="b5cd7-277">String</span></span>|<span data-ttu-id="b5cd7-278">Фамилия контакта, записанная так, как она звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-278">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5cd7-279">Отношения</span><span class="sxs-lookup"><span data-stu-id="b5cd7-279">Relationships</span></span>
| <span data-ttu-id="b5cd7-280">Связь</span><span class="sxs-lookup"><span data-stu-id="b5cd7-280">Relationship</span></span> | <span data-ttu-id="b5cd7-281">Тип</span><span class="sxs-lookup"><span data-stu-id="b5cd7-281">Type</span></span>   |<span data-ttu-id="b5cd7-282">Описание</span><span class="sxs-lookup"><span data-stu-id="b5cd7-282">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5cd7-283">extensions</span><span class="sxs-lookup"><span data-stu-id="b5cd7-283">extensions</span></span>|<span data-ttu-id="b5cd7-284">Коллекция [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="b5cd7-284">[extension](extension.md) collection</span></span>|<span data-ttu-id="b5cd7-p107">Коллекция открытых расширений, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-p107">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b5cd7-288">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b5cd7-288">multiValueExtendedProperties</span></span>|<span data-ttu-id="b5cd7-289">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="b5cd7-289">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="b5cd7-p108">Коллекция расширенных свойств с несколькими значениями, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-p108">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b5cd7-293">photo</span><span class="sxs-lookup"><span data-stu-id="b5cd7-293">photo</span></span>|[<span data-ttu-id="b5cd7-294">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="b5cd7-294">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="b5cd7-p109">Необязательное фото контакта. Можно получить или задать фото для контакта.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-p109">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="b5cd7-297">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b5cd7-297">singleValueExtendedProperties</span></span>|<span data-ttu-id="b5cd7-298">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="b5cd7-298">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="b5cd7-p110">Коллекция расширенных свойств с одним значением, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-p110">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5cd7-302">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5cd7-302">JSON representation</span></span>

<span data-ttu-id="b5cd7-303">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5cd7-303">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="b5cd7-304">См. также</span><span class="sxs-lookup"><span data-stu-id="b5cd7-304">See also</span></span>

- [<span data-ttu-id="b5cd7-305">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="b5cd7-305">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="b5cd7-306">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="b5cd7-306">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)
- [<span data-ttu-id="b5cd7-307">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="b5cd7-307">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="b5cd7-308">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="b5cd7-308">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="b5cd7-309">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="b5cd7-309">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
