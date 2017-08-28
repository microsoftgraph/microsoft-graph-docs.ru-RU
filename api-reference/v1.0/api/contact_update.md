# <a name="update-contact"></a><span data-ttu-id="a48bc-101">Обновление контакта</span><span class="sxs-lookup"><span data-stu-id="a48bc-101">Update contact</span></span>

<span data-ttu-id="a48bc-102">Обновление свойств объекта contact.</span><span class="sxs-lookup"><span data-stu-id="a48bc-102">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a48bc-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a48bc-103">Permissions</span></span>
<span data-ttu-id="a48bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a48bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a48bc-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a48bc-106">Permission type</span></span>      | <span data-ttu-id="a48bc-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a48bc-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a48bc-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a48bc-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a48bc-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a48bc-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a48bc-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a48bc-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a48bc-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a48bc-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a48bc-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a48bc-112">Application</span></span> | <span data-ttu-id="a48bc-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a48bc-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a48bc-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a48bc-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a48bc-115">Объект [contact](../resources/contact.md) из стандартной пользовательской папки [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a48bc-115">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="a48bc-116">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="a48bc-116">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="a48bc-p102">Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md). Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="a48bc-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a48bc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a48bc-119">Request headers</span></span>
| <span data-ttu-id="a48bc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a48bc-120">Header</span></span>       | <span data-ttu-id="a48bc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a48bc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a48bc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a48bc-122">Authorization</span></span>  | <span data-ttu-id="a48bc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a48bc-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a48bc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a48bc-125">Content-Type</span></span>  | <span data-ttu-id="a48bc-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a48bc-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a48bc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a48bc-128">Request body</span></span>
<span data-ttu-id="a48bc-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a48bc-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a48bc-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="a48bc-132">Property</span></span>     | <span data-ttu-id="a48bc-133">Тип</span><span class="sxs-lookup"><span data-stu-id="a48bc-133">Type</span></span>   |<span data-ttu-id="a48bc-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a48bc-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a48bc-135">assistantName</span><span class="sxs-lookup"><span data-stu-id="a48bc-135">assistantName</span></span>|<span data-ttu-id="a48bc-136">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-136">String</span></span>|<span data-ttu-id="a48bc-137">Имя помощника контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-137">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="a48bc-138">birthday</span><span class="sxs-lookup"><span data-stu-id="a48bc-138">birthday</span></span>|<span data-ttu-id="a48bc-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a48bc-139">DateTimeOffset</span></span>|<span data-ttu-id="a48bc-140">Дата рождения контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-140">The contact's birthday.</span></span>|
|<span data-ttu-id="a48bc-141">businessAddress</span><span class="sxs-lookup"><span data-stu-id="a48bc-141">businessAddress</span></span>|[<span data-ttu-id="a48bc-142">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="a48bc-142">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="a48bc-143">Рабочий адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-143">The contact's business address.</span></span>|
|<span data-ttu-id="a48bc-144">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="a48bc-144">businessHomePage</span></span>|<span data-ttu-id="a48bc-145">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-145">String</span></span>|<span data-ttu-id="a48bc-146">Домашняя страница контакта (рабочая).</span><span class="sxs-lookup"><span data-stu-id="a48bc-146">The business home page of the contact.</span></span>|
|<span data-ttu-id="a48bc-147">businessPhones</span><span class="sxs-lookup"><span data-stu-id="a48bc-147">businessPhones</span></span>|<span data-ttu-id="a48bc-148">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-148">String</span></span>|<span data-ttu-id="a48bc-149">Рабочие номера телефонов контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-149">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="a48bc-150">categories</span><span class="sxs-lookup"><span data-stu-id="a48bc-150">categories</span></span>|<span data-ttu-id="a48bc-151">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-151">String</span></span>|<span data-ttu-id="a48bc-152">Категории, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="a48bc-152">The categories associated with the contact.</span></span>|
|<span data-ttu-id="a48bc-153">children</span><span class="sxs-lookup"><span data-stu-id="a48bc-153">children</span></span>|<span data-ttu-id="a48bc-154">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-154">String</span></span>|<span data-ttu-id="a48bc-155">Имена детей контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-155">The names of the contact's children.</span></span>|
|<span data-ttu-id="a48bc-156">companyName</span><span class="sxs-lookup"><span data-stu-id="a48bc-156">companyName</span></span>|<span data-ttu-id="a48bc-157">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-157">String</span></span>|<span data-ttu-id="a48bc-158">Название компании контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-158">The name of the contact's company.</span></span>|
|<span data-ttu-id="a48bc-159">department</span><span class="sxs-lookup"><span data-stu-id="a48bc-159">department</span></span>|<span data-ttu-id="a48bc-160">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-160">String</span></span>|<span data-ttu-id="a48bc-161">Отдел контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-161">The contact's department.</span></span>|
|<span data-ttu-id="a48bc-162">displayName</span><span class="sxs-lookup"><span data-stu-id="a48bc-162">displayName</span></span>|<span data-ttu-id="a48bc-163">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-163">String</span></span>|<span data-ttu-id="a48bc-164">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-164">The contact's display name.</span></span>|
|<span data-ttu-id="a48bc-165">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="a48bc-165">emailAddresses</span></span>|<span data-ttu-id="a48bc-166">Коллекция [EmailAddress](../resources/emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="a48bc-166">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="a48bc-167">Электронные адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-167">The contact's email addresses.</span></span>|
|<span data-ttu-id="a48bc-168">fileAs</span><span class="sxs-lookup"><span data-stu-id="a48bc-168">fileAs</span></span>|<span data-ttu-id="a48bc-169">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-169">String</span></span>|<span data-ttu-id="a48bc-170">Имя, под которым хранится контакт.</span><span class="sxs-lookup"><span data-stu-id="a48bc-170">The name the contact is filed under.</span></span>|
|<span data-ttu-id="a48bc-171">generation</span><span class="sxs-lookup"><span data-stu-id="a48bc-171">generation</span></span>|<span data-ttu-id="a48bc-172">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-172">String</span></span>|<span data-ttu-id="a48bc-173">Поколение контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-173">The contact's generation.</span></span>|
|<span data-ttu-id="a48bc-174">givenName</span><span class="sxs-lookup"><span data-stu-id="a48bc-174">givenName</span></span>|<span data-ttu-id="a48bc-175">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-175">String</span></span>|<span data-ttu-id="a48bc-176">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-176">The contact's given name.</span></span>|
|<span data-ttu-id="a48bc-177">homeAddress</span><span class="sxs-lookup"><span data-stu-id="a48bc-177">homeAddress</span></span>|[<span data-ttu-id="a48bc-178">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="a48bc-178">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="a48bc-179">Домашний адрес контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-179">The contact's home address.</span></span>|
|<span data-ttu-id="a48bc-180">homePhones</span><span class="sxs-lookup"><span data-stu-id="a48bc-180">homePhones</span></span>|<span data-ttu-id="a48bc-181">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a48bc-181">String collection</span></span>|<span data-ttu-id="a48bc-182">Номера домашнего телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-182">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="a48bc-183">imAddresses</span><span class="sxs-lookup"><span data-stu-id="a48bc-183">imAddresses</span></span>|<span data-ttu-id="a48bc-184">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-184">String</span></span>|<span data-ttu-id="a48bc-185">Адреса контакта для обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="a48bc-185">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="a48bc-186">initials</span><span class="sxs-lookup"><span data-stu-id="a48bc-186">initials</span></span>|<span data-ttu-id="a48bc-187">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-187">String</span></span>|<span data-ttu-id="a48bc-188">Инициалы контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-188">The contact's initials.</span></span>|
|<span data-ttu-id="a48bc-189">jobTitle</span><span class="sxs-lookup"><span data-stu-id="a48bc-189">jobTitle</span></span>|<span data-ttu-id="a48bc-190">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-190">String</span></span>|<span data-ttu-id="a48bc-191">Должность контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-191">The contact’s job title.</span></span>|
|<span data-ttu-id="a48bc-192">manager</span><span class="sxs-lookup"><span data-stu-id="a48bc-192">manager</span></span>|<span data-ttu-id="a48bc-193">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-193">String</span></span>|<span data-ttu-id="a48bc-194">Имя руководителя контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-194">The name of the contact's manager.</span></span>
|<span data-ttu-id="a48bc-195">middleName</span><span class="sxs-lookup"><span data-stu-id="a48bc-195">middleName</span></span>|<span data-ttu-id="a48bc-196">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-196">String</span></span>|<span data-ttu-id="a48bc-197">Отчество контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-197">The contact's middle name.</span></span>|
|<span data-ttu-id="a48bc-198">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="a48bc-198">mobilePhone</span></span>|<span data-ttu-id="a48bc-199">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-199">String</span></span>|<span data-ttu-id="a48bc-200">Номер мобильного телефона контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-200">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="a48bc-201">nickName</span><span class="sxs-lookup"><span data-stu-id="a48bc-201">nickName</span></span>|<span data-ttu-id="a48bc-202">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-202">String</span></span>|<span data-ttu-id="a48bc-203">Псевдоним контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-203">The contact's nickname.</span></span>|
|<span data-ttu-id="a48bc-204">officeLocation</span><span class="sxs-lookup"><span data-stu-id="a48bc-204">officeLocation</span></span>|<span data-ttu-id="a48bc-205">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-205">String</span></span>|<span data-ttu-id="a48bc-206">Расположение офиса контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-206">The location of the contact's office.</span></span>|
|<span data-ttu-id="a48bc-207">otherAddress</span><span class="sxs-lookup"><span data-stu-id="a48bc-207">otherAddress</span></span>|[<span data-ttu-id="a48bc-208">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="a48bc-208">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="a48bc-209">Другие адреса контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-209">Other addresses for the contact.</span></span>|
|<span data-ttu-id="a48bc-210">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="a48bc-210">parentFolderId</span></span>|<span data-ttu-id="a48bc-211">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-211">String</span></span>|<span data-ttu-id="a48bc-212">Идентификатор родительской папки контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-212">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="a48bc-213">personalNotes</span><span class="sxs-lookup"><span data-stu-id="a48bc-213">personalNotes</span></span>|<span data-ttu-id="a48bc-214">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-214">String</span></span>|<span data-ttu-id="a48bc-215">Заметки пользователя о контакте.</span><span class="sxs-lookup"><span data-stu-id="a48bc-215">The user's notes about the contact.</span></span>|
|<span data-ttu-id="a48bc-216">profession</span><span class="sxs-lookup"><span data-stu-id="a48bc-216">profession</span></span>|<span data-ttu-id="a48bc-217">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-217">String</span></span>|<span data-ttu-id="a48bc-218">Профессия контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-218">The contact's profession.</span></span>|
|<span data-ttu-id="a48bc-219">spouseName</span><span class="sxs-lookup"><span data-stu-id="a48bc-219">spouseName</span></span>|<span data-ttu-id="a48bc-220">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-220">String</span></span>|<span data-ttu-id="a48bc-221">Имя супруга или супруги контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-221">The name of the contact's spouse.</span></span>|
|<span data-ttu-id="a48bc-222">surname</span><span class="sxs-lookup"><span data-stu-id="a48bc-222">surname</span></span>|<span data-ttu-id="a48bc-223">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-223">String</span></span>|<span data-ttu-id="a48bc-224">Фамилия контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-224">The contact's surname.</span></span>|
|<span data-ttu-id="a48bc-225">title</span><span class="sxs-lookup"><span data-stu-id="a48bc-225">title</span></span>|<span data-ttu-id="a48bc-226">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-226">String</span></span>|<span data-ttu-id="a48bc-227">Звание контакта.</span><span class="sxs-lookup"><span data-stu-id="a48bc-227">The contact's title.</span></span>|
|<span data-ttu-id="a48bc-228">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="a48bc-228">yomiCompanyName</span></span>|<span data-ttu-id="a48bc-229">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-229">String</span></span>|<span data-ttu-id="a48bc-p106">Название компании контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a48bc-p106">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="a48bc-232">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="a48bc-232">yomiGivenName</span></span>|<span data-ttu-id="a48bc-233">String</span><span class="sxs-lookup"><span data-stu-id="a48bc-233">String</span></span>|<span data-ttu-id="a48bc-p107">Имя контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a48bc-p107">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="a48bc-236">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="a48bc-236">yomiSurname</span></span>|<span data-ttu-id="a48bc-237">Строка</span><span class="sxs-lookup"><span data-stu-id="a48bc-237">String</span></span>|<span data-ttu-id="a48bc-p108">Фамилия контакта, записанная так, как она звучит по-японски. Это необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a48bc-p108">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="a48bc-240">Отклик</span><span class="sxs-lookup"><span data-stu-id="a48bc-240">Response</span></span>

<span data-ttu-id="a48bc-241">В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [contact](../resources/contact.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a48bc-241">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a48bc-242">Пример</span><span class="sxs-lookup"><span data-stu-id="a48bc-242">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a48bc-243">Запрос</span><span class="sxs-lookup"><span data-stu-id="a48bc-243">Request</span></span>
<span data-ttu-id="a48bc-244">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a48bc-244">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="a48bc-245">Ответ</span><span class="sxs-lookup"><span data-stu-id="a48bc-245">Response</span></span>
<span data-ttu-id="a48bc-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a48bc-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "businessHomePage": "http://www.contoso.com",
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
