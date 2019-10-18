---
title: Тип ресурса contact
description: Контакт — элемент в Outlook, в котором вы можете упорядочить и хранить сведения о людях и организациях, с которыми поддерживаете связь. Контакты содержатся в папках контактов.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ab0236f92075398f2131b40f14c45bfe215b6ea0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029661"
---
# <a name="contact-resource-type"></a><span data-ttu-id="725e5-104">Тип ресурса contact</span><span class="sxs-lookup"><span data-stu-id="725e5-104">contact resource type</span></span>

<span data-ttu-id="725e5-p102">Контакт — элемент в Outlook, в котором вы можете упорядочить и хранить сведения о людях и организациях, с которыми поддерживаете связь. Контакты содержатся в папках контактов.</span><span class="sxs-lookup"><span data-stu-id="725e5-p102">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="725e5-107">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="725e5-107">This resource supports:</span></span>

- <span data-ttu-id="725e5-108">добавление собственных данных к настраиваемым свойствам в виде [расширений](/graph/extensibility-overview);</span><span class="sxs-lookup"><span data-stu-id="725e5-108">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="725e5-109">подписку на [уведомления об изменениях](/graph/webhooks);</span><span class="sxs-lookup"><span data-stu-id="725e5-109">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="725e5-110">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/contact-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="725e5-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="725e5-111">Методы</span><span class="sxs-lookup"><span data-stu-id="725e5-111">Methods</span></span>

