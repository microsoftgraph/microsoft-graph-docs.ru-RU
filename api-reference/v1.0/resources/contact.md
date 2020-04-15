---
title: Тип ресурса contact
description: Контакт — элемент в Outlook, в котором вы можете упорядочить и хранить сведения о людях и организациях, с которыми поддерживаете связь. Контакты содержатся в папках контактов.
author: kevinbellinger
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0dc276aa7c4b1e996f9c36cf5dcbf587964cc4d7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449488"
---
# <a name="contact-resource-type"></a><span data-ttu-id="9c592-104">Тип ресурса contact</span><span class="sxs-lookup"><span data-stu-id="9c592-104">contact resource type</span></span>

<span data-ttu-id="9c592-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c592-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c592-p102">Контакт — элемент в Outlook, в котором вы можете упорядочить и хранить сведения о людях и организациях, с которыми поддерживаете связь. Контакты содержатся в папках контактов.</span><span class="sxs-lookup"><span data-stu-id="9c592-p102">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="9c592-108">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="9c592-108">This resource supports:</span></span>

- <span data-ttu-id="9c592-109">добавление собственных данных к настраиваемым свойствам в виде [расширений](/graph/extensibility-overview);</span><span class="sxs-lookup"><span data-stu-id="9c592-109">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="9c592-110">подписку на [уведомления об изменениях](/graph/webhooks);</span><span class="sxs-lookup"><span data-stu-id="9c592-110">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="9c592-111">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/contact-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="9c592-111">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="9c592-112">Методы</span><span class="sxs-lookup"><span data-stu-id="9c592-112">Methods</span></span>

