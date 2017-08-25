# <a name="create-open-extension"></a><span data-ttu-id="96413-101">Создание открытого расширения</span><span class="sxs-lookup"><span data-stu-id="96413-101">Create open extension</span></span>

<span data-ttu-id="96413-102">Создание открытого расширения (объекта [openTypeExtension](../resources/openTypeExtension.md)) и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.</span><span class="sxs-lookup"><span data-stu-id="96413-102">Create an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) and add custom properties in a new or existing instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="96413-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96413-103">Permissions</span></span>

<span data-ttu-id="96413-p101">Для вызова этого API требуется одно из указанных ниже разрешений (в зависимости от ресурса, в котором создается расширение). Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="96413-p101">One of the following permissions is required to call this API, depending on the resource you're creating the extension in. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="96413-106">**Поддерживаемый ресурс**</span><span class="sxs-lookup"><span data-stu-id="96413-106">**Supported resource**</span></span>|<span data-ttu-id="96413-107">**Разрешение**</span><span class="sxs-lookup"><span data-stu-id="96413-107">**Permission**</span></span>|<span data-ttu-id="96413-108">**Поддерживаемый ресурс**</span><span class="sxs-lookup"><span data-stu-id="96413-108">**Supported resource**</span></span>|<span data-ttu-id="96413-109">**Разрешение**</span><span class="sxs-lookup"><span data-stu-id="96413-109">**Permission**</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="96413-110">device</span><span class="sxs-lookup"><span data-stu-id="96413-110">device</span></span>](../resources/device.md) | <span data-ttu-id="96413-111">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96413-111">Device.ReadWrite.All</span></span> | [<span data-ttu-id="96413-112">event</span><span class="sxs-lookup"><span data-stu-id="96413-112">event</span></span>](../resources/event.md) | <span data-ttu-id="96413-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96413-113">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="96413-114">group</span><span class="sxs-lookup"><span data-stu-id="96413-114">group</span></span>](../resources/group.md) | <span data-ttu-id="96413-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96413-115">Group.ReadWrite.All</span></span> | <span data-ttu-id="96413-116">[event](../resources/event.md) для групп</span><span class="sxs-lookup"><span data-stu-id="96413-116">[group event](../resources/event.md)</span></span> | <span data-ttu-id="96413-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96413-117">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="96413-118">[post](../resources/post.md) для групп</span><span class="sxs-lookup"><span data-stu-id="96413-118">[group post](../resources/post.md)</span></span> | <span data-ttu-id="96413-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96413-119">Group.ReadWrite.All</span></span> | [<span data-ttu-id="96413-120">message</span><span class="sxs-lookup"><span data-stu-id="96413-120">message</span></span>](../resources/message.md) | <span data-ttu-id="96413-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96413-121">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="96413-122">organization</span><span class="sxs-lookup"><span data-stu-id="96413-122">organization</span></span>](../resources/organization.md) | <span data-ttu-id="96413-123">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="96413-123">Directory.AccessAsUser.All</span></span> | [<span data-ttu-id="96413-124">contact</span><span class="sxs-lookup"><span data-stu-id="96413-124">personal contact</span></span>](../resources/contact.md) (личный контакт) | <span data-ttu-id="96413-125">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96413-125">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="96413-126">user</span><span class="sxs-lookup"><span data-stu-id="96413-126">user</span></span>](../resources/user.md) | <span data-ttu-id="96413-127">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="96413-127">Directory.AccessAsUser.All</span></span> | | |
 
## <a name="http-request"></a><span data-ttu-id="96413-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96413-128">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="96413-129">Создание расширения в новом экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="96413-129">Create an extension in a new resource instance</span></span>

