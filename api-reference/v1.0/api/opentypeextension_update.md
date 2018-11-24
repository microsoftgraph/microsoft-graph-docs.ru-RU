# <a name="update-open-extension"></a><span data-ttu-id="ea669-101">Обновление открытого расширения</span><span class="sxs-lookup"><span data-stu-id="ea669-101">Update open extension</span></span>

<span data-ttu-id="ea669-102">Обновление открытого расширения (объекта [openTypeExtension](../resources/openTypeExtension.md)) с использованием свойств, указанных в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="ea669-102">Update an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) with the properties in the request body:</span></span>

- <span data-ttu-id="ea669-103">Если свойство в теле запроса совпадает с именем существующего свойства в расширении, то данные в расширении будут обновлены.</span><span class="sxs-lookup"><span data-stu-id="ea669-103">If a property in the request body matches the name of an existing property in the extension, the data in the extension is updated.</span></span>
- <span data-ttu-id="ea669-104">В противном случае это свойство и его данные будут добавлены в расширение.</span><span class="sxs-lookup"><span data-stu-id="ea669-104">Otherwise that property and its data are added to the extension.</span></span> 

<span data-ttu-id="ea669-105">Данные в расширении могут относиться к элементарным типам или массивам элементарных типов.</span><span class="sxs-lookup"><span data-stu-id="ea669-105">The data in an extension can be primitive types, or arrays of primitive types.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea669-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea669-106">Permissions</span></span>