| <span data-ttu-id="725e5-112">Метод</span><span class="sxs-lookup"><span data-stu-id="725e5-112">Method</span></span>       | <span data-ttu-id="725e5-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="725e5-113">Return Type</span></span>  |<span data-ttu-id="725e5-114">Описание</span><span class="sxs-lookup"><span data-stu-id="725e5-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="725e5-115">Получение контакта</span><span class="sxs-lookup"><span data-stu-id="725e5-115">Get contact</span></span>](../api/contact-get.md) | [<span data-ttu-id="725e5-116">contact</span><span class="sxs-lookup"><span data-stu-id="725e5-116">contact</span></span>](contact.md) |<span data-ttu-id="725e5-117">Считывание свойств и отношений объекта contact.</span><span class="sxs-lookup"><span data-stu-id="725e5-117">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="725e5-118">Создание</span><span class="sxs-lookup"><span data-stu-id="725e5-118">Create</span></span>](../api/user-post-contacts.md) | [<span data-ttu-id="725e5-119">contact</span><span class="sxs-lookup"><span data-stu-id="725e5-119">contact</span></span>](contact.md) |<span data-ttu-id="725e5-120">Добавление контакта в корневую папку с контактами или конечную точку контактов другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="725e5-120">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="725e5-121">Обновление</span><span class="sxs-lookup"><span data-stu-id="725e5-121">Update</span></span>](../api/contact-update.md) | [<span data-ttu-id="725e5-122">contact</span><span class="sxs-lookup"><span data-stu-id="725e5-122">contact</span></span>](contact.md) |<span data-ttu-id="725e5-123">Обновление объекта contact.</span><span class="sxs-lookup"><span data-stu-id="725e5-123">Update contact object.</span></span> |
|[<span data-ttu-id="725e5-124">Удаление</span><span class="sxs-lookup"><span data-stu-id="725e5-124">Delete</span></span>](../api/contact-delete.md) | <span data-ttu-id="725e5-125">Нет</span><span class="sxs-lookup"><span data-stu-id="725e5-125">None</span></span> |<span data-ttu-id="725e5-126">Удаление объекта contact.</span><span class="sxs-lookup"><span data-stu-id="725e5-126">Delete contact object.</span></span> |
|[<span data-ttu-id="725e5-127">delta</span><span class="sxs-lookup"><span data-stu-id="725e5-127">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="725e5-128">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="725e5-128">[contact](contact.md) collection</span></span>| <span data-ttu-id="725e5-129">Получение набора контактов, которые были добавлены в указанную папку, обновлены в ней или удалены из нее.</span><span class="sxs-lookup"><span data-stu-id="725e5-129">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="725e5-130">**Открытые расширения**</span><span class="sxs-lookup"><span data-stu-id="725e5-130">**Open extensions**</span></span>| | |
|[<span data-ttu-id="725e5-131">Создание открытого расширения</span><span class="sxs-lookup"><span data-stu-id="725e5-131">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="725e5-132">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="725e5-132">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="725e5-133">Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.</span><span class="sxs-lookup"><span data-stu-id="725e5-133">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="725e5-134">Получение открытого расширения</span><span class="sxs-lookup"><span data-stu-id="725e5-134">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="725e5-135">Коллекция [openTypeExtension](opentypeextension.md)</span><span class="sxs-lookup"><span data-stu-id="725e5-135">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="725e5-136">Получение объектов открытого расширения, которые определяются по имени или полному имени.</span><span class="sxs-lookup"><span data-stu-id="725e5-136">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="725e5-137">**Расширения схемы**</span><span class="sxs-lookup"><span data-stu-id="725e5-137">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="725e5-138">Добавление значений расширений для схемы</span><span class="sxs-lookup"><span data-stu-id="725e5-138">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="725e5-139">Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.</span><span class="sxs-lookup"><span data-stu-id="725e5-139">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="725e5-140">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="725e5-140">**Extended properties**</span></span>| | |
|[<span data-ttu-id="725e5-141">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="725e5-141">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="725e5-142">contact</span><span class="sxs-lookup"><span data-stu-id="725e5-142">contact</span></span>](contact.md)  |<span data-ttu-id="725e5-143">Создание одного или нескольких расширенных свойств с одним значением в новом или существующем контакте.</span><span class="sxs-lookup"><span data-stu-id="725e5-143">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="725e5-144">Получение контакта с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="725e5-144">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="725e5-145">contact</span><span class="sxs-lookup"><span data-stu-id="725e5-145">contact</span></span>](contact.md) | <span data-ttu-id="725e5-146">Получение контактов, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="725e5-146">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="725e5-147">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="725e5-147">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="725e5-148">contact</span><span class="sxs-lookup"><span data-stu-id="725e5-148">contact</span></span>](contact.md) | <span data-ttu-id="725e5-149">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем контакте.</span><span class="sxs-lookup"><span data-stu-id="725e5-149">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="725e5-150">Получение контакта с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="725e5-150">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="725e5-151">contact</span><span class="sxs-lookup"><span data-stu-id="725e5-151">contact</span></span>](contact.md) | <span data-ttu-id="725e5-152">Получение контакта, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`.</span><span class="sxs-lookup"><span data-stu-id="725e5-152">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="725e5-153">Свойства</span><span class="sxs-lookup"><span data-stu-id="725e5-153">Properties</span></span>
| <span data-ttu-id="725e5-154">Свойство</span><span class="sxs-lookup"><span data-stu-id="725e5-154">Property</span></span>     | <span data-ttu-id="725e5-155">Тип</span><span class="sxs-lookup"><span data-stu-id="725e5-155">Type</span></span>   |<span data-ttu-id="725e5-156">Описание</span><span class="sxs-lookup"><span data-stu-id="725e5-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="725e5-157">assistantName</span><span class="sxs-lookup"><span data-stu-id="725e5-157">assistantName</span></span>|<span data-ttu-id="725e5-158">String</span><span class="sxs-lookup"><span data-stu-id="725e5-158">String</span></span>|<span data-ttu-id="725e5-159">Имя помощника контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-159">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="725e5-160">birthday</span><span class="sxs-lookup"><span data-stu-id="725e5-160">birthday</span></span>|<span data-ttu-id="725e5-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="725e5-161">DateTimeOffset</span></span>|<span data-ttu-id="725e5-p103">Дата рождения контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="725e5-p103">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="725e5-165">businessAddress</span><span class="sxs-lookup"><span data-stu-id="725e5-165">businessAddress</span></span>|[<span data-ttu-id="725e5-166">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="725e5-166">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="725e5-167">Рабочий адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-167">The contact's business address.</span></span>|
|<span data-ttu-id="725e5-168">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="725e5-168">businessHomePage</span></span>|<span data-ttu-id="725e5-169">String</span><span class="sxs-lookup"><span data-stu-id="725e5-169">String</span></span>|<span data-ttu-id="725e5-170">Домашняя страница контакта (рабочая).</span><span class="sxs-lookup"><span data-stu-id="725e5-170">The business home page of the contact.</span></span>|
|<span data-ttu-id="725e5-171">businessPhones</span><span class="sxs-lookup"><span data-stu-id="725e5-171">businessPhones</span></span>|<span data-ttu-id="725e5-172">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="725e5-172">String collection</span></span>|<span data-ttu-id="725e5-173">Рабочие номера телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-173">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="725e5-174">categories</span><span class="sxs-lookup"><span data-stu-id="725e5-174">categories</span></span>|<span data-ttu-id="725e5-175">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="725e5-175">String collection</span></span>|<span data-ttu-id="725e5-176">Категории, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="725e5-176">The categories associated with the contact.</span></span>|
|<span data-ttu-id="725e5-177">changeKey</span><span class="sxs-lookup"><span data-stu-id="725e5-177">changeKey</span></span>|<span data-ttu-id="725e5-178">Строка</span><span class="sxs-lookup"><span data-stu-id="725e5-178">String</span></span>|<span data-ttu-id="725e5-p104">Указывает версию контакта. При каждом изменении контакта также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="725e5-p104">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="725e5-182">children</span><span class="sxs-lookup"><span data-stu-id="725e5-182">children</span></span>|<span data-ttu-id="725e5-183">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="725e5-183">String collection</span></span>|<span data-ttu-id="725e5-184">Имена детей контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-184">The names of the contact's children.</span></span>|
|<span data-ttu-id="725e5-185">companyName</span><span class="sxs-lookup"><span data-stu-id="725e5-185">companyName</span></span>|<span data-ttu-id="725e5-186">String</span><span class="sxs-lookup"><span data-stu-id="725e5-186">String</span></span>|<span data-ttu-id="725e5-187">Название компании контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-187">The name of the contact's company.</span></span>|
|<span data-ttu-id="725e5-188">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="725e5-188">createdDateTime</span></span>|<span data-ttu-id="725e5-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="725e5-189">DateTimeOffset</span></span>|<span data-ttu-id="725e5-p105">Время создания контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="725e5-p105">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="725e5-193">отделу;</span><span class="sxs-lookup"><span data-stu-id="725e5-193">department</span></span>|<span data-ttu-id="725e5-194">String</span><span class="sxs-lookup"><span data-stu-id="725e5-194">String</span></span>|<span data-ttu-id="725e5-195">Отдел контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-195">The contact's department.</span></span>|
|<span data-ttu-id="725e5-196">displayName</span><span class="sxs-lookup"><span data-stu-id="725e5-196">displayName</span></span>|<span data-ttu-id="725e5-197">String</span><span class="sxs-lookup"><span data-stu-id="725e5-197">String</span></span>|<span data-ttu-id="725e5-198">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-198">The contact's display name.</span></span> <span data-ttu-id="725e5-199">Отображаемое имя можно указать в операции [создания](../api/user-post-contacts.md) или [обновления](../api/contact-update.md).</span><span class="sxs-lookup"><span data-stu-id="725e5-199">You can specify the display name in a [create](../api/user-post-contacts.md) or [update](../api/contact-update.md) operation.</span></span> <span data-ttu-id="725e5-200">Обратите внимание, что последующие обновления других свойств могут привести к тому, что автоматически созданное значение перезапишет указанное значение displayName.</span><span class="sxs-lookup"><span data-stu-id="725e5-200">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="725e5-201">Чтобы сохранить существующее значение, всегда добавляйте его как displayName в операцию [обновления](../api/contact-update.md).</span><span class="sxs-lookup"><span data-stu-id="725e5-201">To preserve a pre-existing value, always include it as displayName in an [update](../api/contact-update.md) operation.</span></span>|
|<span data-ttu-id="725e5-202">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="725e5-202">emailAddresses</span></span>|<span data-ttu-id="725e5-203">Коллекция [EmailAddress](emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="725e5-203">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="725e5-204">Электронные адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-204">The contact's email addresses.</span></span>|
|<span data-ttu-id="725e5-205">fileAs</span><span class="sxs-lookup"><span data-stu-id="725e5-205">fileAs</span></span>|<span data-ttu-id="725e5-206">String</span><span class="sxs-lookup"><span data-stu-id="725e5-206">String</span></span>|<span data-ttu-id="725e5-207">Имя, под которым хранится контакт.</span><span class="sxs-lookup"><span data-stu-id="725e5-207">The name the contact is filed under.</span></span>|
|<span data-ttu-id="725e5-208">generation</span><span class="sxs-lookup"><span data-stu-id="725e5-208">generation</span></span>|<span data-ttu-id="725e5-209">String</span><span class="sxs-lookup"><span data-stu-id="725e5-209">String</span></span>|<span data-ttu-id="725e5-210">Поколение контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-210">The contact's generation.</span></span>|
|<span data-ttu-id="725e5-211">givenName</span><span class="sxs-lookup"><span data-stu-id="725e5-211">givenName</span></span>|<span data-ttu-id="725e5-212">String</span><span class="sxs-lookup"><span data-stu-id="725e5-212">String</span></span>|<span data-ttu-id="725e5-213">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-213">The contact's given name.</span></span>|
|<span data-ttu-id="725e5-214">homeAddress</span><span class="sxs-lookup"><span data-stu-id="725e5-214">homeAddress</span></span>|[<span data-ttu-id="725e5-215">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="725e5-215">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="725e5-216">Домашний адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-216">The contact's home address.</span></span>|
|<span data-ttu-id="725e5-217">homePhones</span><span class="sxs-lookup"><span data-stu-id="725e5-217">homePhones</span></span>|<span data-ttu-id="725e5-218">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="725e5-218">String collection</span></span>|<span data-ttu-id="725e5-219">Номера домашних телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-219">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="725e5-220">id</span><span class="sxs-lookup"><span data-stu-id="725e5-220">id</span></span>|<span data-ttu-id="725e5-221">String</span><span class="sxs-lookup"><span data-stu-id="725e5-221">String</span></span>|<span data-ttu-id="725e5-p107">Уникальный идентификатор контакта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="725e5-p107">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="725e5-224">imAddresses</span><span class="sxs-lookup"><span data-stu-id="725e5-224">imAddresses</span></span>|<span data-ttu-id="725e5-225">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="725e5-225">String collection</span></span>|<span data-ttu-id="725e5-226">Адреса контакта для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="725e5-226">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="725e5-227">initials</span><span class="sxs-lookup"><span data-stu-id="725e5-227">initials</span></span>|<span data-ttu-id="725e5-228">String</span><span class="sxs-lookup"><span data-stu-id="725e5-228">String</span></span>|<span data-ttu-id="725e5-229">Инициалы контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-229">The contact's initials.</span></span>|
|<span data-ttu-id="725e5-230">jobTitle</span><span class="sxs-lookup"><span data-stu-id="725e5-230">jobTitle</span></span>|<span data-ttu-id="725e5-231">String</span><span class="sxs-lookup"><span data-stu-id="725e5-231">String</span></span>|<span data-ttu-id="725e5-232">Должность контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-232">The contact’s job title.</span></span>|
|<span data-ttu-id="725e5-233">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="725e5-233">lastModifiedDateTime</span></span>|<span data-ttu-id="725e5-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="725e5-234">DateTimeOffset</span></span>|<span data-ttu-id="725e5-p108">Время изменения контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="725e5-p108">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="725e5-238">manager</span><span class="sxs-lookup"><span data-stu-id="725e5-238">manager</span></span>|<span data-ttu-id="725e5-239">String</span><span class="sxs-lookup"><span data-stu-id="725e5-239">String</span></span>|<span data-ttu-id="725e5-240">Имя руководителя контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-240">The name of the contact's manager.</span></span>
|<span data-ttu-id="725e5-241">middleName</span><span class="sxs-lookup"><span data-stu-id="725e5-241">middleName</span></span>|<span data-ttu-id="725e5-242">String</span><span class="sxs-lookup"><span data-stu-id="725e5-242">String</span></span>|<span data-ttu-id="725e5-243">Отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-243">The contact's middle name.</span></span>|
|<span data-ttu-id="725e5-244">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="725e5-244">mobilePhone</span></span>|<span data-ttu-id="725e5-245">String</span><span class="sxs-lookup"><span data-stu-id="725e5-245">String</span></span>|<span data-ttu-id="725e5-246">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-246">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="725e5-247">nickName</span><span class="sxs-lookup"><span data-stu-id="725e5-247">nickName</span></span>|<span data-ttu-id="725e5-248">String</span><span class="sxs-lookup"><span data-stu-id="725e5-248">String</span></span>|<span data-ttu-id="725e5-249">Псевдоним контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-249">The contact's nickname.</span></span>|
|<span data-ttu-id="725e5-250">officeLocation</span><span class="sxs-lookup"><span data-stu-id="725e5-250">officeLocation</span></span>|<span data-ttu-id="725e5-251">String</span><span class="sxs-lookup"><span data-stu-id="725e5-251">String</span></span>|<span data-ttu-id="725e5-252">Расположение офиса контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-252">The location of the contact's office.</span></span>|
|<span data-ttu-id="725e5-253">otherAddress</span><span class="sxs-lookup"><span data-stu-id="725e5-253">otherAddress</span></span>|[<span data-ttu-id="725e5-254">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="725e5-254">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="725e5-255">Другие адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-255">Other addresses for the contact.</span></span>|
|<span data-ttu-id="725e5-256">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="725e5-256">parentFolderId</span></span>|<span data-ttu-id="725e5-257">String</span><span class="sxs-lookup"><span data-stu-id="725e5-257">String</span></span>|<span data-ttu-id="725e5-258">Идентификатор родительской папки контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-258">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="725e5-259">personalNotes</span><span class="sxs-lookup"><span data-stu-id="725e5-259">personalNotes</span></span>|<span data-ttu-id="725e5-260">String</span><span class="sxs-lookup"><span data-stu-id="725e5-260">String</span></span>|<span data-ttu-id="725e5-261">Заметки пользователя о контакте.</span><span class="sxs-lookup"><span data-stu-id="725e5-261">The user's notes about the contact.</span></span>|
|<span data-ttu-id="725e5-262">profession</span><span class="sxs-lookup"><span data-stu-id="725e5-262">profession</span></span>|<span data-ttu-id="725e5-263">String</span><span class="sxs-lookup"><span data-stu-id="725e5-263">String</span></span>|<span data-ttu-id="725e5-264">Профессия контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-264">The contact's profession.</span></span>|
|<span data-ttu-id="725e5-265">spouseName</span><span class="sxs-lookup"><span data-stu-id="725e5-265">spouseName</span></span>|<span data-ttu-id="725e5-266">String</span><span class="sxs-lookup"><span data-stu-id="725e5-266">String</span></span>|<span data-ttu-id="725e5-267">Имя супруга или супруги контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-267">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="725e5-268">surname</span><span class="sxs-lookup"><span data-stu-id="725e5-268">surname</span></span>|<span data-ttu-id="725e5-269">String</span><span class="sxs-lookup"><span data-stu-id="725e5-269">String</span></span>|<span data-ttu-id="725e5-270">Фамилия контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-270">The contact's surname.</span></span>|
|<span data-ttu-id="725e5-271">title</span><span class="sxs-lookup"><span data-stu-id="725e5-271">title</span></span>|<span data-ttu-id="725e5-272">String</span><span class="sxs-lookup"><span data-stu-id="725e5-272">String</span></span>|<span data-ttu-id="725e5-273">Звание контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-273">The contact's title.</span></span>|
|<span data-ttu-id="725e5-274">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="725e5-274">yomiCompanyName</span></span>|<span data-ttu-id="725e5-275">String</span><span class="sxs-lookup"><span data-stu-id="725e5-275">String</span></span>|<span data-ttu-id="725e5-276">Название компании контакта, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="725e5-276">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="725e5-277">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="725e5-277">yomiGivenName</span></span>|<span data-ttu-id="725e5-278">String</span><span class="sxs-lookup"><span data-stu-id="725e5-278">String</span></span>|<span data-ttu-id="725e5-279">Имя контакта, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="725e5-279">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="725e5-280">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="725e5-280">yomiSurname</span></span>|<span data-ttu-id="725e5-281">String</span><span class="sxs-lookup"><span data-stu-id="725e5-281">String</span></span>|<span data-ttu-id="725e5-282">Фамилия контакта, записанная так, как она звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="725e5-282">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="725e5-283">Отношения</span><span class="sxs-lookup"><span data-stu-id="725e5-283">Relationships</span></span>
| <span data-ttu-id="725e5-284">Отношение</span><span class="sxs-lookup"><span data-stu-id="725e5-284">Relationship</span></span> | <span data-ttu-id="725e5-285">Тип</span><span class="sxs-lookup"><span data-stu-id="725e5-285">Type</span></span>   |<span data-ttu-id="725e5-286">Описание</span><span class="sxs-lookup"><span data-stu-id="725e5-286">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="725e5-287">extensions</span><span class="sxs-lookup"><span data-stu-id="725e5-287">extensions</span></span>|<span data-ttu-id="725e5-288">Коллекция [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="725e5-288">[extension](extension.md) collection</span></span>|<span data-ttu-id="725e5-p109">Коллекция открытых расширений, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="725e5-p109">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="725e5-292">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="725e5-292">multiValueExtendedProperties</span></span>|<span data-ttu-id="725e5-293">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="725e5-293">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="725e5-p110">Коллекция расширенных свойств с несколькими значениями, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="725e5-p110">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="725e5-297">Фотография
</span><span class="sxs-lookup"><span data-stu-id="725e5-297">photo</span></span>|[<span data-ttu-id="725e5-298">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="725e5-298">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="725e5-p111">Необязательное фото контакта. Можно получить или задать фото для контакта.</span><span class="sxs-lookup"><span data-stu-id="725e5-p111">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="725e5-301">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="725e5-301">singleValueExtendedProperties</span></span>|<span data-ttu-id="725e5-302">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="725e5-302">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="725e5-p112">Коллекция расширенных свойств с одним значением, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="725e5-p112">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="725e5-306">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="725e5-306">JSON representation</span></span>

<span data-ttu-id="725e5-307">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="725e5-307">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="725e5-308">См. также</span><span class="sxs-lookup"><span data-stu-id="725e5-308">See also</span></span>

- [<span data-ttu-id="725e5-309">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="725e5-309">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="725e5-310">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="725e5-310">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)
- [<span data-ttu-id="725e5-311">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="725e5-311">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="725e5-312">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="725e5-312">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="725e5-313">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="725e5-313">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