<span data-ttu-id="96413-130">Используйте такой же запрос REST, что и при создании экземпляра.</span><span class="sxs-lookup"><span data-stu-id="96413-130">Use the same REST request as creating the instance.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="96413-p102">**Примечание.** В приведенном выше синтаксисе показаны некоторые распространенные способы создания поддерживаемых экземпляров ресурса. Все другие варианты синтаксиса POST, позволяющие создавать эти экземпляры ресурса, поддерживают создание открытых расширений этих экземпляров подобным образом.</span><span class="sxs-lookup"><span data-stu-id="96413-p102">**Note:** The above syntax shows some common ways to create the supported resource instances. All other POST syntax that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="96413-133">В разделе [Тело запроса](#request-body) показано, как включить свойства нового экземпляра ресурса _и расширение_ в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="96413-133">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="96413-134">Создание расширения в существующем экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="96413-134">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="96413-135">Идентифицируйте экземпляр ресурса в запросе и выполните операцию `POST` для свойства навигации **extensions**.</span><span class="sxs-lookup"><span data-stu-id="96413-135">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

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

><span data-ttu-id="96413-p103">**Примечание.** В приведенном выше синтаксисе показаны некоторые распространенные способы определения экземпляра ресурса, чье расширение нужно создать. Все другие варианты синтаксиса, позволяющие определить эти экземпляры ресурса, поддерживают создание открытых расширений этих экземпляров подобным образом.</span><span class="sxs-lookup"><span data-stu-id="96413-p103">**Note:** The above syntax shows some common ways to identify a resource instance, in order to create an extension in it. All other syntax that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="96413-138">В разделе [Тело запроса](#request-body) показано, как включить _расширение_ в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="96413-138">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="parameters"></a><span data-ttu-id="96413-139">Параметры</span><span class="sxs-lookup"><span data-stu-id="96413-139">Parameters</span></span>
|<span data-ttu-id="96413-140">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="96413-140">**Parameter**</span></span>|<span data-ttu-id="96413-141">**Тип**</span><span class="sxs-lookup"><span data-stu-id="96413-141">**Type**</span></span>|<span data-ttu-id="96413-142">**Описание**</span><span class="sxs-lookup"><span data-stu-id="96413-142">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="96413-143">_Параметры URL-адреса_</span><span class="sxs-lookup"><span data-stu-id="96413-143">_URL parameters_</span></span>|
|<span data-ttu-id="96413-144">id</span><span class="sxs-lookup"><span data-stu-id="96413-144">id</span></span>|<span data-ttu-id="96413-145">string</span><span class="sxs-lookup"><span data-stu-id="96413-145">string</span></span>|<span data-ttu-id="96413-p104">Уникальный идентификатор объекта в соответствующей коллекции. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96413-p104">A unique identifier for an object in the corresponding collection. Required.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="96413-148">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96413-148">Request headers</span></span>
| <span data-ttu-id="96413-149">Имя</span><span class="sxs-lookup"><span data-stu-id="96413-149">Name</span></span>       | <span data-ttu-id="96413-150">Значение</span><span class="sxs-lookup"><span data-stu-id="96413-150">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="96413-151">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96413-151">Authorization</span></span> | <span data-ttu-id="96413-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96413-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96413-154">Content-Type</span><span class="sxs-lookup"><span data-stu-id="96413-154">Content-Type</span></span> | <span data-ttu-id="96413-155">application/json</span><span class="sxs-lookup"><span data-stu-id="96413-155">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="96413-156">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="96413-156">Request body</span></span>

<span data-ttu-id="96413-p106">Предоставьте описание объекта [openTypeExtension](../resources/openTypeExtension.md) в формате JSON с указанными ниже обязательными парами "имя-значение", а также дополнительными пользовательскими данными. Полезные данные JSON могут относиться к простому типу или представлять собой массив элементов простого типа.</span><span class="sxs-lookup"><span data-stu-id="96413-p106">Provide a JSON body of an [openTypeExtension](../resources/openTypeExtension.md), with the following required name-value pairs, and any additional custom data. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="96413-159">Имя</span><span class="sxs-lookup"><span data-stu-id="96413-159">Name</span></span>       | <span data-ttu-id="96413-160">Значение</span><span class="sxs-lookup"><span data-stu-id="96413-160">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="96413-161">@odata.type</span><span class="sxs-lookup"><span data-stu-id="96413-161">@odata.type</span></span> | <span data-ttu-id="96413-162">Microsoft.Graph.OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="96413-162">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="96413-163">extensionName</span><span class="sxs-lookup"><span data-stu-id="96413-163">extensionName</span></span> | <span data-ttu-id="96413-164">%уникальная_строка%</span><span class="sxs-lookup"><span data-stu-id="96413-164">%unique_string%</span></span> |

<span data-ttu-id="96413-165">При создании расширения в _новом_ экземпляре ресурса предоставьте не только объект **openTypeExtension**, но и представление JSON соответствующих свойств для создания этого экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="96413-165">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="96413-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="96413-166">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="96413-167">Код ответа</span><span class="sxs-lookup"><span data-stu-id="96413-167">Response code</span></span>
<span data-ttu-id="96413-168">В зависимости от операции, можно использовать код ответа `201 Created` или `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="96413-168">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="96413-p107">При создании расширения в той же операции, которая используется для создания экземпляра ресурса, успешно выполненная операция возвращает такой же код ответа, что и при создании экземпляра ресурса без расширения. Изучите соответствующие статьи о создании экземпляров, перечисленные [выше](#create-an-extension-in-a-new-resource-instance).</span><span class="sxs-lookup"><span data-stu-id="96413-p107">When creating an extension in the same operation as creating a resource instance, a successful operation returns the same response code as when the operation is used to create only the resource instance without the extension. Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

#### <a name="response-body"></a><span data-ttu-id="96413-171">Тело отклика</span><span class="sxs-lookup"><span data-stu-id="96413-171">Response body</span></span>
| <span data-ttu-id="96413-172">Сценарий</span><span class="sxs-lookup"><span data-stu-id="96413-172">Scenario</span></span>       | <span data-ttu-id="96413-173">Ресурс</span><span class="sxs-lookup"><span data-stu-id="96413-173">Resource</span></span>  | <span data-ttu-id="96413-174">Тело отклика</span><span class="sxs-lookup"><span data-stu-id="96413-174">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="96413-175">Создание расширения с явным созданием _нового_ экземпляра ресурса</span><span class="sxs-lookup"><span data-stu-id="96413-175">Creating an extension while explicitly creating a _new_ resource instance</span></span> | [<span data-ttu-id="96413-176">contact](../resources/contact.md), [event](../resources/event.md), [message</span><span class="sxs-lookup"><span data-stu-id="96413-176">contact](../resources/contact.md), [event](../resources/event.md), [message</span></span>](../resources/message.md) | <span data-ttu-id="96413-177">Включает новый экземпляр, дополненный объектом [openTypeExtension](../resources/openTypeExtension.md).</span><span class="sxs-lookup"><span data-stu-id="96413-177">Includes the new instance expanded with the [openTypeExtension](../resources/openTypeExtension.md) object.</span></span> |
| <span data-ttu-id="96413-178">Создание расширения с неявным созданием экземпляра ресурса</span><span class="sxs-lookup"><span data-stu-id="96413-178">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="96413-179">post</span><span class="sxs-lookup"><span data-stu-id="96413-179">post</span></span>](../resources/post.md) | <span data-ttu-id="96413-180">Ответ содержит только код ответа без текста.</span><span class="sxs-lookup"><span data-stu-id="96413-180">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="96413-181">Создание расширения в _существующем_ экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="96413-181">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="96413-182">Все поддерживаемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="96413-182">All supported resources</span></span> | <span data-ttu-id="96413-183">Включает объект **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="96413-183">Includes the **openTypeExtension** object.</span></span> |
 


## <a name="example"></a><span data-ttu-id="96413-184">Пример</span><span class="sxs-lookup"><span data-stu-id="96413-184">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="96413-185">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="96413-185">Request 1</span></span>

<span data-ttu-id="96413-p108">В первом примере сообщение и расширение создаются в одном запросе. Текст запроса включает следующие данные:</span><span class="sxs-lookup"><span data-stu-id="96413-p108">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="96413-188">Свойства **subject**, **body** и **toRecipients**, характерные для нового сообщения.</span><span class="sxs-lookup"><span data-stu-id="96413-188">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span> 
- <span data-ttu-id="96413-189">Данные для расширения:</span><span class="sxs-lookup"><span data-stu-id="96413-189">And for the extension:</span></span>

  - <span data-ttu-id="96413-190">Тип `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="96413-190">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
  - <span data-ttu-id="96413-191">Имя расширения "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="96413-191">The extension name "Com.Contoso.Referral".</span></span> 
  - <span data-ttu-id="96413-192">Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `expirationDate` и `dealValue`.</span><span class="sxs-lookup"><span data-stu-id="96413-192">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>  

<!-- {
  "blockType": "request",
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
      "@odata.type": "Microsoft.Graph.OpenTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="96413-193">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="96413-193">Response 1</span></span>

<span data-ttu-id="96413-p109">Ниже представлен отклик для первого примера. Текст отклика включает свойства нового сообщения и следующие данные для нового расширения:</span><span class="sxs-lookup"><span data-stu-id="96413-p109">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="96413-196">Свойство **id** с полным именем `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="96413-196">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span> 
- <span data-ttu-id="96413-197">Стандартное свойство **extensionName**, указанное в запросе.</span><span class="sxs-lookup"><span data-stu-id="96413-197">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="96413-198">Пользовательские данные из запроса, сохраненные в виде 3 настраиваемых свойств.</span><span class="sxs-lookup"><span data-stu-id="96413-198">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="96413-p110">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96413-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
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

##### <a name="request-2"></a><span data-ttu-id="96413-201">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="96413-201">Request 2</span></span>

<span data-ttu-id="96413-p111">Во втором примере показано создание расширения в указанном сообщении. Текст запроса включает следующие данные для расширения:</span><span class="sxs-lookup"><span data-stu-id="96413-p111">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="96413-204">Тип `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="96413-204">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="96413-205">Имя расширения "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="96413-205">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="96413-206">Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `dealValue` и `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="96413-206">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>  

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions

{ 
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension", 
  "extensionName" : "Com.Contoso.Referral", 
  "companyName" : "Wingtip Toys", 
  "dealValue" : 500050, 
  "expirationDate" : "2015-12-03T10:00:00.000Z" 
} 
```

##### <a name="response-2"></a><span data-ttu-id="96413-207">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="96413-207">Response 2</span></span>

<span data-ttu-id="96413-p112">Ниже представлен отклик для второго примера. Текст отклика включает следующие данные для нового расширения:</span><span class="sxs-lookup"><span data-stu-id="96413-p112">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="96413-210">Свойство по умолчанию **extensionName**.</span><span class="sxs-lookup"><span data-stu-id="96413-210">The default property **extensionName**.</span></span>
- <span data-ttu-id="96413-211">Свойство **id** с полным именем `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="96413-211">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span> 
- <span data-ttu-id="96413-212">Сохраняемые пользовательские данные.</span><span class="sxs-lookup"><span data-stu-id="96413-212">The custom data to be stored.</span></span>  

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
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

##### <a name="request-3"></a><span data-ttu-id="96413-213">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="96413-213">Request 3</span></span>

<span data-ttu-id="96413-p113">В третьем примере показано создание расширения в указанном событии группы. Текст запроса включает следующие данные для расширения:</span><span class="sxs-lookup"><span data-stu-id="96413-p113">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="96413-216">Тип `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="96413-216">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="96413-217">Имя расширения "Com.Contoso.Deal".</span><span class="sxs-lookup"><span data-stu-id="96413-217">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="96413-218">Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `dealValue` и `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="96413-218">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>  

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl17IsAAA=')/extensions 

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

##### <a name="response-3"></a><span data-ttu-id="96413-219">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="96413-219">Response 3</span></span>

<span data-ttu-id="96413-220">Ниже представлен отклик из третьего примера.</span><span class="sxs-lookup"><span data-stu-id="96413-220">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

##### <a name="request-4"></a><span data-ttu-id="96413-221">Запрос 4</span><span class="sxs-lookup"><span data-stu-id="96413-221">Request 4</span></span>

<span data-ttu-id="96413-p114">В четвертом примере показано создание расширения в новой записи группы с помощью одного вызова действия **reply** для существующей записи группы. Действие **reply** создает запись и внедряет в нее новое расширение. Текст запроса включает свойство **post**, которое, в свою очередь, содержит свойство **body** новой записи и следующие данные для нового расширения:</span><span class="sxs-lookup"><span data-stu-id="96413-p114">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="96413-225">Тип `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="96413-225">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="96413-226">Имя расширения "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="96413-226">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="96413-227">Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `expirationDate` и массив строк `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="96413-227">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=')/microsoft.graph.reply 

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

##### <a name="response-4"></a><span data-ttu-id="96413-228">Отклик 4</span><span class="sxs-lookup"><span data-stu-id="96413-228">Response 4</span></span>

<span data-ttu-id="96413-p115">Ниже представлен отклик из четвертого примера. При успешном создании расширения в новой записи группы возвращается только код отклика HTTP 202.</span><span class="sxs-lookup"><span data-stu-id="96413-p115">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

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

##### <a name="request-5"></a><span data-ttu-id="96413-231">Запрос 5</span><span class="sxs-lookup"><span data-stu-id="96413-231">Request 5</span></span>

<span data-ttu-id="96413-p116">В пятом примере показано создание расширения в новой записи группы с помощью той же операции POST, которая создает беседу. Операция POST создает беседу, цепочку и запись, а также внедряет в эту запись новое расширение. Текст отклика включает свойства **Topic** и **Threads**, а также дочерний объект **post** для новой беседы. Объект **post**, в свою очередь, содержит свойство **body** новой записи и следующие данные расширения:</span><span class="sxs-lookup"><span data-stu-id="96413-p116">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="96413-236">Тип `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="96413-236">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="96413-237">Имя расширения "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="96413-237">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="96413-238">Дополнительные данные, хранящиеся в виде 3 настраиваемых свойств в полезных данных JSON: `companyName`, `expirationDate` и массив строк `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="96413-238">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations

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

##### <a name="response-5"></a><span data-ttu-id="96413-239">Отклик 5</span><span class="sxs-lookup"><span data-stu-id="96413-239">Response 5</span></span>

<span data-ttu-id="96413-p117">Ниже представлен отклик из пятого примера, содержащий новую беседу и идентификатор цепочки. Эта новая цепочка содержит автоматически созданную запись, включающую новое расширение.</span><span class="sxs-lookup"><span data-stu-id="96413-p117">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span> 

<span data-ttu-id="96413-p118">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96413-p118">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="96413-p119">Чтобы получить новое расширение, сначала [получите все записи](../api/conversationthread_list_posts.md) из цепочки. Изначально в ней должна быть только одна запись. Затем примените идентификатор записи и имя расширения `Com.Contoso.Benefits`, чтобы [получить расширение](../api/opentypeextension_get.md).</span><span class="sxs-lookup"><span data-stu-id="96413-p119">To get the new extension, first [get all the posts](../api/conversationthread_list_posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension_get.md).</span></span>

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
