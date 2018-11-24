# <a name="create-open-extension"></a><span data-ttu-id="2a3ec-101">Создание открытого расширения</span><span class="sxs-lookup"><span data-stu-id="2a3ec-101">Create open extension</span></span>

<span data-ttu-id="2a3ec-102">Создание открытого расширения (объекта [openTypeExtension](../resources/openTypeExtension.md)) и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-102">Create an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) and add custom properties in a new or existing instance of a resource.</span></span>

> <span data-ttu-id="2a3ec-103">**Примечание:** При создании open расширения Outlook ресурсов, содержатся в разделе **относящиеся к Outlook** в разделе [Тип ресурса openTypeExtension](../resources/opentypeextension.md#outlook-specific-considerations).</span><span class="sxs-lookup"><span data-stu-id="2a3ec-103">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="2a3ec-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a3ec-104">Permissions</span></span>

<span data-ttu-id="2a3ec-105">В зависимости от разрешений и ресурсов, которое вы создаете расширения в тип (делегированные или приложение) запрошенный, разрешение, указанное в следующей таблице минимальными правами требуется для вызова этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-105">Depending on the resource you're creating the extension in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="2a3ec-106">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2a3ec-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="2a3ec-107">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="2a3ec-107">Supported resource</span></span> | <span data-ttu-id="2a3ec-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a3ec-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2a3ec-109">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a3ec-109">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a3ec-110">Для приложения</span><span class="sxs-lookup"><span data-stu-id="2a3ec-110">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="2a3ec-111">device</span><span class="sxs-lookup"><span data-stu-id="2a3ec-111">device</span></span>](../resources/device.md) | <span data-ttu-id="2a3ec-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2a3ec-112">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="2a3ec-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2a3ec-113">Not supported</span></span> | <span data-ttu-id="2a3ec-114">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a3ec-114">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="2a3ec-115">event</span><span class="sxs-lookup"><span data-stu-id="2a3ec-115">event</span></span>](../resources/event.md) | <span data-ttu-id="2a3ec-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a3ec-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="2a3ec-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a3ec-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="2a3ec-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a3ec-118">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="2a3ec-119">group</span><span class="sxs-lookup"><span data-stu-id="2a3ec-119">group</span></span>](../resources/group.md) | <span data-ttu-id="2a3ec-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a3ec-120">Group.ReadWrite.All</span></span> | <span data-ttu-id="2a3ec-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2a3ec-121">Not supported</span></span> | <span data-ttu-id="2a3ec-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a3ec-122">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="2a3ec-123">[event](../resources/event.md) для групп</span><span class="sxs-lookup"><span data-stu-id="2a3ec-123">[group event](../resources/event.md)</span></span> | <span data-ttu-id="2a3ec-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a3ec-124">Group.ReadWrite.All</span></span> | <span data-ttu-id="2a3ec-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2a3ec-125">Not supported</span></span> | <span data-ttu-id="2a3ec-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2a3ec-126">Not supported</span></span> |
| <span data-ttu-id="2a3ec-127">[post](../resources/post.md) для групп</span><span class="sxs-lookup"><span data-stu-id="2a3ec-127">[group post](../resources/post.md)</span></span> | <span data-ttu-id="2a3ec-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a3ec-128">Group.ReadWrite.All</span></span> | <span data-ttu-id="2a3ec-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2a3ec-129">Not supported</span></span> | <span data-ttu-id="2a3ec-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a3ec-130">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="2a3ec-131">message</span><span class="sxs-lookup"><span data-stu-id="2a3ec-131">message</span></span>](../resources/message.md) | <span data-ttu-id="2a3ec-132">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a3ec-132">Mail.ReadWrite</span></span> | <span data-ttu-id="2a3ec-133">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a3ec-133">Mail.ReadWrite</span></span> | <span data-ttu-id="2a3ec-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a3ec-134">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="2a3ec-135">organization</span><span class="sxs-lookup"><span data-stu-id="2a3ec-135">organization</span></span>](../resources/organization.md) | <span data-ttu-id="2a3ec-136">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2a3ec-136">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="2a3ec-137">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2a3ec-137">Not supported</span></span> | <span data-ttu-id="2a3ec-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2a3ec-138">Not supported</span></span> |
| <span data-ttu-id="2a3ec-139">[contact](../resources/contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="2a3ec-139">[personal contact](../resources/contact.md)</span></span> | <span data-ttu-id="2a3ec-140">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a3ec-140">Contacts.ReadWrite</span></span> | <span data-ttu-id="2a3ec-141">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a3ec-141">Contacts.ReadWrite</span></span> | <span data-ttu-id="2a3ec-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a3ec-142">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="2a3ec-143">user</span><span class="sxs-lookup"><span data-stu-id="2a3ec-143">user</span></span>](../resources/user.md) | <span data-ttu-id="2a3ec-144">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a3ec-144">User.ReadWrite.All</span></span> | <span data-ttu-id="2a3ec-145">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a3ec-145">User.ReadWrite</span></span> | <span data-ttu-id="2a3ec-146">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a3ec-146">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a3ec-147">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a3ec-147">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="2a3ec-148">Создание расширения в новом экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="2a3ec-148">Create an extension in a new resource instance</span></span>