| <span data-ttu-id="9c592-113">Метод</span><span class="sxs-lookup"><span data-stu-id="9c592-113">Method</span></span>       | <span data-ttu-id="9c592-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9c592-114">Return Type</span></span>  |<span data-ttu-id="9c592-115">Описание</span><span class="sxs-lookup"><span data-stu-id="9c592-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c592-116">Получение контакта</span><span class="sxs-lookup"><span data-stu-id="9c592-116">Get contact</span></span>](../api/contact-get.md) | [<span data-ttu-id="9c592-117">contact</span><span class="sxs-lookup"><span data-stu-id="9c592-117">contact</span></span>](contact.md) |<span data-ttu-id="9c592-118">Считывание свойств и отношений объекта contact.</span><span class="sxs-lookup"><span data-stu-id="9c592-118">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="9c592-119">Создание</span><span class="sxs-lookup"><span data-stu-id="9c592-119">Create</span></span>](../api/user-post-contacts.md) | [<span data-ttu-id="9c592-120">contact</span><span class="sxs-lookup"><span data-stu-id="9c592-120">contact</span></span>](contact.md) |<span data-ttu-id="9c592-121">Добавление контакта в корневую папку с контактами или конечную точку контактов другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="9c592-121">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="9c592-122">Обновление</span><span class="sxs-lookup"><span data-stu-id="9c592-122">Update</span></span>](../api/contact-update.md) | [<span data-ttu-id="9c592-123">contact</span><span class="sxs-lookup"><span data-stu-id="9c592-123">contact</span></span>](contact.md) |<span data-ttu-id="9c592-124">Обновление объекта contact.</span><span class="sxs-lookup"><span data-stu-id="9c592-124">Update contact object.</span></span> |
|[<span data-ttu-id="9c592-125">Удаление</span><span class="sxs-lookup"><span data-stu-id="9c592-125">Delete</span></span>](../api/contact-delete.md) | <span data-ttu-id="9c592-126">Нет</span><span class="sxs-lookup"><span data-stu-id="9c592-126">None</span></span> |<span data-ttu-id="9c592-127">Удаление объекта contact.</span><span class="sxs-lookup"><span data-stu-id="9c592-127">Delete contact object.</span></span> |
|[<span data-ttu-id="9c592-128">delta</span><span class="sxs-lookup"><span data-stu-id="9c592-128">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="9c592-129">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="9c592-129">[contact](contact.md) collection</span></span>| <span data-ttu-id="9c592-130">Получение набора контактов, которые были добавлены в указанную папку, обновлены в ней или удалены из нее.</span><span class="sxs-lookup"><span data-stu-id="9c592-130">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="9c592-131">**Открытые расширения**</span><span class="sxs-lookup"><span data-stu-id="9c592-131">**Open extensions**</span></span>| | |
|[<span data-ttu-id="9c592-132">Создание открытого расширения</span><span class="sxs-lookup"><span data-stu-id="9c592-132">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="9c592-133">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="9c592-133">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="9c592-134">Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.</span><span class="sxs-lookup"><span data-stu-id="9c592-134">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="9c592-135">Получение открытого расширения</span><span class="sxs-lookup"><span data-stu-id="9c592-135">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="9c592-136">Коллекция [openTypeExtension](opentypeextension.md)</span><span class="sxs-lookup"><span data-stu-id="9c592-136">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="9c592-137">Получение объектов открытого расширения, которые определяются по имени или полному имени.</span><span class="sxs-lookup"><span data-stu-id="9c592-137">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="9c592-138">**Расширения схемы**</span><span class="sxs-lookup"><span data-stu-id="9c592-138">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="9c592-139">Добавление значений расширений для схемы</span><span class="sxs-lookup"><span data-stu-id="9c592-139">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="9c592-140">Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.</span><span class="sxs-lookup"><span data-stu-id="9c592-140">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="9c592-141">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="9c592-141">**Extended properties**</span></span>| | |
|[<span data-ttu-id="9c592-142">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="9c592-142">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="9c592-143">contact</span><span class="sxs-lookup"><span data-stu-id="9c592-143">contact</span></span>](contact.md)  |<span data-ttu-id="9c592-144">Создание одного или нескольких расширенных свойств с одним значением в новом или существующем контакте.</span><span class="sxs-lookup"><span data-stu-id="9c592-144">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="9c592-145">Получение контакта с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="9c592-145">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="9c592-146">contact</span><span class="sxs-lookup"><span data-stu-id="9c592-146">contact</span></span>](contact.md) | <span data-ttu-id="9c592-147">Получение контактов, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="9c592-147">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="9c592-148">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="9c592-148">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="9c592-149">contact</span><span class="sxs-lookup"><span data-stu-id="9c592-149">contact</span></span>](contact.md) | <span data-ttu-id="9c592-150">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем контакте.</span><span class="sxs-lookup"><span data-stu-id="9c592-150">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="9c592-151">Получение контакта с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="9c592-151">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="9c592-152">contact</span><span class="sxs-lookup"><span data-stu-id="9c592-152">contact</span></span>](contact.md) | <span data-ttu-id="9c592-153">Получение контакта, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`.</span><span class="sxs-lookup"><span data-stu-id="9c592-153">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="9c592-154">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c592-154">Properties</span></span>
| <span data-ttu-id="9c592-155">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c592-155">Property</span></span>     | <span data-ttu-id="9c592-156">Тип</span><span class="sxs-lookup"><span data-stu-id="9c592-156">Type</span></span>   |<span data-ttu-id="9c592-157">Описание</span><span class="sxs-lookup"><span data-stu-id="9c592-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c592-158">assistantName</span><span class="sxs-lookup"><span data-stu-id="9c592-158">assistantName</span></span>|<span data-ttu-id="9c592-159">String</span><span class="sxs-lookup"><span data-stu-id="9c592-159">String</span></span>|<span data-ttu-id="9c592-160">Имя помощника контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-160">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="9c592-161">birthday</span><span class="sxs-lookup"><span data-stu-id="9c592-161">birthday</span></span>|<span data-ttu-id="9c592-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c592-162">DateTimeOffset</span></span>|<span data-ttu-id="9c592-p103">Дата рождения контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9c592-p103">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9c592-166">businessAddress</span><span class="sxs-lookup"><span data-stu-id="9c592-166">businessAddress</span></span>|[<span data-ttu-id="9c592-167">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="9c592-167">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="9c592-168">Рабочий адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-168">The contact's business address.</span></span>|
|<span data-ttu-id="9c592-169">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="9c592-169">businessHomePage</span></span>|<span data-ttu-id="9c592-170">String</span><span class="sxs-lookup"><span data-stu-id="9c592-170">String</span></span>|<span data-ttu-id="9c592-171">Домашняя страница контакта (рабочая).</span><span class="sxs-lookup"><span data-stu-id="9c592-171">The business home page of the contact.</span></span>|
|<span data-ttu-id="9c592-172">businessPhones</span><span class="sxs-lookup"><span data-stu-id="9c592-172">businessPhones</span></span>|<span data-ttu-id="9c592-173">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9c592-173">String collection</span></span>|<span data-ttu-id="9c592-174">Рабочие номера телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-174">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="9c592-175">categories</span><span class="sxs-lookup"><span data-stu-id="9c592-175">categories</span></span>|<span data-ttu-id="9c592-176">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9c592-176">String collection</span></span>|<span data-ttu-id="9c592-177">Категории, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="9c592-177">The categories associated with the contact.</span></span>|
|<span data-ttu-id="9c592-178">changeKey</span><span class="sxs-lookup"><span data-stu-id="9c592-178">changeKey</span></span>|<span data-ttu-id="9c592-179">Строка</span><span class="sxs-lookup"><span data-stu-id="9c592-179">String</span></span>|<span data-ttu-id="9c592-p104">Указывает версию контакта. При каждом изменении контакта также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="9c592-p104">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="9c592-183">children</span><span class="sxs-lookup"><span data-stu-id="9c592-183">children</span></span>|<span data-ttu-id="9c592-184">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9c592-184">String collection</span></span>|<span data-ttu-id="9c592-185">Имена детей контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-185">The names of the contact's children.</span></span>|
|<span data-ttu-id="9c592-186">companyName</span><span class="sxs-lookup"><span data-stu-id="9c592-186">companyName</span></span>|<span data-ttu-id="9c592-187">String</span><span class="sxs-lookup"><span data-stu-id="9c592-187">String</span></span>|<span data-ttu-id="9c592-188">Название компании контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-188">The name of the contact's company.</span></span>|
|<span data-ttu-id="9c592-189">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9c592-189">createdDateTime</span></span>|<span data-ttu-id="9c592-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c592-190">DateTimeOffset</span></span>|<span data-ttu-id="9c592-p105">Время создания контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9c592-p105">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9c592-194">отделу;</span><span class="sxs-lookup"><span data-stu-id="9c592-194">department</span></span>|<span data-ttu-id="9c592-195">String</span><span class="sxs-lookup"><span data-stu-id="9c592-195">String</span></span>|<span data-ttu-id="9c592-196">Отдел контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-196">The contact's department.</span></span>|
|<span data-ttu-id="9c592-197">displayName</span><span class="sxs-lookup"><span data-stu-id="9c592-197">displayName</span></span>|<span data-ttu-id="9c592-198">String</span><span class="sxs-lookup"><span data-stu-id="9c592-198">String</span></span>|<span data-ttu-id="9c592-199">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-199">The contact's display name.</span></span> <span data-ttu-id="9c592-200">Отображаемое имя можно указать в операции [создания](../api/user-post-contacts.md) или [обновления](../api/contact-update.md).</span><span class="sxs-lookup"><span data-stu-id="9c592-200">You can specify the display name in a [create](../api/user-post-contacts.md) or [update](../api/contact-update.md) operation.</span></span> <span data-ttu-id="9c592-201">Обратите внимание, что последующие обновления других свойств могут привести к тому, что автоматически созданное значение перезапишет указанное значение displayName.</span><span class="sxs-lookup"><span data-stu-id="9c592-201">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="9c592-202">Чтобы сохранить существующее значение, всегда добавляйте его как displayName в операцию [обновления](../api/contact-update.md).</span><span class="sxs-lookup"><span data-stu-id="9c592-202">To preserve a pre-existing value, always include it as displayName in an [update](../api/contact-update.md) operation.</span></span>|
|<span data-ttu-id="9c592-203">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="9c592-203">emailAddresses</span></span>|<span data-ttu-id="9c592-204">Коллекция [EmailAddress](emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="9c592-204">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="9c592-205">Электронные адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-205">The contact's email addresses.</span></span>|
|<span data-ttu-id="9c592-206">fileAs</span><span class="sxs-lookup"><span data-stu-id="9c592-206">fileAs</span></span>|<span data-ttu-id="9c592-207">String</span><span class="sxs-lookup"><span data-stu-id="9c592-207">String</span></span>|<span data-ttu-id="9c592-208">Имя, под которым хранится контакт.</span><span class="sxs-lookup"><span data-stu-id="9c592-208">The name the contact is filed under.</span></span>|
|<span data-ttu-id="9c592-209">generation</span><span class="sxs-lookup"><span data-stu-id="9c592-209">generation</span></span>|<span data-ttu-id="9c592-210">String</span><span class="sxs-lookup"><span data-stu-id="9c592-210">String</span></span>|<span data-ttu-id="9c592-211">Поколение контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-211">The contact's generation.</span></span>|
|<span data-ttu-id="9c592-212">givenName</span><span class="sxs-lookup"><span data-stu-id="9c592-212">givenName</span></span>|<span data-ttu-id="9c592-213">String</span><span class="sxs-lookup"><span data-stu-id="9c592-213">String</span></span>|<span data-ttu-id="9c592-214">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-214">The contact's given name.</span></span>|
|<span data-ttu-id="9c592-215">homeAddress</span><span class="sxs-lookup"><span data-stu-id="9c592-215">homeAddress</span></span>|[<span data-ttu-id="9c592-216">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="9c592-216">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="9c592-217">Домашний адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-217">The contact's home address.</span></span>|
|<span data-ttu-id="9c592-218">homePhones</span><span class="sxs-lookup"><span data-stu-id="9c592-218">homePhones</span></span>|<span data-ttu-id="9c592-219">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9c592-219">String collection</span></span>|<span data-ttu-id="9c592-220">Номера домашних телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-220">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="9c592-221">id</span><span class="sxs-lookup"><span data-stu-id="9c592-221">id</span></span>|<span data-ttu-id="9c592-222">String</span><span class="sxs-lookup"><span data-stu-id="9c592-222">String</span></span>|<span data-ttu-id="9c592-p107">Уникальный идентификатор контакта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9c592-p107">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="9c592-225">imAddresses</span><span class="sxs-lookup"><span data-stu-id="9c592-225">imAddresses</span></span>|<span data-ttu-id="9c592-226">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9c592-226">String collection</span></span>|<span data-ttu-id="9c592-227">Адреса контакта для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="9c592-227">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="9c592-228">initials</span><span class="sxs-lookup"><span data-stu-id="9c592-228">initials</span></span>|<span data-ttu-id="9c592-229">String</span><span class="sxs-lookup"><span data-stu-id="9c592-229">String</span></span>|<span data-ttu-id="9c592-230">Инициалы контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-230">The contact's initials.</span></span>|
|<span data-ttu-id="9c592-231">jobTitle</span><span class="sxs-lookup"><span data-stu-id="9c592-231">jobTitle</span></span>|<span data-ttu-id="9c592-232">String</span><span class="sxs-lookup"><span data-stu-id="9c592-232">String</span></span>|<span data-ttu-id="9c592-233">Должность контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-233">The contact’s job title.</span></span>|
|<span data-ttu-id="9c592-234">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c592-234">lastModifiedDateTime</span></span>|<span data-ttu-id="9c592-235">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c592-235">DateTimeOffset</span></span>|<span data-ttu-id="9c592-p108">Время изменения контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9c592-p108">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9c592-239">manager</span><span class="sxs-lookup"><span data-stu-id="9c592-239">manager</span></span>|<span data-ttu-id="9c592-240">String</span><span class="sxs-lookup"><span data-stu-id="9c592-240">String</span></span>|<span data-ttu-id="9c592-241">Имя руководителя контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-241">The name of the contact's manager.</span></span>
|<span data-ttu-id="9c592-242">middleName</span><span class="sxs-lookup"><span data-stu-id="9c592-242">middleName</span></span>|<span data-ttu-id="9c592-243">String</span><span class="sxs-lookup"><span data-stu-id="9c592-243">String</span></span>|<span data-ttu-id="9c592-244">Отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-244">The contact's middle name.</span></span>|
|<span data-ttu-id="9c592-245">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="9c592-245">mobilePhone</span></span>|<span data-ttu-id="9c592-246">String</span><span class="sxs-lookup"><span data-stu-id="9c592-246">String</span></span>|<span data-ttu-id="9c592-247">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-247">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="9c592-248">nickName</span><span class="sxs-lookup"><span data-stu-id="9c592-248">nickName</span></span>|<span data-ttu-id="9c592-249">String</span><span class="sxs-lookup"><span data-stu-id="9c592-249">String</span></span>|<span data-ttu-id="9c592-250">Псевдоним контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-250">The contact's nickname.</span></span>|
|<span data-ttu-id="9c592-251">officeLocation</span><span class="sxs-lookup"><span data-stu-id="9c592-251">officeLocation</span></span>|<span data-ttu-id="9c592-252">String</span><span class="sxs-lookup"><span data-stu-id="9c592-252">String</span></span>|<span data-ttu-id="9c592-253">Расположение офиса контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-253">The location of the contact's office.</span></span>|
|<span data-ttu-id="9c592-254">otherAddress</span><span class="sxs-lookup"><span data-stu-id="9c592-254">otherAddress</span></span>|[<span data-ttu-id="9c592-255">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="9c592-255">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="9c592-256">Другие адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-256">Other addresses for the contact.</span></span>|
|<span data-ttu-id="9c592-257">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="9c592-257">parentFolderId</span></span>|<span data-ttu-id="9c592-258">String</span><span class="sxs-lookup"><span data-stu-id="9c592-258">String</span></span>|<span data-ttu-id="9c592-259">Идентификатор родительской папки контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-259">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="9c592-260">personalNotes</span><span class="sxs-lookup"><span data-stu-id="9c592-260">personalNotes</span></span>|<span data-ttu-id="9c592-261">String</span><span class="sxs-lookup"><span data-stu-id="9c592-261">String</span></span>|<span data-ttu-id="9c592-262">Заметки пользователя о контакте.</span><span class="sxs-lookup"><span data-stu-id="9c592-262">The user's notes about the contact.</span></span>|
|<span data-ttu-id="9c592-263">profession</span><span class="sxs-lookup"><span data-stu-id="9c592-263">profession</span></span>|<span data-ttu-id="9c592-264">String</span><span class="sxs-lookup"><span data-stu-id="9c592-264">String</span></span>|<span data-ttu-id="9c592-265">Профессия контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-265">The contact's profession.</span></span>|
|<span data-ttu-id="9c592-266">spouseName</span><span class="sxs-lookup"><span data-stu-id="9c592-266">spouseName</span></span>|<span data-ttu-id="9c592-267">String</span><span class="sxs-lookup"><span data-stu-id="9c592-267">String</span></span>|<span data-ttu-id="9c592-268">Имя супруга или супруги контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-268">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="9c592-269">surname</span><span class="sxs-lookup"><span data-stu-id="9c592-269">surname</span></span>|<span data-ttu-id="9c592-270">String</span><span class="sxs-lookup"><span data-stu-id="9c592-270">String</span></span>|<span data-ttu-id="9c592-271">Фамилия контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-271">The contact's surname.</span></span>|
|<span data-ttu-id="9c592-272">title</span><span class="sxs-lookup"><span data-stu-id="9c592-272">title</span></span>|<span data-ttu-id="9c592-273">String</span><span class="sxs-lookup"><span data-stu-id="9c592-273">String</span></span>|<span data-ttu-id="9c592-274">Звание контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-274">The contact's title.</span></span>|
|<span data-ttu-id="9c592-275">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="9c592-275">yomiCompanyName</span></span>|<span data-ttu-id="9c592-276">String</span><span class="sxs-lookup"><span data-stu-id="9c592-276">String</span></span>|<span data-ttu-id="9c592-277">Название компании контакта, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="9c592-277">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="9c592-278">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="9c592-278">yomiGivenName</span></span>|<span data-ttu-id="9c592-279">String</span><span class="sxs-lookup"><span data-stu-id="9c592-279">String</span></span>|<span data-ttu-id="9c592-280">Имя контакта, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="9c592-280">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="9c592-281">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="9c592-281">yomiSurname</span></span>|<span data-ttu-id="9c592-282">String</span><span class="sxs-lookup"><span data-stu-id="9c592-282">String</span></span>|<span data-ttu-id="9c592-283">Фамилия контакта, записанная так, как она звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="9c592-283">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c592-284">Отношения</span><span class="sxs-lookup"><span data-stu-id="9c592-284">Relationships</span></span>
| <span data-ttu-id="9c592-285">Связь</span><span class="sxs-lookup"><span data-stu-id="9c592-285">Relationship</span></span> | <span data-ttu-id="9c592-286">Тип</span><span class="sxs-lookup"><span data-stu-id="9c592-286">Type</span></span>   |<span data-ttu-id="9c592-287">Описание</span><span class="sxs-lookup"><span data-stu-id="9c592-287">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c592-288">extensions</span><span class="sxs-lookup"><span data-stu-id="9c592-288">extensions</span></span>|<span data-ttu-id="9c592-289">Коллекция [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="9c592-289">[extension](extension.md) collection</span></span>|<span data-ttu-id="9c592-p109">Коллекция открытых расширений, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9c592-p109">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="9c592-293">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="9c592-293">multiValueExtendedProperties</span></span>|<span data-ttu-id="9c592-294">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="9c592-294">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="9c592-p110">Коллекция расширенных свойств с несколькими значениями, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9c592-p110">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="9c592-298">Фотография
</span><span class="sxs-lookup"><span data-stu-id="9c592-298">photo</span></span>|[<span data-ttu-id="9c592-299">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="9c592-299">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="9c592-p111">Необязательное фото контакта. Можно получить или задать фото для контакта.</span><span class="sxs-lookup"><span data-stu-id="9c592-p111">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="9c592-302">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="9c592-302">singleValueExtendedProperties</span></span>|<span data-ttu-id="9c592-303">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="9c592-303">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="9c592-p112">Коллекция расширенных свойств с одним значением, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9c592-p112">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c592-307">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9c592-307">JSON representation</span></span>

<span data-ttu-id="9c592-308">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c592-308">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="9c592-309">См. также</span><span class="sxs-lookup"><span data-stu-id="9c592-309">See also</span></span>

- [<span data-ttu-id="9c592-310">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="9c592-310">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="9c592-311">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="9c592-311">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)
- [<span data-ttu-id="9c592-312">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="9c592-312">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9c592-313">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="9c592-313">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="9c592-314">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="9c592-314">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