<span data-ttu-id="ea669-107">В зависимости от разрешений и ресурсов, данное расширение имени файла, созданного на тип (делегированные или приложение) запрошенный, разрешение, указанное в следующей таблице минимальными правами требуется для вызова этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="ea669-107">Depending on the resource that the extension was created in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="ea669-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ea669-108">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="ea669-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="ea669-109">Supported resource</span></span> | <span data-ttu-id="ea669-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea669-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ea669-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea669-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea669-112">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ea669-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="ea669-113">device</span><span class="sxs-lookup"><span data-stu-id="ea669-113">device</span></span>](../resources/device.md) | <span data-ttu-id="ea669-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ea669-114">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="ea669-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ea669-115">Not supported</span></span> | <span data-ttu-id="ea669-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea669-116">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="ea669-117">event</span><span class="sxs-lookup"><span data-stu-id="ea669-117">event</span></span>](../resources/event.md) | <span data-ttu-id="ea669-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea669-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="ea669-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea669-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="ea669-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea669-120">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="ea669-121">group</span><span class="sxs-lookup"><span data-stu-id="ea669-121">group</span></span>](../resources/group.md) | <span data-ttu-id="ea669-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea669-122">Group.ReadWrite.All</span></span> | <span data-ttu-id="ea669-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ea669-123">Not supported</span></span> | <span data-ttu-id="ea669-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea669-124">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="ea669-125">[event](../resources/event.md) для групп</span><span class="sxs-lookup"><span data-stu-id="ea669-125">[group event](../resources/event.md)</span></span> | <span data-ttu-id="ea669-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea669-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="ea669-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ea669-127">Not supported</span></span> | <span data-ttu-id="ea669-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ea669-128">Not supported</span></span> |
| <span data-ttu-id="ea669-129">[post](../resources/post.md) для групп</span><span class="sxs-lookup"><span data-stu-id="ea669-129">[group post](../resources/post.md)</span></span> | <span data-ttu-id="ea669-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea669-130">Group.ReadWrite.All</span></span> | <span data-ttu-id="ea669-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ea669-131">Not supported</span></span> | <span data-ttu-id="ea669-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea669-132">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="ea669-133">message</span><span class="sxs-lookup"><span data-stu-id="ea669-133">message</span></span>](../resources/message.md) | <span data-ttu-id="ea669-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea669-134">Mail.ReadWrite</span></span> | <span data-ttu-id="ea669-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea669-135">Mail.ReadWrite</span></span> | <span data-ttu-id="ea669-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea669-136">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="ea669-137">organization</span><span class="sxs-lookup"><span data-stu-id="ea669-137">organization</span></span>](../resources/organization.md) | <span data-ttu-id="ea669-138">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ea669-138">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="ea669-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ea669-139">Not supported</span></span> | <span data-ttu-id="ea669-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ea669-140">Not supported</span></span> |
| <span data-ttu-id="ea669-141">[contact](../resources/contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="ea669-141">[personal contact](../resources/contact.md)</span></span> | <span data-ttu-id="ea669-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea669-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="ea669-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea669-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="ea669-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea669-144">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="ea669-145">user</span><span class="sxs-lookup"><span data-stu-id="ea669-145">user</span></span>](../resources/user.md) | <span data-ttu-id="ea669-146">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea669-146">User.ReadWrite.All</span></span> | <span data-ttu-id="ea669-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea669-147">User.ReadWrite</span></span> | <span data-ttu-id="ea669-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea669-148">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea669-149">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea669-149">HTTP request</span></span>
<span data-ttu-id="ea669-150">В запросе идентифицируйте экземпляр ресурса, воспользуйтесь свойством навигации **extensions** этого экземпляра, чтобы определить расширение, и укажите метод `PATCH` для этого экземпляра расширения.</span><span class="sxs-lookup"><span data-stu-id="ea669-150">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `PATCH` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/extensions/{extensionId}
PATCH /groups/{id}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
PATCH /organization/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/extensions/{extensionId}
```

><span data-ttu-id="ea669-p102">**Примечание.** В приведенном выше синтаксисе показаны некоторые распространенные способы определения экземпляра ресурса, чье расширение нужно обновить. Все другие варианты синтаксиса, позволяющие определить эти экземпляры ресурса, поддерживают обновление открытых расширений этих экземпляров подобным образом.</span><span class="sxs-lookup"><span data-stu-id="ea669-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to update an extension in it. All other syntax that allows you to identify these resource instances supports updating open extensions in them in a similar way.</span></span>

<span data-ttu-id="ea669-153">См. раздел [Тело запроса](#request-body) о том, как включить в тело запроса пользовательские данные для изменения или дополнения этого расширения.</span><span class="sxs-lookup"><span data-stu-id="ea669-153">See the [Request body](#request-body) section about including in the request body any custom data to change or add to that extension.</span></span>


## <a name="path-parameters"></a><span data-ttu-id="ea669-154">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="ea669-154">Path parameters</span></span>
|<span data-ttu-id="ea669-155">Параметр</span><span class="sxs-lookup"><span data-stu-id="ea669-155">Parameter</span></span>|<span data-ttu-id="ea669-156">Тип</span><span class="sxs-lookup"><span data-stu-id="ea669-156">Type</span></span>|<span data-ttu-id="ea669-157">Описание</span><span class="sxs-lookup"><span data-stu-id="ea669-157">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ea669-158">id</span><span class="sxs-lookup"><span data-stu-id="ea669-158">id</span></span>|<span data-ttu-id="ea669-159">строка</span><span class="sxs-lookup"><span data-stu-id="ea669-159">string</span></span>|<span data-ttu-id="ea669-p103">Уникальный идентификатор экземпляра в соответствующей коллекции. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea669-p103">A unique identifier for an instance of the corresponding collection. Required.</span></span>|
|<span data-ttu-id="ea669-162">extensionId</span><span class="sxs-lookup"><span data-stu-id="ea669-162">extensionId</span></span>|<span data-ttu-id="ea669-163">string</span><span class="sxs-lookup"><span data-stu-id="ea669-163">string</span></span>|<span data-ttu-id="ea669-p104">Этот параметр может быть именем расширения, которое представляет собой уникальный текстовый идентификатор для расширения, либо полным именем, в котором сцеплены тип расширения и уникальный текстовый идентификатор. Полное имя возвращается в свойстве `id` при создании расширения. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea669-p104">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="ea669-167">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea669-167">Request headers</span></span>
| <span data-ttu-id="ea669-168">Имя</span><span class="sxs-lookup"><span data-stu-id="ea669-168">Name</span></span>       | <span data-ttu-id="ea669-169">Значение</span><span class="sxs-lookup"><span data-stu-id="ea669-169">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ea669-170">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea669-170">Authorization</span></span> | <span data-ttu-id="ea669-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea669-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ea669-173">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ea669-173">Content-Type</span></span> | <span data-ttu-id="ea669-174">application/json</span><span class="sxs-lookup"><span data-stu-id="ea669-174">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea669-175">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ea669-175">Request body</span></span>

<span data-ttu-id="ea669-p106">Задайте основной текст JSON объекта [openTypeExtension](../resources/openTypeExtension.md) с указанными ниже обязательными парами имя-значение и любыми пользовательскими данными, которые необходимо изменить или добавить в это расширение. Полезные данные JSON могут иметь простой тип или представлять собой массив элементов простого типа.</span><span class="sxs-lookup"><span data-stu-id="ea669-p106">Provide a JSON body of an [openTypeExtension](../resources/openTypeExtension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="ea669-178">Имя</span><span class="sxs-lookup"><span data-stu-id="ea669-178">Name</span></span>       | <span data-ttu-id="ea669-179">Значение</span><span class="sxs-lookup"><span data-stu-id="ea669-179">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ea669-180">@odata.type</span><span class="sxs-lookup"><span data-stu-id="ea669-180">@odata.type</span></span> | <span data-ttu-id="ea669-181">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="ea669-181">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="ea669-182">extensionName</span><span class="sxs-lookup"><span data-stu-id="ea669-182">extensionName</span></span> | <span data-ttu-id="ea669-183">%уникальная_строка%</span><span class="sxs-lookup"><span data-stu-id="ea669-183">%unique_string%</span></span> |

## <a name="response"></a><span data-ttu-id="ea669-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea669-184">Response</span></span>

<span data-ttu-id="ea669-185">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [openTypeExtension](../resources/openTypeExtension.md).</span><span class="sxs-lookup"><span data-stu-id="ea669-185">If successful, this method returns a `200 OK` response code and the updated [openTypeExtension](../resources/openTypeExtension.md) object.</span></span>


## <a name="example"></a><span data-ttu-id="ea669-186">Пример</span><span class="sxs-lookup"><span data-stu-id="ea669-186">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="ea669-187">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="ea669-187">Request 1</span></span>

<span data-ttu-id="ea669-p107">В первом примере показано, как обновить расширение в сообщении. Изначально расширение представлено указанными ниже полезными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="ea669-p107">The first example shows how to update an extension in a message. The extension is initially represented by the following JSON payload:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

<span data-ttu-id="ea669-190">Вы можете ссылаться на расширение по его имени:</span><span class="sxs-lookup"><span data-stu-id="ea669-190">You can reference the extension by its name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="ea669-191">Кроме того, вы можете ссылаться на расширение по его полному имени:</span><span class="sxs-lookup"><span data-stu-id="ea669-191">Or you can reference the extension by its fully qualified name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

<span data-ttu-id="ea669-192">Для обновления указанного выше расширения используйте любой пример запроса и приведенный ниже тело запроса следующими способами:</span><span class="sxs-lookup"><span data-stu-id="ea669-192">You can use either example request and the following request body to update the above extension by:</span></span>
- <span data-ttu-id="ea669-193">изменив значение параметра `companyName` с `Wingtip Toys` на `Wingtip Toys (USA)`;</span><span class="sxs-lookup"><span data-stu-id="ea669-193">Changing `companyName` from `Wingtip Toys` to `Wingtip Toys (USA)`</span></span>
- <span data-ttu-id="ea669-194">изменив значение параметра `dealValue` с `500050` на `500100`; `500100`</span><span class="sxs-lookup"><span data-stu-id="ea669-194">Changing `dealValue` from `500050` to `500100`</span></span>
- <span data-ttu-id="ea669-195">добавив новые данные в качестве пользовательского свойства `updated`.</span><span class="sxs-lookup"><span data-stu-id="ea669-195">Adding new data as the custom property `updated`</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.type": "microsoft.graph.openTypeExtension",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": "500100",
    "expirationDate": "2015-12-03T10:00:00.000Z",
    "updated": "2015-10-29T11:00:00.000Z"
} 
```