<span data-ttu-id="2a3ec-149">Использование того же запроса REST, которая используется для создания экземпляра.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-149">Use the same REST request that you use to create the instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="2a3ec-150">**Примечание:** Этот синтаксис показаны наиболее распространенные способы создания экземпляров поддерживаемые ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-150">**Note:** This syntax shows some common ways to create the supported resource instances.</span></span> <span data-ttu-id="2a3ec-151">Все синтаксис POST, которые можно создавать экземпляры этих ресурсов поддерживает создание open расширения в их аналогичным образом.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-151">All other POST syntaxes that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="2a3ec-152">В разделе [Тело запроса](#request-body) показано, как включить свойства нового экземпляра ресурса _и расширение_ в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-152">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="2a3ec-153">Создание расширения в существующем экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="2a3ec-153">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="2a3ec-154">Идентифицируйте экземпляр ресурса в запросе и выполните операцию `POST` для свойства навигации **extensions**.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-154">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/extensions
POST /users/{id|userPrincipalName}/events/{id}/extensions
POST /groups/{id}/extensions
POST /groups/{id}/events/{id}/extensions
POST /groups/{id}/threads/{id}/posts/{id}/extensions
POST /users/{id|userPrincipalName}/messages/{id}/extensions
POST /organization/{id}/extensions
POST /users/{id|userPrincipalName}/contacts/{id}/extensions
POST /users/{id|userPrincipalName}/extensions
```

><span data-ttu-id="2a3ec-155">**Примечание:** Этот синтаксис показаны наиболее распространенные способы идентификации экземпляра ресурсов, чтобы создать расширение в его.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-155">**Note:** This syntax shows some common ways to identify a resource instance, in order to create an extension in it.</span></span> <span data-ttu-id="2a3ec-156">Все другие синтаксисы, позволяет легко идентифицировать экземпляры этих ресурсов поддерживает создание open расширений в их аналогичным образом.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-156">All other syntaxes that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="2a3ec-157">В разделе [Тело запроса](#request-body) показано, как включить _расширение_ в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-157">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="2a3ec-158">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="2a3ec-158">Path parameters</span></span>
|<span data-ttu-id="2a3ec-159">Параметр</span><span class="sxs-lookup"><span data-stu-id="2a3ec-159">Parameter</span></span>|<span data-ttu-id="2a3ec-160">Тип</span><span class="sxs-lookup"><span data-stu-id="2a3ec-160">Type</span></span>|<span data-ttu-id="2a3ec-161">Описание</span><span class="sxs-lookup"><span data-stu-id="2a3ec-161">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2a3ec-162">id</span><span class="sxs-lookup"><span data-stu-id="2a3ec-162">id</span></span>|<span data-ttu-id="2a3ec-163">строка</span><span class="sxs-lookup"><span data-stu-id="2a3ec-163">string</span></span>|<span data-ttu-id="2a3ec-p104">Уникальный идентификатор объекта в соответствующей коллекции. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-p104">A unique identifier for an object in the corresponding collection. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2a3ec-166">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a3ec-166">Request headers</span></span>

| <span data-ttu-id="2a3ec-167">Имя</span><span class="sxs-lookup"><span data-stu-id="2a3ec-167">Name</span></span>       | <span data-ttu-id="2a3ec-168">Значение</span><span class="sxs-lookup"><span data-stu-id="2a3ec-168">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="2a3ec-169">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a3ec-169">Authorization</span></span> | <span data-ttu-id="2a3ec-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2a3ec-172">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a3ec-172">Content-Type</span></span> | <span data-ttu-id="2a3ec-173">application/json</span><span class="sxs-lookup"><span data-stu-id="2a3ec-173">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a3ec-174">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2a3ec-174">Request body</span></span>

<span data-ttu-id="2a3ec-p106">Предоставьте описание объекта [openTypeExtension](../resources/openTypeExtension.md) в формате JSON с указанными ниже обязательными парами "имя-значение", а также дополнительными пользовательскими данными. Полезные данные JSON могут относиться к простому типу или представлять собой массив элементов простого типа.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-p106">Provide a JSON body of an [openTypeExtension](../resources/openTypeExtension.md), with the following required name-value pairs, and any additional custom data. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="2a3ec-177">Имя</span><span class="sxs-lookup"><span data-stu-id="2a3ec-177">Name</span></span>       | <span data-ttu-id="2a3ec-178">Значение</span><span class="sxs-lookup"><span data-stu-id="2a3ec-178">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="2a3ec-179">@odata.type</span><span class="sxs-lookup"><span data-stu-id="2a3ec-179">@odata.type</span></span> | <span data-ttu-id="2a3ec-180">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="2a3ec-180">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="2a3ec-181">extensionName</span><span class="sxs-lookup"><span data-stu-id="2a3ec-181">extensionName</span></span> | <span data-ttu-id="2a3ec-182">%уникальная_строка%</span><span class="sxs-lookup"><span data-stu-id="2a3ec-182">%unique_string%</span></span> |

<span data-ttu-id="2a3ec-183">При создании расширения в _новом_ экземпляре ресурса предоставьте не только объект **openTypeExtension**, но и представление JSON соответствующих свойств для создания этого экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-183">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="2a3ec-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a3ec-184">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="2a3ec-185">Код ответа</span><span class="sxs-lookup"><span data-stu-id="2a3ec-185">Response code</span></span>

<span data-ttu-id="2a3ec-186">В зависимости от операции, можно использовать код ответа `201 Created` или `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-186">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="2a3ec-187">При создании расширения с помощью той же операции, которая используется для создания экземпляра ресурсов, операция возвращает один и тот же код ответа, который возвращается при использовании операции для создания экземпляра ресурсов без расширения.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-187">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension.</span></span>
<span data-ttu-id="2a3ec-188">Ссылки на соответствующие разделы для создания экземпляра как перечисленных [выше](#create-an-extension-in-a-new-resource-instance).</span><span class="sxs-lookup"><span data-stu-id="2a3ec-188">Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="2a3ec-189">Текст ответа</span><span class="sxs-lookup"><span data-stu-id="2a3ec-189">Response body</span></span>

| <span data-ttu-id="2a3ec-190">Сценарий</span><span class="sxs-lookup"><span data-stu-id="2a3ec-190">Scenario</span></span>       | <span data-ttu-id="2a3ec-191">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2a3ec-191">Resource</span></span>  | <span data-ttu-id="2a3ec-192">Тело отклика</span><span class="sxs-lookup"><span data-stu-id="2a3ec-192">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="2a3ec-193">Создание расширения с явным созданием _нового_ экземпляра ресурса</span><span class="sxs-lookup"><span data-stu-id="2a3ec-193">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="2a3ec-194">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="2a3ec-194">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="2a3ec-195">Включает новый экземпляр, дополненный объектом [openTypeExtension](../resources/openTypeExtension.md).</span><span class="sxs-lookup"><span data-stu-id="2a3ec-195">Includes the new instance expanded with the [openTypeExtension](../resources/openTypeExtension.md) object.</span></span> |
| <span data-ttu-id="2a3ec-196">Создание расширения с неявным созданием экземпляра ресурса</span><span class="sxs-lookup"><span data-stu-id="2a3ec-196">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="2a3ec-197">post</span><span class="sxs-lookup"><span data-stu-id="2a3ec-197">post</span></span>](../resources/post.md) | <span data-ttu-id="2a3ec-198">Ответ содержит только код ответа без текста.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-198">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="2a3ec-199">Создание расширения в _существующем_ экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="2a3ec-199">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="2a3ec-200">Все поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="2a3ec-200">All supported resources</span></span> | <span data-ttu-id="2a3ec-201">Включает объект **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-201">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="2a3ec-202">Пример</span><span class="sxs-lookup"><span data-stu-id="2a3ec-202">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="2a3ec-203">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="2a3ec-203">Request 1</span></span>

