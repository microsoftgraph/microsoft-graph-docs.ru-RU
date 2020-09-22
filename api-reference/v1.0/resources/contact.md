---
title: Тип ресурса contact
description: Контакт — элемент в Outlook, в котором вы можете упорядочить и хранить сведения о людях и организациях, с которыми поддерживаете связь. Контакты содержатся в папках контактов.
author: kevinbellinger
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1815f00f4f402433c6854b32d1f4734c95a372de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056991"
---
# <a name="contact-resource-type"></a><span data-ttu-id="4c992-104">Тип ресурса contact</span><span class="sxs-lookup"><span data-stu-id="4c992-104">contact resource type</span></span>

<span data-ttu-id="4c992-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c992-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4c992-p102">Контакт — элемент в Outlook, в котором вы можете упорядочить и хранить сведения о людях и организациях, с которыми поддерживаете связь. Контакты содержатся в папках контактов.</span><span class="sxs-lookup"><span data-stu-id="4c992-p102">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="4c992-108">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="4c992-108">This resource supports:</span></span>

- <span data-ttu-id="4c992-109">добавление собственных данных к настраиваемым свойствам в виде [расширений](/graph/extensibility-overview);</span><span class="sxs-lookup"><span data-stu-id="4c992-109">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="4c992-110">подписку на [уведомления об изменениях](/graph/webhooks);</span><span class="sxs-lookup"><span data-stu-id="4c992-110">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="4c992-111">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/contact-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="4c992-111">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="4c992-112">Методы</span><span class="sxs-lookup"><span data-stu-id="4c992-112">Methods</span></span>

