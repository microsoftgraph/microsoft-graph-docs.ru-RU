# <a name="update-contact"></a><span data-ttu-id="eea84-101">Обновление контакта</span><span class="sxs-lookup"><span data-stu-id="eea84-101">Update contact</span></span>

<span data-ttu-id="eea84-102">Обновление свойств объекта contact.</span><span class="sxs-lookup"><span data-stu-id="eea84-102">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="eea84-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eea84-103">Permissions</span></span>
<span data-ttu-id="eea84-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eea84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eea84-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eea84-106">Permission type</span></span>      | <span data-ttu-id="eea84-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eea84-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eea84-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eea84-108">Delegated (work or school account)</span></span> | <span data-ttu-id="eea84-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eea84-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="eea84-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eea84-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eea84-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eea84-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="eea84-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eea84-112">Application</span></span> | <span data-ttu-id="eea84-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eea84-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eea84-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eea84-114">HTTP request</span></span>
<span data-ttu-id="eea84-115"><!-- { "blockType": "ignored" } -->[Обратитесь](../resources/contact.md) в пользователя по умолчанию [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="eea84-115"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="eea84-116">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="eea84-116">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="eea84-p102">Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md). Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="eea84-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="eea84-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eea84-119">Request headers</span></span>
| <span data-ttu-id="eea84-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eea84-120">Header</span></span>       | <span data-ttu-id="eea84-121">Значение</span><span class="sxs-lookup"><span data-stu-id="eea84-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eea84-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eea84-122">Authorization</span></span>  | <span data-ttu-id="eea84-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eea84-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eea84-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eea84-125">Content-Type</span></span>  | <span data-ttu-id="eea84-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eea84-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eea84-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eea84-128">Request body</span></span>
<span data-ttu-id="eea84-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="eea84-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eea84-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="eea84-132">Property</span></span>     | <span data-ttu-id="eea84-133">Тип</span><span class="sxs-lookup"><span data-stu-id="eea84-133">Type</span></span>   |<span data-ttu-id="eea84-134">Описание</span><span class="sxs-lookup"><span data-stu-id="eea84-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eea84-135">assistantName</span><span class="sxs-lookup"><span data-stu-id="eea84-135">assistantName</span></span>|<span data-ttu-id="eea84-136">String</span><span class="sxs-lookup"><span data-stu-id="eea84-136">String</span></span>|<span data-ttu-id="eea84-137">Имя помощника контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-137">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="eea84-138">birthday</span><span class="sxs-lookup"><span data-stu-id="eea84-138">birthday</span></span>|<span data-ttu-id="eea84-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eea84-139">DateTimeOffset</span></span>|<span data-ttu-id="eea84-140">Дата рождения контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-140">The contact's birthday.</span></span>|
|<span data-ttu-id="eea84-141">businessAddress</span><span class="sxs-lookup"><span data-stu-id="eea84-141">businessAddress</span></span>|[<span data-ttu-id="eea84-142">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="eea84-142">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="eea84-143">Рабочий адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-143">The contact's business address.</span></span>|
|<span data-ttu-id="eea84-144">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="eea84-144">businessHomePage</span></span>|<span data-ttu-id="eea84-145">String</span><span class="sxs-lookup"><span data-stu-id="eea84-145">String</span></span>|<span data-ttu-id="eea84-146">Домашняя страница контакта (рабочая).</span><span class="sxs-lookup"><span data-stu-id="eea84-146">The business home page of the contact.</span></span>|
|<span data-ttu-id="eea84-147">businessPhones</span><span class="sxs-lookup"><span data-stu-id="eea84-147">businessPhones</span></span>|<span data-ttu-id="eea84-148">String</span><span class="sxs-lookup"><span data-stu-id="eea84-148">String</span></span>|<span data-ttu-id="eea84-149">Рабочие номера телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-149">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="eea84-150">categories</span><span class="sxs-lookup"><span data-stu-id="eea84-150">categories</span></span>|<span data-ttu-id="eea84-151">String</span><span class="sxs-lookup"><span data-stu-id="eea84-151">String</span></span>|<span data-ttu-id="eea84-152">Категории, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="eea84-152">The categories associated with the contact.</span></span>|
|<span data-ttu-id="eea84-153">children</span><span class="sxs-lookup"><span data-stu-id="eea84-153">children</span></span>|<span data-ttu-id="eea84-154">String</span><span class="sxs-lookup"><span data-stu-id="eea84-154">String</span></span>|<span data-ttu-id="eea84-155">Имена детей контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-155">The names of the contact's children.</span></span>|
|<span data-ttu-id="eea84-156">companyName</span><span class="sxs-lookup"><span data-stu-id="eea84-156">companyName</span></span>|<span data-ttu-id="eea84-157">String</span><span class="sxs-lookup"><span data-stu-id="eea84-157">String</span></span>|<span data-ttu-id="eea84-158">Название компании контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-158">The name of the contact's company.</span></span>|
|<span data-ttu-id="eea84-159">department</span><span class="sxs-lookup"><span data-stu-id="eea84-159">department</span></span>|<span data-ttu-id="eea84-160">String</span><span class="sxs-lookup"><span data-stu-id="eea84-160">String</span></span>|<span data-ttu-id="eea84-161">Отдел контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-161">The contact's department.</span></span>|
|<span data-ttu-id="eea84-162">displayName</span><span class="sxs-lookup"><span data-stu-id="eea84-162">displayName</span></span>|<span data-ttu-id="eea84-163">String</span><span class="sxs-lookup"><span data-stu-id="eea84-163">String</span></span>|<span data-ttu-id="eea84-164">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-164">The contact's display name.</span></span> <span data-ttu-id="eea84-165">Обратите внимание, что более поздние обновления для других свойств может стать причиной автоматически подставленное значение для перезаписи значение displayName, заданные.</span><span class="sxs-lookup"><span data-stu-id="eea84-165">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="eea84-166">Чтобы сохранить существующие значения, всегда включите его в качестве displayName в операции обновления.</span><span class="sxs-lookup"><span data-stu-id="eea84-166">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="eea84-167">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="eea84-167">emailAddresses</span></span>|<span data-ttu-id="eea84-168">Коллекция [EmailAddress](../resources/emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="eea84-168">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="eea84-169">Электронные адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-169">The contact's email addresses.</span></span>|
|<span data-ttu-id="eea84-170">fileAs</span><span class="sxs-lookup"><span data-stu-id="eea84-170">fileAs</span></span>|<span data-ttu-id="eea84-171">String</span><span class="sxs-lookup"><span data-stu-id="eea84-171">String</span></span>|<span data-ttu-id="eea84-172">Имя, под которым хранится контакт.</span><span class="sxs-lookup"><span data-stu-id="eea84-172">The name the contact is filed under.</span></span>|
|<span data-ttu-id="eea84-173">generation</span><span class="sxs-lookup"><span data-stu-id="eea84-173">generation</span></span>|<span data-ttu-id="eea84-174">String</span><span class="sxs-lookup"><span data-stu-id="eea84-174">String</span></span>|<span data-ttu-id="eea84-175">Поколение контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-175">The contact's generation.</span></span>|
|<span data-ttu-id="eea84-176">givenName</span><span class="sxs-lookup"><span data-stu-id="eea84-176">givenName</span></span>|<span data-ttu-id="eea84-177">String</span><span class="sxs-lookup"><span data-stu-id="eea84-177">String</span></span>|<span data-ttu-id="eea84-178">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-178">The contact's given name.</span></span>|
|<span data-ttu-id="eea84-179">homeAddress</span><span class="sxs-lookup"><span data-stu-id="eea84-179">homeAddress</span></span>|[<span data-ttu-id="eea84-180">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="eea84-180">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="eea84-181">Домашний адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-181">The contact's home address.</span></span>|
|<span data-ttu-id="eea84-182">homePhones</span><span class="sxs-lookup"><span data-stu-id="eea84-182">homePhones</span></span>|<span data-ttu-id="eea84-183">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="eea84-183">String collection</span></span>|<span data-ttu-id="eea84-184">Номера домашнего телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-184">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="eea84-185">imAddresses</span><span class="sxs-lookup"><span data-stu-id="eea84-185">imAddresses</span></span>|<span data-ttu-id="eea84-186">String</span><span class="sxs-lookup"><span data-stu-id="eea84-186">String</span></span>|<span data-ttu-id="eea84-187">Адреса контакта для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="eea84-187">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="eea84-188">initials</span><span class="sxs-lookup"><span data-stu-id="eea84-188">initials</span></span>|<span data-ttu-id="eea84-189">String</span><span class="sxs-lookup"><span data-stu-id="eea84-189">String</span></span>|<span data-ttu-id="eea84-190">Инициалы контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-190">The contact's initials.</span></span>|
|<span data-ttu-id="eea84-191">jobTitle</span><span class="sxs-lookup"><span data-stu-id="eea84-191">jobTitle</span></span>|<span data-ttu-id="eea84-192">String</span><span class="sxs-lookup"><span data-stu-id="eea84-192">String</span></span>|<span data-ttu-id="eea84-193">Должность контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-193">The contact’s job title.</span></span>|
|<span data-ttu-id="eea84-194">manager</span><span class="sxs-lookup"><span data-stu-id="eea84-194">manager</span></span>|<span data-ttu-id="eea84-195">String</span><span class="sxs-lookup"><span data-stu-id="eea84-195">String</span></span>|<span data-ttu-id="eea84-196">Имя руководителя контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-196">The name of the contact's manager.</span></span>
|<span data-ttu-id="eea84-197">middleName</span><span class="sxs-lookup"><span data-stu-id="eea84-197">middleName</span></span>|<span data-ttu-id="eea84-198">String</span><span class="sxs-lookup"><span data-stu-id="eea84-198">String</span></span>|<span data-ttu-id="eea84-199">Отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-199">The contact's middle name.</span></span>|
|<span data-ttu-id="eea84-200">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="eea84-200">mobilePhone</span></span>|<span data-ttu-id="eea84-201">String</span><span class="sxs-lookup"><span data-stu-id="eea84-201">String</span></span>|<span data-ttu-id="eea84-202">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-202">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="eea84-203">nickName</span><span class="sxs-lookup"><span data-stu-id="eea84-203">nickName</span></span>|<span data-ttu-id="eea84-204">String</span><span class="sxs-lookup"><span data-stu-id="eea84-204">String</span></span>|<span data-ttu-id="eea84-205">Псевдоним контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-205">The contact's nickname.</span></span>|
|<span data-ttu-id="eea84-206">officeLocation</span><span class="sxs-lookup"><span data-stu-id="eea84-206">officeLocation</span></span>|<span data-ttu-id="eea84-207">String</span><span class="sxs-lookup"><span data-stu-id="eea84-207">String</span></span>|<span data-ttu-id="eea84-208">Расположение офиса контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-208">The location of the contact's office.</span></span>|
|<span data-ttu-id="eea84-209">otherAddress</span><span class="sxs-lookup"><span data-stu-id="eea84-209">otherAddress</span></span>|[<span data-ttu-id="eea84-210">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="eea84-210">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="eea84-211">Другие адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-211">Other addresses for the contact.</span></span>|
|<span data-ttu-id="eea84-212">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="eea84-212">parentFolderId</span></span>|<span data-ttu-id="eea84-213">String</span><span class="sxs-lookup"><span data-stu-id="eea84-213">String</span></span>|<span data-ttu-id="eea84-214">Идентификатор родительской папки контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-214">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="eea84-215">personalNotes</span><span class="sxs-lookup"><span data-stu-id="eea84-215">personalNotes</span></span>|<span data-ttu-id="eea84-216">String</span><span class="sxs-lookup"><span data-stu-id="eea84-216">String</span></span>|<span data-ttu-id="eea84-217">Заметки пользователя о контакте.</span><span class="sxs-lookup"><span data-stu-id="eea84-217">The user's notes about the contact.</span></span>|
|<span data-ttu-id="eea84-218">profession</span><span class="sxs-lookup"><span data-stu-id="eea84-218">profession</span></span>|<span data-ttu-id="eea84-219">String</span><span class="sxs-lookup"><span data-stu-id="eea84-219">String</span></span>|<span data-ttu-id="eea84-220">Профессия контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-220">The contact's profession.</span></span>|
|<span data-ttu-id="eea84-221">spouseName</span><span class="sxs-lookup"><span data-stu-id="eea84-221">spouseName</span></span>|<span data-ttu-id="eea84-222">String</span><span class="sxs-lookup"><span data-stu-id="eea84-222">String</span></span>|<span data-ttu-id="eea84-223">Имя супруга или супруги контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-223">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="eea84-224">surname</span><span class="sxs-lookup"><span data-stu-id="eea84-224">surname</span></span>|<span data-ttu-id="eea84-225">String</span><span class="sxs-lookup"><span data-stu-id="eea84-225">String</span></span>|<span data-ttu-id="eea84-226">Фамилия контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-226">The contact's surname.</span></span>|
|<span data-ttu-id="eea84-227">title</span><span class="sxs-lookup"><span data-stu-id="eea84-227">title</span></span>|<span data-ttu-id="eea84-228">String</span><span class="sxs-lookup"><span data-stu-id="eea84-228">String</span></span>|<span data-ttu-id="eea84-229">Звание контакта.</span><span class="sxs-lookup"><span data-stu-id="eea84-229">The contact's title.</span></span>|
|<span data-ttu-id="eea84-230">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="eea84-230">yomiCompanyName</span></span>|<span data-ttu-id="eea84-231">String</span><span class="sxs-lookup"><span data-stu-id="eea84-231">String</span></span>|<span data-ttu-id="eea84-p107">Название компании контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="eea84-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="eea84-234">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="eea84-234">yomiGivenName</span></span>|<span data-ttu-id="eea84-235">String</span><span class="sxs-lookup"><span data-stu-id="eea84-235">String</span></span>|<span data-ttu-id="eea84-p108">Имя контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="eea84-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="eea84-238">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="eea84-238">yomiSurname</span></span>|<span data-ttu-id="eea84-239">String</span><span class="sxs-lookup"><span data-stu-id="eea84-239">String</span></span>|<span data-ttu-id="eea84-p109">Фамилия контакта, записанная так, как она звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="eea84-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="eea84-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="eea84-242">Response</span></span>

<span data-ttu-id="eea84-243">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [contact](../resources/contact.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eea84-243">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eea84-244">Пример</span><span class="sxs-lookup"><span data-stu-id="eea84-244">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eea84-245">Запрос</span><span class="sxs-lookup"><span data-stu-id="eea84-245">Request</span></span>
<span data-ttu-id="eea84-246">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eea84-246">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contacts/{id}
Content-type: application/json
Content-length: 1977

{
  "homeAddress": {
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "postalCode": "98121"
  },
  "birthday": "1974-07-22"
}
```
##### <a name="response"></a><span data-ttu-id="eea84-247">Ответ</span><span class="sxs-lookup"><span data-stu-id="eea84-247">Response</span></span>
<span data-ttu-id="eea84-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="eea84-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1977

{
  "id": "AAMkAGI2THk0AAA=",
  "createdDateTime": "2014-10-19T23:08:24Z",
  "lastModifiedDateTime": "2014-10-19T23:08:24Z",
  "changeKey": "EQAAABYAAACd9nJ/tVysQos2hTfspaWRAAADTIa4",
  "categories": [],
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "birthday": "1974-07-22",
  "fileAs": "Fort, Garth",
  "displayName": "Garth Fort",
  "givenName": "Garth",
  "initials": "G.F.",
  "middleName": null,
  "nickName": "Garth",
  "surname": "Fort",
  "title": null,
  "yomiGivenName": null,
  "yomiSurname": null,
  "yomiCompanyName": null,
  "generation": null,
  "emailAddresses": [
    {
      "name": "Garth",
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com"
    }
  ],
  "imAddresses": [
    "sip:garthf@a830edad9050849nda1.onmicrosoft.com"
  ],
  "jobTitle": "Web Marketing Manager",
  "companyName": "Contoso, Inc.",
  "department": "Sales & Marketing",
  "officeLocation": "20/1101",
  "profession": null,
  "businessHomePage": "https://www.contoso.com",
  "assistantName": null,
  "manager": null,
  "homePhones": [],
  "mobilePhone": null,
  "businessPhones": [
    "+1 918 555 0101"
  ],
  "homeAddress": {
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "postalCode": "98121"
  },
  "businessAddress": {
      "street": "10 Contoso Way",
      "city": "Redmond",
      "state": "WA",
      "countryOrRegion": "USA",
      "postalCode": "98075"  
  },
  "otherAddress": {},
  "spouseName": null,
  "personalNotes": null,
  "children": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