<span data-ttu-id="2a3ec-p108">В первом примере сообщение и расширение создаются в одном запросе. Текст запроса включает следующие данные:</span><span class="sxs-lookup"><span data-stu-id="2a3ec-p108">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="2a3ec-206">Свойства **subject**, **body** и **toRecipients**, характерные для нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-206">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="2a3ec-207">Данные для расширения:</span><span class="sxs-lookup"><span data-stu-id="2a3ec-207">And for the extension:</span></span>

  - <span data-ttu-id="2a3ec-208">Тип `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-208">The type `microsoft.graph.openTypeExtension`.</span></span>
  - <span data-ttu-id="2a3ec-209">Имя расширения "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="2a3ec-209">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="2a3ec-210">Дополнительные данные, хранимых в три настраиваемых свойств в полезных данных JSON: `companyName`, `expirationDate`, и `dealValue`.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-210">Additional data to be stored as three custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages

{
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "You should be proud!"
  },
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com"
      }
    }
  ],
  "extensions": [
    {
      "@odata.type": "microsoft.graph.openTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

### <a name="response-1"></a><span data-ttu-id="2a3ec-211">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="2a3ec-211">Response 1</span></span>

<span data-ttu-id="2a3ec-p109">Ниже представлен отклик для первого примера. Текст отклика включает свойства нового сообщения и следующие данные для нового расширения:</span><span class="sxs-lookup"><span data-stu-id="2a3ec-p109">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="2a3ec-214">Свойство **id** с полным именем `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-214">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="2a3ec-215">Стандартное свойство **extensionName**, указанное в запросе.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-215">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="2a3ec-216">Пользовательские данные из запроса, сохраненные в виде 3 настраиваемых свойств.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-216">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="2a3ec-p110">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')",
  "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj\"",
  "id": "AAMkAGEbs88AAB84uLuAAA=",
  "createdDateTime": "2015-10-30T03:03:43Z",
  "lastModifiedDateTime": "2015-10-30T03:03:43Z",
  "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj",
  "categories": [ ],
  "receivedDateTime": "2015-10-30T03:03:43Z",
  "sentDateTime": "2015-10-30T03:03:43Z",
  "hasAttachments": false,
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r
\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nYou should be proud!\r\n</body>\r
\n</html>\r\n"
  },
  "bodyPreview": "You should be proud!",
  "importance": "Normal",
  "parentFolderId": "AQMkAGEwAAAIBDwAAAA==",
  "sender": null,
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com",
        "name": "John Doe"
      }
    }
  ],
  "ccRecipients": [ ],
  "bccRecipients": [ ],
  "replyTo": [ ],
  "conversationId": "AAQkAGEFGugh3SVdMzzc=",
  "isDeliveryReceiptRequested": false,
  "isReadReceiptRequested": false,
  "isRead": true,
  "isDraft": true,
  "webLink": "https://outlook.office.com/owa/?