| <span data-ttu-id="4c992-113">Метод</span><span class="sxs-lookup"><span data-stu-id="4c992-113">Method</span></span>       | <span data-ttu-id="4c992-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4c992-114">Return Type</span></span>  |<span data-ttu-id="4c992-115">Описание</span><span class="sxs-lookup"><span data-stu-id="4c992-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4c992-116">Получение контакта</span><span class="sxs-lookup"><span data-stu-id="4c992-116">Get contact</span></span>](../api/contact-get.md) | [<span data-ttu-id="4c992-117">contact</span><span class="sxs-lookup"><span data-stu-id="4c992-117">contact</span></span>](contact.md) |<span data-ttu-id="4c992-118">Считывание свойств и отношений объекта contact.</span><span class="sxs-lookup"><span data-stu-id="4c992-118">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="4c992-119">Создание</span><span class="sxs-lookup"><span data-stu-id="4c992-119">Create</span></span>](../api/user-post-contacts.md) | [<span data-ttu-id="4c992-120">contact</span><span class="sxs-lookup"><span data-stu-id="4c992-120">contact</span></span>](contact.md) |<span data-ttu-id="4c992-121">Добавление контакта в корневую папку с контактами или конечную точку контактов другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="4c992-121">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="4c992-122">Обновление</span><span class="sxs-lookup"><span data-stu-id="4c992-122">Update</span></span>](../api/contact-update.md) | [<span data-ttu-id="4c992-123">contact</span><span class="sxs-lookup"><span data-stu-id="4c992-123">contact</span></span>](contact.md) |<span data-ttu-id="4c992-124">Обновление объекта contact.</span><span class="sxs-lookup"><span data-stu-id="4c992-124">Update contact object.</span></span> |
|[<span data-ttu-id="4c992-125">Удаление</span><span class="sxs-lookup"><span data-stu-id="4c992-125">Delete</span></span>](../api/contact-delete.md) | <span data-ttu-id="4c992-126">Нет</span><span class="sxs-lookup"><span data-stu-id="4c992-126">None</span></span> |<span data-ttu-id="4c992-127">Удаление объекта contact.</span><span class="sxs-lookup"><span data-stu-id="4c992-127">Delete contact object.</span></span> |
|[<span data-ttu-id="4c992-128">delta</span><span class="sxs-lookup"><span data-stu-id="4c992-128">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="4c992-129">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="4c992-129">[contact](contact.md) collection</span></span>| <span data-ttu-id="4c992-130">Получение набора контактов, которые были добавлены в указанную папку, обновлены в ней или удалены из нее.</span><span class="sxs-lookup"><span data-stu-id="4c992-130">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="4c992-131">**Открытые расширения**</span><span class="sxs-lookup"><span data-stu-id="4c992-131">**Open extensions**</span></span>| | |
|[<span data-ttu-id="4c992-132">Создание открытого расширения</span><span class="sxs-lookup"><span data-stu-id="4c992-132">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="4c992-133">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="4c992-133">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="4c992-134">Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.</span><span class="sxs-lookup"><span data-stu-id="4c992-134">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="4c992-135">Получение открытого расширения</span><span class="sxs-lookup"><span data-stu-id="4c992-135">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="4c992-136">Коллекция [openTypeExtension](opentypeextension.md)</span><span class="sxs-lookup"><span data-stu-id="4c992-136">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="4c992-137">Получение объектов открытого расширения, которые определяются по имени или полному имени.</span><span class="sxs-lookup"><span data-stu-id="4c992-137">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="4c992-138">**Расширения схемы**</span><span class="sxs-lookup"><span data-stu-id="4c992-138">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="4c992-139">Добавление значений расширений для схемы</span><span class="sxs-lookup"><span data-stu-id="4c992-139">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="4c992-140">Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.</span><span class="sxs-lookup"><span data-stu-id="4c992-140">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="4c992-141">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="4c992-141">**Extended properties**</span></span>| | |
|[<span data-ttu-id="4c992-142">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="4c992-142">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="4c992-143">contact</span><span class="sxs-lookup"><span data-stu-id="4c992-143">contact</span></span>](contact.md)  |<span data-ttu-id="4c992-144">Создание одного или нескольких расширенных свойств с одним значением в новом или существующем контакте.</span><span class="sxs-lookup"><span data-stu-id="4c992-144">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="4c992-145">Получение контакта с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="4c992-145">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="4c992-146">contact</span><span class="sxs-lookup"><span data-stu-id="4c992-146">contact</span></span>](contact.md) | <span data-ttu-id="4c992-147">Получение контактов, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="4c992-147">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="4c992-148">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="4c992-148">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="4c992-149">contact</span><span class="sxs-lookup"><span data-stu-id="4c992-149">contact</span></span>](contact.md) | <span data-ttu-id="4c992-150">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем контакте.</span><span class="sxs-lookup"><span data-stu-id="4c992-150">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="4c992-151">Получение контакта с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="4c992-151">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="4c992-152">contact</span><span class="sxs-lookup"><span data-stu-id="4c992-152">contact</span></span>](contact.md) | <span data-ttu-id="4c992-153">Получение контакта, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`.</span><span class="sxs-lookup"><span data-stu-id="4c992-153">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="4c992-154">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c992-154">Properties</span></span>
| <span data-ttu-id="4c992-155">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c992-155">Property</span></span>     | <span data-ttu-id="4c992-156">Тип</span><span class="sxs-lookup"><span data-stu-id="4c992-156">Type</span></span>   |<span data-ttu-id="4c992-157">Описание</span><span class="sxs-lookup"><span data-stu-id="4c992-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c992-158">assistantName</span><span class="sxs-lookup"><span data-stu-id="4c992-158">assistantName</span></span>|<span data-ttu-id="4c992-159">String</span><span class="sxs-lookup"><span data-stu-id="4c992-159">String</span></span>|<span data-ttu-id="4c992-160">Имя помощника контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-160">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="4c992-161">birthday</span><span class="sxs-lookup"><span data-stu-id="4c992-161">birthday</span></span>|<span data-ttu-id="4c992-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c992-162">DateTimeOffset</span></span>|<span data-ttu-id="4c992-p103">Дата рождения контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4c992-p103">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4c992-166">businessAddress</span><span class="sxs-lookup"><span data-stu-id="4c992-166">businessAddress</span></span>|[<span data-ttu-id="4c992-167">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="4c992-167">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="4c992-168">Рабочий адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-168">The contact's business address.</span></span>|
|<span data-ttu-id="4c992-169">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="4c992-169">businessHomePage</span></span>|<span data-ttu-id="4c992-170">String</span><span class="sxs-lookup"><span data-stu-id="4c992-170">String</span></span>|<span data-ttu-id="4c992-171">Домашняя страница контакта (рабочая).</span><span class="sxs-lookup"><span data-stu-id="4c992-171">The business home page of the contact.</span></span>|
|<span data-ttu-id="4c992-172">businessPhones</span><span class="sxs-lookup"><span data-stu-id="4c992-172">businessPhones</span></span>|<span data-ttu-id="4c992-173">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4c992-173">String collection</span></span>|<span data-ttu-id="4c992-174">Рабочие номера телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-174">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="4c992-175">categories</span><span class="sxs-lookup"><span data-stu-id="4c992-175">categories</span></span>|<span data-ttu-id="4c992-176">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4c992-176">String collection</span></span>|<span data-ttu-id="4c992-177">Категории, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="4c992-177">The categories associated with the contact.</span></span>|
|<span data-ttu-id="4c992-178">changeKey</span><span class="sxs-lookup"><span data-stu-id="4c992-178">changeKey</span></span>|<span data-ttu-id="4c992-179">Строка</span><span class="sxs-lookup"><span data-stu-id="4c992-179">String</span></span>|<span data-ttu-id="4c992-p104">Указывает версию контакта. При каждом изменении контакта также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="4c992-p104">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="4c992-183">children</span><span class="sxs-lookup"><span data-stu-id="4c992-183">children</span></span>|<span data-ttu-id="4c992-184">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4c992-184">String collection</span></span>|<span data-ttu-id="4c992-185">Имена детей контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-185">The names of the contact's children.</span></span>|
|<span data-ttu-id="4c992-186">companyName</span><span class="sxs-lookup"><span data-stu-id="4c992-186">companyName</span></span>|<span data-ttu-id="4c992-187">String</span><span class="sxs-lookup"><span data-stu-id="4c992-187">String</span></span>|<span data-ttu-id="4c992-188">Название компании контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-188">The name of the contact's company.</span></span>|
|<span data-ttu-id="4c992-189">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c992-189">createdDateTime</span></span>|<span data-ttu-id="4c992-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c992-190">DateTimeOffset</span></span>|<span data-ttu-id="4c992-p105">Время создания контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4c992-p105">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4c992-194">отделу;</span><span class="sxs-lookup"><span data-stu-id="4c992-194">department</span></span>|<span data-ttu-id="4c992-195">String</span><span class="sxs-lookup"><span data-stu-id="4c992-195">String</span></span>|<span data-ttu-id="4c992-196">Отдел контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-196">The contact's department.</span></span>|
|<span data-ttu-id="4c992-197">displayName</span><span class="sxs-lookup"><span data-stu-id="4c992-197">displayName</span></span>|<span data-ttu-id="4c992-198">String</span><span class="sxs-lookup"><span data-stu-id="4c992-198">String</span></span>|<span data-ttu-id="4c992-199">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-199">The contact's display name.</span></span> <span data-ttu-id="4c992-200">Отображаемое имя можно указать в операции [создания](../api/user-post-contacts.md) или [обновления](../api/contact-update.md).</span><span class="sxs-lookup"><span data-stu-id="4c992-200">You can specify the display name in a [create](../api/user-post-contacts.md) or [update](../api/contact-update.md) operation.</span></span> <span data-ttu-id="4c992-201">Обратите внимание, что последующие обновления других свойств могут привести к тому, что автоматически созданное значение перезапишет указанное значение displayName.</span><span class="sxs-lookup"><span data-stu-id="4c992-201">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="4c992-202">Чтобы сохранить существующее значение, всегда добавляйте его как displayName в операцию [обновления](../api/contact-update.md).</span><span class="sxs-lookup"><span data-stu-id="4c992-202">To preserve a pre-existing value, always include it as displayName in an [update](../api/contact-update.md) operation.</span></span>|
|<span data-ttu-id="4c992-203">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="4c992-203">emailAddresses</span></span>|<span data-ttu-id="4c992-204">Коллекция [EmailAddress](emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="4c992-204">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="4c992-205">Электронные адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-205">The contact's email addresses.</span></span>|
|<span data-ttu-id="4c992-206">fileAs</span><span class="sxs-lookup"><span data-stu-id="4c992-206">fileAs</span></span>|<span data-ttu-id="4c992-207">String</span><span class="sxs-lookup"><span data-stu-id="4c992-207">String</span></span>|<span data-ttu-id="4c992-208">Имя, под которым хранится контакт.</span><span class="sxs-lookup"><span data-stu-id="4c992-208">The name the contact is filed under.</span></span>|
|<span data-ttu-id="4c992-209">generation</span><span class="sxs-lookup"><span data-stu-id="4c992-209">generation</span></span>|<span data-ttu-id="4c992-210">String</span><span class="sxs-lookup"><span data-stu-id="4c992-210">String</span></span>|<span data-ttu-id="4c992-211">Поколение контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-211">The contact's generation.</span></span>|
|<span data-ttu-id="4c992-212">givenName</span><span class="sxs-lookup"><span data-stu-id="4c992-212">givenName</span></span>|<span data-ttu-id="4c992-213">String</span><span class="sxs-lookup"><span data-stu-id="4c992-213">String</span></span>|<span data-ttu-id="4c992-214">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-214">The contact's given name.</span></span>|
|<span data-ttu-id="4c992-215">homeAddress</span><span class="sxs-lookup"><span data-stu-id="4c992-215">homeAddress</span></span>|[<span data-ttu-id="4c992-216">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="4c992-216">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="4c992-217">Домашний адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-217">The contact's home address.</span></span>|
|<span data-ttu-id="4c992-218">homePhones</span><span class="sxs-lookup"><span data-stu-id="4c992-218">homePhones</span></span>|<span data-ttu-id="4c992-219">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4c992-219">String collection</span></span>|<span data-ttu-id="4c992-220">Номера домашних телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-220">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="4c992-221">id</span><span class="sxs-lookup"><span data-stu-id="4c992-221">id</span></span>|<span data-ttu-id="4c992-222">String</span><span class="sxs-lookup"><span data-stu-id="4c992-222">String</span></span>|<span data-ttu-id="4c992-p107">Уникальный идентификатор контакта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c992-p107">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="4c992-225">imAddresses</span><span class="sxs-lookup"><span data-stu-id="4c992-225">imAddresses</span></span>|<span data-ttu-id="4c992-226">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4c992-226">String collection</span></span>|<span data-ttu-id="4c992-227">Адреса контакта для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="4c992-227">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="4c992-228">initials</span><span class="sxs-lookup"><span data-stu-id="4c992-228">initials</span></span>|<span data-ttu-id="4c992-229">String</span><span class="sxs-lookup"><span data-stu-id="4c992-229">String</span></span>|<span data-ttu-id="4c992-230">Инициалы контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-230">The contact's initials.</span></span>|
|<span data-ttu-id="4c992-231">jobTitle</span><span class="sxs-lookup"><span data-stu-id="4c992-231">jobTitle</span></span>|<span data-ttu-id="4c992-232">String</span><span class="sxs-lookup"><span data-stu-id="4c992-232">String</span></span>|<span data-ttu-id="4c992-233">Должность контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-233">The contact’s job title.</span></span>|
|<span data-ttu-id="4c992-234">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c992-234">lastModifiedDateTime</span></span>|<span data-ttu-id="4c992-235">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c992-235">DateTimeOffset</span></span>|<span data-ttu-id="4c992-p108">Время изменения контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4c992-p108">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4c992-239">manager</span><span class="sxs-lookup"><span data-stu-id="4c992-239">manager</span></span>|<span data-ttu-id="4c992-240">String</span><span class="sxs-lookup"><span data-stu-id="4c992-240">String</span></span>|<span data-ttu-id="4c992-241">Имя руководителя контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-241">The name of the contact's manager.</span></span>
|<span data-ttu-id="4c992-242">middleName</span><span class="sxs-lookup"><span data-stu-id="4c992-242">middleName</span></span>|<span data-ttu-id="4c992-243">String</span><span class="sxs-lookup"><span data-stu-id="4c992-243">String</span></span>|<span data-ttu-id="4c992-244">Отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-244">The contact's middle name.</span></span>|
|<span data-ttu-id="4c992-245">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="4c992-245">mobilePhone</span></span>|<span data-ttu-id="4c992-246">String</span><span class="sxs-lookup"><span data-stu-id="4c992-246">String</span></span>|<span data-ttu-id="4c992-247">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-247">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="4c992-248">nickName</span><span class="sxs-lookup"><span data-stu-id="4c992-248">nickName</span></span>|<span data-ttu-id="4c992-249">String</span><span class="sxs-lookup"><span data-stu-id="4c992-249">String</span></span>|<span data-ttu-id="4c992-250">Псевдоним контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-250">The contact's nickname.</span></span>|
|<span data-ttu-id="4c992-251">officeLocation</span><span class="sxs-lookup"><span data-stu-id="4c992-251">officeLocation</span></span>|<span data-ttu-id="4c992-252">String</span><span class="sxs-lookup"><span data-stu-id="4c992-252">String</span></span>|<span data-ttu-id="4c992-253">Расположение офиса контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-253">The location of the contact's office.</span></span>|
|<span data-ttu-id="4c992-254">otherAddress</span><span class="sxs-lookup"><span data-stu-id="4c992-254">otherAddress</span></span>|[<span data-ttu-id="4c992-255">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="4c992-255">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="4c992-256">Другие адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-256">Other addresses for the contact.</span></span>|
|<span data-ttu-id="4c992-257">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="4c992-257">parentFolderId</span></span>|<span data-ttu-id="4c992-258">String</span><span class="sxs-lookup"><span data-stu-id="4c992-258">String</span></span>|<span data-ttu-id="4c992-259">Идентификатор родительской папки контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-259">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="4c992-260">personalNotes</span><span class="sxs-lookup"><span data-stu-id="4c992-260">personalNotes</span></span>|<span data-ttu-id="4c992-261">String</span><span class="sxs-lookup"><span data-stu-id="4c992-261">String</span></span>|<span data-ttu-id="4c992-262">Заметки пользователя о контакте.</span><span class="sxs-lookup"><span data-stu-id="4c992-262">The user's notes about the contact.</span></span>|
|<span data-ttu-id="4c992-263">profession</span><span class="sxs-lookup"><span data-stu-id="4c992-263">profession</span></span>|<span data-ttu-id="4c992-264">String</span><span class="sxs-lookup"><span data-stu-id="4c992-264">String</span></span>|<span data-ttu-id="4c992-265">Профессия контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-265">The contact's profession.</span></span>|
|<span data-ttu-id="4c992-266">spouseName</span><span class="sxs-lookup"><span data-stu-id="4c992-266">spouseName</span></span>|<span data-ttu-id="4c992-267">String</span><span class="sxs-lookup"><span data-stu-id="4c992-267">String</span></span>|<span data-ttu-id="4c992-268">Имя супруга или супруги контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-268">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="4c992-269">surname</span><span class="sxs-lookup"><span data-stu-id="4c992-269">surname</span></span>|<span data-ttu-id="4c992-270">String</span><span class="sxs-lookup"><span data-stu-id="4c992-270">String</span></span>|<span data-ttu-id="4c992-271">Фамилия контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-271">The contact's surname.</span></span>|
|<span data-ttu-id="4c992-272">title</span><span class="sxs-lookup"><span data-stu-id="4c992-272">title</span></span>|<span data-ttu-id="4c992-273">String</span><span class="sxs-lookup"><span data-stu-id="4c992-273">String</span></span>|<span data-ttu-id="4c992-274">Звание контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-274">The contact's title.</span></span>|
|<span data-ttu-id="4c992-275">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="4c992-275">yomiCompanyName</span></span>|<span data-ttu-id="4c992-276">String</span><span class="sxs-lookup"><span data-stu-id="4c992-276">String</span></span>|<span data-ttu-id="4c992-277">Название компании контакта, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="4c992-277">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="4c992-278">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="4c992-278">yomiGivenName</span></span>|<span data-ttu-id="4c992-279">String</span><span class="sxs-lookup"><span data-stu-id="4c992-279">String</span></span>|<span data-ttu-id="4c992-280">Имя контакта, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="4c992-280">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="4c992-281">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="4c992-281">yomiSurname</span></span>|<span data-ttu-id="4c992-282">String</span><span class="sxs-lookup"><span data-stu-id="4c992-282">String</span></span>|<span data-ttu-id="4c992-283">Фамилия контакта, записанная так, как она звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="4c992-283">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c992-284">Отношения</span><span class="sxs-lookup"><span data-stu-id="4c992-284">Relationships</span></span>
| <span data-ttu-id="4c992-285">Связь</span><span class="sxs-lookup"><span data-stu-id="4c992-285">Relationship</span></span> | <span data-ttu-id="4c992-286">Тип</span><span class="sxs-lookup"><span data-stu-id="4c992-286">Type</span></span>   |<span data-ttu-id="4c992-287">Описание</span><span class="sxs-lookup"><span data-stu-id="4c992-287">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c992-288">extensions</span><span class="sxs-lookup"><span data-stu-id="4c992-288">extensions</span></span>|<span data-ttu-id="4c992-289">Коллекция [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="4c992-289">[extension](extension.md) collection</span></span>|<span data-ttu-id="4c992-p109">Коллекция открытых расширений, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4c992-p109">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="4c992-293">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="4c992-293">multiValueExtendedProperties</span></span>|<span data-ttu-id="4c992-294">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="4c992-294">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="4c992-p110">Коллекция расширенных свойств с несколькими значениями, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4c992-p110">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="4c992-298">Фотография
</span><span class="sxs-lookup"><span data-stu-id="4c992-298">photo</span></span>|[<span data-ttu-id="4c992-299">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="4c992-299">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="4c992-p111">Необязательное фото контакта. Можно получить или задать фото для контакта.</span><span class="sxs-lookup"><span data-stu-id="4c992-p111">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="4c992-302">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="4c992-302">singleValueExtendedProperties</span></span>|<span data-ttu-id="4c992-303">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="4c992-303">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="4c992-p112">Коллекция расширенных свойств с одним значением, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4c992-p112">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c992-307">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c992-307">JSON representation</span></span>

<span data-ttu-id="4c992-308">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c992-308">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="4c992-309">См. также</span><span class="sxs-lookup"><span data-stu-id="4c992-309">See also</span></span>

- [<span data-ttu-id="4c992-310">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="4c992-310">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="4c992-311">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="4c992-311">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)
- [<span data-ttu-id="4c992-312">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="4c992-312">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4c992-313">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="4c992-313">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="4c992-314">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="4c992-314">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

