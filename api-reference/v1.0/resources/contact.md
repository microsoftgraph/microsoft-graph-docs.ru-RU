---
title: Тип ресурса contact
description: Контакт — элемент в Outlook, в котором вы можете упорядочить и хранить сведения о людях и организациях, с которыми поддерживаете связь. Контакты содержатся в папках контактов.
author: angelgolfer-ms
ms.openlocfilehash: 13eb3b1e3f88c5018031176cffbcc89a038073ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334974"
---
# <a name="contact-resource-type"></a><span data-ttu-id="61500-104">Тип ресурса contact</span><span class="sxs-lookup"><span data-stu-id="61500-104">contact resource type</span></span>

<span data-ttu-id="61500-p102">Контакт — элемент в Outlook, в котором вы можете упорядочить и хранить сведения о людях и организациях, с которыми поддерживаете связь. Контакты содержатся в папках контактов.</span><span class="sxs-lookup"><span data-stu-id="61500-p102">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="61500-107">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="61500-107">This resource supports:</span></span>

- <span data-ttu-id="61500-108">Добавление настраиваемых свойств данные как [расширения](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="61500-108">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="61500-109">Подписка на [уведомления об изменении](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="61500-109">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="61500-110">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/contact-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="61500-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="61500-111">Методы</span><span class="sxs-lookup"><span data-stu-id="61500-111">Methods</span></span>

| <span data-ttu-id="61500-112">Метод</span><span class="sxs-lookup"><span data-stu-id="61500-112">Method</span></span>       | <span data-ttu-id="61500-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="61500-113">Return Type</span></span>  |<span data-ttu-id="61500-114">Описание</span><span class="sxs-lookup"><span data-stu-id="61500-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="61500-115">Получение контакта</span><span class="sxs-lookup"><span data-stu-id="61500-115">Get contact</span></span>](../api/contact-get.md) | [<span data-ttu-id="61500-116">contact</span><span class="sxs-lookup"><span data-stu-id="61500-116">contact</span></span>](contact.md) |<span data-ttu-id="61500-117">Считывание свойств и отношений объекта contact.</span><span class="sxs-lookup"><span data-stu-id="61500-117">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="61500-118">Создание</span><span class="sxs-lookup"><span data-stu-id="61500-118">Create</span></span>](../api/user-post-contacts.md) | [<span data-ttu-id="61500-119">contact</span><span class="sxs-lookup"><span data-stu-id="61500-119">contact</span></span>](contact.md) |<span data-ttu-id="61500-120">Добавление контакта в корневую папку с контактами или конечную точку контактов другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="61500-120">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="61500-121">Обновление</span><span class="sxs-lookup"><span data-stu-id="61500-121">Update</span></span>](../api/contact-update.md) | [<span data-ttu-id="61500-122">contact</span><span class="sxs-lookup"><span data-stu-id="61500-122">contact</span></span>](contact.md) |<span data-ttu-id="61500-123">Обновление объекта contact.</span><span class="sxs-lookup"><span data-stu-id="61500-123">Update contact object.</span></span> |
|[<span data-ttu-id="61500-124">Удаление</span><span class="sxs-lookup"><span data-stu-id="61500-124">Delete</span></span>](../api/contact-delete.md) | <span data-ttu-id="61500-125">Нет</span><span class="sxs-lookup"><span data-stu-id="61500-125">None</span></span> |<span data-ttu-id="61500-126">Удаление объекта contact.</span><span class="sxs-lookup"><span data-stu-id="61500-126">Delete contact object.</span></span> |
|[<span data-ttu-id="61500-127">delta</span><span class="sxs-lookup"><span data-stu-id="61500-127">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="61500-128">Коллекция [contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="61500-128">[contact](contact.md) collection</span></span>| <span data-ttu-id="61500-129">Получение набора контактов, которые были добавлены в указанную папку, обновлены в ней или удалены из нее.</span><span class="sxs-lookup"><span data-stu-id="61500-129">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="61500-130">**Открытые расширения**</span><span class="sxs-lookup"><span data-stu-id="61500-130">**Open extensions**</span></span>| | |
|[<span data-ttu-id="61500-131">Создание открытого расширения</span><span class="sxs-lookup"><span data-stu-id="61500-131">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="61500-132">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="61500-132">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="61500-133">Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.</span><span class="sxs-lookup"><span data-stu-id="61500-133">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="61500-134">Получение открытого расширения</span><span class="sxs-lookup"><span data-stu-id="61500-134">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="61500-135">Коллекция [openTypeExtension](opentypeextension.md)</span><span class="sxs-lookup"><span data-stu-id="61500-135">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="61500-136">Получение объектов открытого расширения, которые определяются по имени или полному имени.</span><span class="sxs-lookup"><span data-stu-id="61500-136">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="61500-137">**Расширения схемы**</span><span class="sxs-lookup"><span data-stu-id="61500-137">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="61500-138">Добавление значений расширений для схемы</span><span class="sxs-lookup"><span data-stu-id="61500-138">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="61500-139">Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.</span><span class="sxs-lookup"><span data-stu-id="61500-139">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="61500-140">**Расширенные свойства**</span><span class="sxs-lookup"><span data-stu-id="61500-140">**Extended properties**</span></span>| | |
|[<span data-ttu-id="61500-141">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="61500-141">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="61500-142">contact</span><span class="sxs-lookup"><span data-stu-id="61500-142">contact</span></span>](contact.md)  |<span data-ttu-id="61500-143">Создание одного или нескольких расширенных свойств с одним значением в новом или существующем контакте.</span><span class="sxs-lookup"><span data-stu-id="61500-143">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="61500-144">Получение контакта с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="61500-144">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="61500-145">contact</span><span class="sxs-lookup"><span data-stu-id="61500-145">contact</span></span>](contact.md) | <span data-ttu-id="61500-146">Получение контактов, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="61500-146">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="61500-147">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="61500-147">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="61500-148">contact</span><span class="sxs-lookup"><span data-stu-id="61500-148">contact</span></span>](contact.md) | <span data-ttu-id="61500-149">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем контакте.</span><span class="sxs-lookup"><span data-stu-id="61500-149">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="61500-150">Получение контакта с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="61500-150">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="61500-151">contact</span><span class="sxs-lookup"><span data-stu-id="61500-151">contact</span></span>](contact.md) | <span data-ttu-id="61500-152">Получение контакта, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`.</span><span class="sxs-lookup"><span data-stu-id="61500-152">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="61500-153">Свойства</span><span class="sxs-lookup"><span data-stu-id="61500-153">Properties</span></span>
| <span data-ttu-id="61500-154">Свойство</span><span class="sxs-lookup"><span data-stu-id="61500-154">Property</span></span>     | <span data-ttu-id="61500-155">Тип</span><span class="sxs-lookup"><span data-stu-id="61500-155">Type</span></span>   |<span data-ttu-id="61500-156">Описание</span><span class="sxs-lookup"><span data-stu-id="61500-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61500-157">assistantName</span><span class="sxs-lookup"><span data-stu-id="61500-157">assistantName</span></span>|<span data-ttu-id="61500-158">String</span><span class="sxs-lookup"><span data-stu-id="61500-158">String</span></span>|<span data-ttu-id="61500-159">Имя помощника контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-159">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="61500-160">birthday</span><span class="sxs-lookup"><span data-stu-id="61500-160">birthday</span></span>|<span data-ttu-id="61500-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61500-161">DateTimeOffset</span></span>|<span data-ttu-id="61500-p103">Дата рождения контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="61500-p103">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="61500-165">businessAddress</span><span class="sxs-lookup"><span data-stu-id="61500-165">businessAddress</span></span>|[<span data-ttu-id="61500-166">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="61500-166">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="61500-167">Рабочий адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-167">The contact's business address.</span></span>|
|<span data-ttu-id="61500-168">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="61500-168">businessHomePage</span></span>|<span data-ttu-id="61500-169">String</span><span class="sxs-lookup"><span data-stu-id="61500-169">String</span></span>|<span data-ttu-id="61500-170">Домашняя страница контакта (рабочая).</span><span class="sxs-lookup"><span data-stu-id="61500-170">The business home page of the contact.</span></span>|
|<span data-ttu-id="61500-171">businessPhones</span><span class="sxs-lookup"><span data-stu-id="61500-171">businessPhones</span></span>|<span data-ttu-id="61500-172">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="61500-172">String collection</span></span>|<span data-ttu-id="61500-173">Рабочие номера телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-173">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="61500-174">categories</span><span class="sxs-lookup"><span data-stu-id="61500-174">categories</span></span>|<span data-ttu-id="61500-175">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="61500-175">String collection</span></span>|<span data-ttu-id="61500-176">Категории, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="61500-176">The categories associated with the contact.</span></span>|
|<span data-ttu-id="61500-177">changeKey</span><span class="sxs-lookup"><span data-stu-id="61500-177">changeKey</span></span>|<span data-ttu-id="61500-178">Строка</span><span class="sxs-lookup"><span data-stu-id="61500-178">String</span></span>|<span data-ttu-id="61500-p104">Указывает версию контакта. При каждом изменении контакта также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="61500-p104">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="61500-182">children</span><span class="sxs-lookup"><span data-stu-id="61500-182">children</span></span>|<span data-ttu-id="61500-183">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="61500-183">String collection</span></span>|<span data-ttu-id="61500-184">Имена детей контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-184">The names of the contact's children.</span></span>|
|<span data-ttu-id="61500-185">companyName</span><span class="sxs-lookup"><span data-stu-id="61500-185">companyName</span></span>|<span data-ttu-id="61500-186">String</span><span class="sxs-lookup"><span data-stu-id="61500-186">String</span></span>|<span data-ttu-id="61500-187">Название компании контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-187">The name of the contact's company.</span></span>|
|<span data-ttu-id="61500-188">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61500-188">createdDateTime</span></span>|<span data-ttu-id="61500-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61500-189">DateTimeOffset</span></span>|<span data-ttu-id="61500-p105">Время создания контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="61500-p105">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="61500-193">отделу;</span><span class="sxs-lookup"><span data-stu-id="61500-193">department</span></span>|<span data-ttu-id="61500-194">String</span><span class="sxs-lookup"><span data-stu-id="61500-194">String</span></span>|<span data-ttu-id="61500-195">Отдел контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-195">The contact's department.</span></span>|
|<span data-ttu-id="61500-196">displayName</span><span class="sxs-lookup"><span data-stu-id="61500-196">displayName</span></span>|<span data-ttu-id="61500-197">String</span><span class="sxs-lookup"><span data-stu-id="61500-197">String</span></span>|<span data-ttu-id="61500-198">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-198">The contact's display name.</span></span> <span data-ttu-id="61500-199">В ходе операции [создания](../api/user-post-contacts.md) или [обновления](../api/contact-update.md) можно указать отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="61500-199">You can specify the display name in a [create](../api/user-post-contacts.md) or [update](../api/contact-update.md) operation.</span></span> <span data-ttu-id="61500-200">Обратите внимание, что более поздние обновления для других свойств может стать причиной автоматически подставленное значение для перезаписи значение displayName, заданные.</span><span class="sxs-lookup"><span data-stu-id="61500-200">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="61500-201">Чтобы сохранить существующие значения, всегда включите его в качестве displayName в рамках одной операции [обновления](../api/contact-update.md) .</span><span class="sxs-lookup"><span data-stu-id="61500-201">To preserve a pre-existing value, always include it as displayName in an [update](../api/contact-update.md) operation.</span></span>|
|<span data-ttu-id="61500-202">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="61500-202">emailAddresses</span></span>|<span data-ttu-id="61500-203">Коллекция [EmailAddress](emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="61500-203">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="61500-204">Электронные адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-204">The contact's email addresses.</span></span>|
|<span data-ttu-id="61500-205">fileAs</span><span class="sxs-lookup"><span data-stu-id="61500-205">fileAs</span></span>|<span data-ttu-id="61500-206">String</span><span class="sxs-lookup"><span data-stu-id="61500-206">String</span></span>|<span data-ttu-id="61500-207">Имя, под которым хранится контакт.</span><span class="sxs-lookup"><span data-stu-id="61500-207">The name the contact is filed under.</span></span>|
|<span data-ttu-id="61500-208">generation</span><span class="sxs-lookup"><span data-stu-id="61500-208">generation</span></span>|<span data-ttu-id="61500-209">String</span><span class="sxs-lookup"><span data-stu-id="61500-209">String</span></span>|<span data-ttu-id="61500-210">Поколение контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-210">The contact's generation.</span></span>|
|<span data-ttu-id="61500-211">givenName</span><span class="sxs-lookup"><span data-stu-id="61500-211">givenName</span></span>|<span data-ttu-id="61500-212">String</span><span class="sxs-lookup"><span data-stu-id="61500-212">String</span></span>|<span data-ttu-id="61500-213">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-213">The contact's given name.</span></span>|
|<span data-ttu-id="61500-214">homeAddress</span><span class="sxs-lookup"><span data-stu-id="61500-214">homeAddress</span></span>|[<span data-ttu-id="61500-215">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="61500-215">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="61500-216">Домашний адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-216">The contact's home address.</span></span>|
|<span data-ttu-id="61500-217">homePhones</span><span class="sxs-lookup"><span data-stu-id="61500-217">homePhones</span></span>|<span data-ttu-id="61500-218">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="61500-218">String collection</span></span>|<span data-ttu-id="61500-219">Номера домашних телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-219">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="61500-220">id</span><span class="sxs-lookup"><span data-stu-id="61500-220">id</span></span>|<span data-ttu-id="61500-221">String</span><span class="sxs-lookup"><span data-stu-id="61500-221">String</span></span>|<span data-ttu-id="61500-p107">Уникальный идентификатор контакта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61500-p107">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="61500-224">imAddresses</span><span class="sxs-lookup"><span data-stu-id="61500-224">imAddresses</span></span>|<span data-ttu-id="61500-225">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="61500-225">String collection</span></span>|<span data-ttu-id="61500-226">Адреса контакта для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="61500-226">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="61500-227">initials</span><span class="sxs-lookup"><span data-stu-id="61500-227">initials</span></span>|<span data-ttu-id="61500-228">String</span><span class="sxs-lookup"><span data-stu-id="61500-228">String</span></span>|<span data-ttu-id="61500-229">Инициалы контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-229">The contact's initials.</span></span>|
|<span data-ttu-id="61500-230">jobTitle</span><span class="sxs-lookup"><span data-stu-id="61500-230">jobTitle</span></span>|<span data-ttu-id="61500-231">String</span><span class="sxs-lookup"><span data-stu-id="61500-231">String</span></span>|<span data-ttu-id="61500-232">Должность контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-232">The contact’s job title.</span></span>|
|<span data-ttu-id="61500-233">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61500-233">lastModifiedDateTime</span></span>|<span data-ttu-id="61500-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61500-234">DateTimeOffset</span></span>|<span data-ttu-id="61500-p108">Время изменения контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="61500-p108">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="61500-238">manager</span><span class="sxs-lookup"><span data-stu-id="61500-238">manager</span></span>|<span data-ttu-id="61500-239">String</span><span class="sxs-lookup"><span data-stu-id="61500-239">String</span></span>|<span data-ttu-id="61500-240">Имя руководителя контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-240">The name of the contact's manager.</span></span>
|<span data-ttu-id="61500-241">middleName</span><span class="sxs-lookup"><span data-stu-id="61500-241">middleName</span></span>|<span data-ttu-id="61500-242">String</span><span class="sxs-lookup"><span data-stu-id="61500-242">String</span></span>|<span data-ttu-id="61500-243">Отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-243">The contact's middle name.</span></span>|
|<span data-ttu-id="61500-244">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="61500-244">mobilePhone</span></span>|<span data-ttu-id="61500-245">String</span><span class="sxs-lookup"><span data-stu-id="61500-245">String</span></span>|<span data-ttu-id="61500-246">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-246">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="61500-247">nickName</span><span class="sxs-lookup"><span data-stu-id="61500-247">nickName</span></span>|<span data-ttu-id="61500-248">String</span><span class="sxs-lookup"><span data-stu-id="61500-248">String</span></span>|<span data-ttu-id="61500-249">Псевдоним контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-249">The contact's nickname.</span></span>|
|<span data-ttu-id="61500-250">officeLocation</span><span class="sxs-lookup"><span data-stu-id="61500-250">officeLocation</span></span>|<span data-ttu-id="61500-251">String</span><span class="sxs-lookup"><span data-stu-id="61500-251">String</span></span>|<span data-ttu-id="61500-252">Расположение офиса контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-252">The location of the contact's office.</span></span>|
|<span data-ttu-id="61500-253">otherAddress</span><span class="sxs-lookup"><span data-stu-id="61500-253">otherAddress</span></span>|[<span data-ttu-id="61500-254">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="61500-254">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="61500-255">Другие адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-255">Other addresses for the contact.</span></span>|
|<span data-ttu-id="61500-256">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="61500-256">parentFolderId</span></span>|<span data-ttu-id="61500-257">String</span><span class="sxs-lookup"><span data-stu-id="61500-257">String</span></span>|<span data-ttu-id="61500-258">Идентификатор родительской папки контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-258">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="61500-259">personalNotes</span><span class="sxs-lookup"><span data-stu-id="61500-259">personalNotes</span></span>|<span data-ttu-id="61500-260">String</span><span class="sxs-lookup"><span data-stu-id="61500-260">String</span></span>|<span data-ttu-id="61500-261">Заметки пользователя о контакте.</span><span class="sxs-lookup"><span data-stu-id="61500-261">The user's notes about the contact.</span></span>|
|<span data-ttu-id="61500-262">profession</span><span class="sxs-lookup"><span data-stu-id="61500-262">profession</span></span>|<span data-ttu-id="61500-263">String</span><span class="sxs-lookup"><span data-stu-id="61500-263">String</span></span>|<span data-ttu-id="61500-264">Профессия контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-264">The contact's profession.</span></span>|
|<span data-ttu-id="61500-265">spouseName</span><span class="sxs-lookup"><span data-stu-id="61500-265">spouseName</span></span>|<span data-ttu-id="61500-266">String</span><span class="sxs-lookup"><span data-stu-id="61500-266">String</span></span>|<span data-ttu-id="61500-267">Имя супруга или супруги контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-267">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="61500-268">surname</span><span class="sxs-lookup"><span data-stu-id="61500-268">surname</span></span>|<span data-ttu-id="61500-269">String</span><span class="sxs-lookup"><span data-stu-id="61500-269">String</span></span>|<span data-ttu-id="61500-270">Фамилия контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-270">The contact's surname.</span></span>|
|<span data-ttu-id="61500-271">title</span><span class="sxs-lookup"><span data-stu-id="61500-271">title</span></span>|<span data-ttu-id="61500-272">String</span><span class="sxs-lookup"><span data-stu-id="61500-272">String</span></span>|<span data-ttu-id="61500-273">Звание контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-273">The contact's title.</span></span>|
|<span data-ttu-id="61500-274">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="61500-274">yomiCompanyName</span></span>|<span data-ttu-id="61500-275">String</span><span class="sxs-lookup"><span data-stu-id="61500-275">String</span></span>|<span data-ttu-id="61500-276">Название компании контакта, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="61500-276">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="61500-277">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="61500-277">yomiGivenName</span></span>|<span data-ttu-id="61500-278">String</span><span class="sxs-lookup"><span data-stu-id="61500-278">String</span></span>|<span data-ttu-id="61500-279">Имя контакта, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="61500-279">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="61500-280">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="61500-280">yomiSurname</span></span>|<span data-ttu-id="61500-281">String</span><span class="sxs-lookup"><span data-stu-id="61500-281">String</span></span>|<span data-ttu-id="61500-282">Фамилия контакта, записанная так, как она звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="61500-282">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61500-283">Отношения</span><span class="sxs-lookup"><span data-stu-id="61500-283">Relationships</span></span>
| <span data-ttu-id="61500-284">Связь</span><span class="sxs-lookup"><span data-stu-id="61500-284">Relationship</span></span> | <span data-ttu-id="61500-285">Тип</span><span class="sxs-lookup"><span data-stu-id="61500-285">Type</span></span>   |<span data-ttu-id="61500-286">Описание</span><span class="sxs-lookup"><span data-stu-id="61500-286">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61500-287">extensions</span><span class="sxs-lookup"><span data-stu-id="61500-287">extensions</span></span>|<span data-ttu-id="61500-288">Коллекция [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="61500-288">[extension](extension.md) collection</span></span>|<span data-ttu-id="61500-p109">Коллекция открытых расширений, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="61500-p109">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="61500-292">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="61500-292">multiValueExtendedProperties</span></span>|<span data-ttu-id="61500-293">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="61500-293">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="61500-p110">Коллекция расширенных свойств с несколькими значениями, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="61500-p110">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="61500-297">photo</span><span class="sxs-lookup"><span data-stu-id="61500-297">photo</span></span>|[<span data-ttu-id="61500-298">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="61500-298">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="61500-p111">Необязательное фото контакта. Можно получить или задать фото для контакта.</span><span class="sxs-lookup"><span data-stu-id="61500-p111">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="61500-301">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="61500-301">singleValueExtendedProperties</span></span>|<span data-ttu-id="61500-302">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="61500-302">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="61500-p112">Коллекция расширенных свойств с одним значением, определенных для контакта. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="61500-p112">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61500-306">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61500-306">JSON representation</span></span>

<span data-ttu-id="61500-307">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61500-307">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="61500-308">См. также</span><span class="sxs-lookup"><span data-stu-id="61500-308">See also</span></span>

- [<span data-ttu-id="61500-309">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="61500-309">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="61500-310">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="61500-310">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)
- [<span data-ttu-id="61500-311">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="61500-311">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="61500-312">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="61500-312">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="61500-313">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="61500-313">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