ItemID=AAMkAGEbs88AAB84uLuAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
  "inferenceClassification": "Focused",
  "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages
('AAMkAGEbs88AAB84uLuAAA%3D')/extensions",
  "extensions": [
    {
      "@odata.type": "#microsoft.graph.openTypeExtension",
      "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
      "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

****

### <a name="request-2"></a><span data-ttu-id="2a3ec-219">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="2a3ec-219">Request 2</span></span>

<span data-ttu-id="2a3ec-p111">Во втором примере показано создание расширения в указанном сообщении. Текст запроса включает следующие данные для расширения:</span><span class="sxs-lookup"><span data-stu-id="2a3ec-p111">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="2a3ec-222">Тип `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-222">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="2a3ec-223">Имя расширения "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="2a3ec-223">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="2a3ec-224">Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `dealValue` и `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-224">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```

### <a name="response-2"></a><span data-ttu-id="2a3ec-225">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="2a3ec-225">Response 2</span></span>

<span data-ttu-id="2a3ec-p112">Ниже представлен отклик для второго примера. Текст отклика включает следующие данные для нового расширения:</span><span class="sxs-lookup"><span data-stu-id="2a3ec-p112">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="2a3ec-228">Свойство по умолчанию **extensionName**.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-228">The default property **extensionName**.</span></span>
- <span data-ttu-id="2a3ec-229">Свойство **id** с полным именем `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-229">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="2a3ec-230">Сохраняемые пользовательские данные.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-230">The custom data to be stored.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

### <a name="request-3"></a><span data-ttu-id="2a3ec-231">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="2a3ec-231">Request 3</span></span>

<span data-ttu-id="2a3ec-p113">В третьем примере показано создание расширения в указанном событии группы. Текст запроса включает следующие данные для расширения:</span><span class="sxs-lookup"><span data-stu-id="2a3ec-p113">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="2a3ec-234">Тип `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-234">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="2a3ec-235">Имя расширения "Com.Contoso.Deal".</span><span class="sxs-lookup"><span data-stu-id="2a3ec-235">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="2a3ec-236">Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `dealValue` и `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-236">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

### <a name="response-3"></a><span data-ttu-id="2a3ec-237">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="2a3ec-237">Response 3</span></span>

<span data-ttu-id="2a3ec-238">Ниже представлен отклик из третьего примера.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-238">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

### <a name="request-4"></a><span data-ttu-id="2a3ec-239">Запрос 4</span><span class="sxs-lookup"><span data-stu-id="2a3ec-239">Request 4</span></span>

<span data-ttu-id="2a3ec-p114">В четвертом примере показано создание расширения в новой записи группы с помощью одного вызова действия **reply** для существующей записи группы. Действие **reply** создает запись и внедряет в нее новое расширение. Текст запроса включает свойство **post**, которое, в свою очередь, содержит свойство **body** новой записи и следующие данные для нового расширения:</span><span class="sxs-lookup"><span data-stu-id="2a3ec-p114">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="2a3ec-243">Тип `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-243">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="2a3ec-244">Имя расширения "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="2a3ec-244">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="2a3ec-245">Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `expirationDate` и массив строк `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-245">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=/reply

{
  "post": {
    "body": {
      "contentType": "html",
      "content": "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  "extensions": [
    {
      "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
      "extensionName": "Com.Contoso.HR",
      "companyName": "Contoso",
      "expirationDate": "2015-07-03T13:04:00.000Z",
      "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
      ]
    }
  ]
  }
}
```

### <a name="response-4"></a><span data-ttu-id="2a3ec-246">Отклик 4</span><span class="sxs-lookup"><span data-stu-id="2a3ec-246">Response 4</span></span>

<span data-ttu-id="2a3ec-p115">Ниже представлен отклик из четвертого примера. При успешном создании расширения в новой записи группы возвращается только код отклика HTTP 202.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-p115">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Content-type: text/plain
Content-Length: 0
```

****

### <a name="request-5"></a><span data-ttu-id="2a3ec-249">Запрос 5</span><span class="sxs-lookup"><span data-stu-id="2a3ec-249">Request 5</span></span>

<span data-ttu-id="2a3ec-p116">В пятом примере показано создание расширения в новой записи группы с помощью той же операции POST, которая создает беседу. Операция POST создает беседу, цепочку и запись, а также внедряет в эту запись новое расширение. Текст отклика включает свойства **Topic** и **Threads**, а также дочерний объект **post** для новой беседы. Объект **post**, в свою очередь, содержит свойство **body** новой записи и следующие данные расширения:</span><span class="sxs-lookup"><span data-stu-id="2a3ec-p116">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="2a3ec-254">Тип `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-254">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="2a3ec-255">Имя расширения "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="2a3ec-255">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="2a3ec-256">Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `expirationDate` и массив строк `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-256">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/conversations

{
  "Topic": "Does anyone have a second?",
  "Threads": [
    {
      "Posts": [
        {
          "Body": {
            "ContentType": "HTML",
            "Content": "This is urgent!"
          },
          "Extensions": [
            {
              "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
              "extensionName": "Com.Contoso.Benefits",
              "companyName": "Contoso",
              "expirationDate": "2016-08-03T11:00:00.000Z",
              "topPicks": [
                "Employees only",
                "Add spouse or guest",
                "Add family"
              ]
            }
          ]
        }
      ]
    }
  ]
}
```

### <a name="response-5"></a><span data-ttu-id="2a3ec-257">Отклик 5</span><span class="sxs-lookup"><span data-stu-id="2a3ec-257">Response 5</span></span>

<span data-ttu-id="2a3ec-p117">Ниже представлен отклик из пятого примера, содержащий новую беседу и идентификатор цепочки. Эта новая цепочка содержит автоматически созданную запись, включающую новое расширение.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-p117">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="2a3ec-p118">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a3ec-p118">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="2a3ec-p119">Чтобы получить новое расширение, сначала [получите все записи](../api/conversationthread_list_posts.md) из цепочки. Изначально в ней должна быть только одна запись. Затем примените идентификатор записи и имя расширения `Com.Contoso.Benefits`, чтобы [получить расширение](../api/opentypeextension_get.md).</span><span class="sxs-lookup"><span data-stu-id="2a3ec-p119">To get the new extension, first [get all the posts](../api/conversationthread_list_posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension_get.md).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations/$entity",
    "id": "AAQkADJToRlbJ5Mg7TFM7H-j3Y=",
    "threads@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations('AAQkADJToRlbJ5Mg7TFM7H-j3Y%3D')/threads",
    "threads": [
        {
            "id": "AAQkADJDtMUzsf_PdhAAswJOhGVsnkyDtMUzsf_Pdg=="
        }
    ]
}

```

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