#### <a name="response-1"></a><span data-ttu-id="ea669-196">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="ea669-196">Response 1</span></span>

<span data-ttu-id="ea669-197">Вот отклик, который не зависит от способа, которым вы ссылаетесь на расширение.</span><span class="sxs-lookup"><span data-stu-id="ea669-197">Here is the response which is the same regardless of the way used to reference the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": 500100,
    "expirationDate": "2015-12-03T10:00:00Z",
    "updated": "2015-10-29T11:00:00.000Z"
}
```

****

#### <a name="request-2"></a><span data-ttu-id="ea669-198">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="ea669-198">Request 2</span></span>

<span data-ttu-id="ea669-p108">Во втором примере показано, как обновить расширение в публикации группы. Изначально расширение представлено указанными ниже полезными данными JSON, в котором параметр `expirationDate` имеет значение `2015-07-03T13:04:00Z`:</span><span class="sxs-lookup"><span data-stu-id="ea669-p108">The second example shows how to update an extension in a group post. The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2015-07-03T13:04:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<span data-ttu-id="ea669-201">Ниже приведен запрос и тело запроса для изменения значения параметра `expirationDate` на `2016-07-30T11:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="ea669-201">The following is the request and request body to change the `expirationDate` to `2016-07-30T11:00:00Z`:</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate"],
  "name": "update_opentypeextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate
Content-type: application/json

{
   "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
   "extensionName": "Com.Contoso.Estimate",
   "companyName": "Contoso",
   "expirationDate": "2016-07-30T11:00:00.000Z",
   "DealValue": 1010100,
   "topPicks": [
       "Employees only",
       "Add spouse or guest",
       "Add family"
    ]
}
```

#### <a name="response-2"></a><span data-ttu-id="ea669-202">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="ea669-202">Response 2</span></span>

<span data-ttu-id="ea669-203">Вот отклик для второго примера, в котором отображается обновленный параметр `expirationDate` в расширении.</span><span class="sxs-lookup"><span data-stu-id="ea669-203">Here is the response of the second example which shows the updated `expirationDate` in the extension.</span></span>

<!-- {  
  "blockType": "ignored",  
  "truncated": true,  
  "@odata.type": "microsoft.graph.openTypeExtension"  
} --> 
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2016-07-30T11:00:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
} -->
