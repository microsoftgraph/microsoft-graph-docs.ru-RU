# <a name="delete-open-extension"></a><span data-ttu-id="f5648-101">Удаление открытого расширения</span><span class="sxs-lookup"><span data-stu-id="f5648-101">Delete open extension</span></span>

<span data-ttu-id="f5648-102">Удаление открытого расширения (объекта [openTypeExtension](../resources/openTypeExtension.md)) из указанного экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="f5648-102">Delete an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f5648-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5648-103">Permissions</span></span>

<span data-ttu-id="f5648-p101">Для вызова этого API требуется одно из указанных ниже разрешений (в зависимости от ресурса, из которого удаляется расширение). Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f5648-p101">One of the following permissions is required to call this API, depending on the resource you're deleting the extension from. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f5648-106">**Поддерживаемый ресурс**</span><span class="sxs-lookup"><span data-stu-id="f5648-106">**Supported resource**</span></span>|<span data-ttu-id="f5648-107">**Разрешение**</span><span class="sxs-lookup"><span data-stu-id="f5648-107">**Permission**</span></span>|<span data-ttu-id="f5648-108">**Поддерживаемый ресурс**</span><span class="sxs-lookup"><span data-stu-id="f5648-108">**Supported resource**</span></span>|<span data-ttu-id="f5648-109">**Разрешение**</span><span class="sxs-lookup"><span data-stu-id="f5648-109">**Permission**</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="f5648-110">устройство</span><span class="sxs-lookup"><span data-stu-id="f5648-110">device</span></span>](../resources/device.md) | <span data-ttu-id="f5648-111">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5648-111">Device.ReadWrite.All</span></span> | [<span data-ttu-id="f5648-112">событие</span><span class="sxs-lookup"><span data-stu-id="f5648-112">event</span></span>](../resources/event.md) | <span data-ttu-id="f5648-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5648-113">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="f5648-114">группа</span><span class="sxs-lookup"><span data-stu-id="f5648-114">group</span></span>](../resources/group.md) | <span data-ttu-id="f5648-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5648-115">Group.ReadWrite.All</span></span> | <span data-ttu-id="f5648-116">[[event](../resources/event.md) для групп](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="f5648-116">[group event](../resources/event.md)</span></span> | <span data-ttu-id="f5648-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5648-117">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="f5648-118">[[post](../resources/post.md) для групп](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="f5648-118">[group post](../resources/post.md)</span></span> | <span data-ttu-id="f5648-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5648-119">Group.ReadWrite.All</span></span> | [<span data-ttu-id="f5648-120">сообщение</span><span class="sxs-lookup"><span data-stu-id="f5648-120">message</span></span>](../resources/message.md) | <span data-ttu-id="f5648-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5648-121">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="f5648-122">организация</span><span class="sxs-lookup"><span data-stu-id="f5648-122">organization</span></span>](../resources/organization.md) | <span data-ttu-id="f5648-123">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f5648-123">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="f5648-124">[[contact](../resources/contact.md) (личный контакт)](../resources/contact.md)</span><span class="sxs-lookup"><span data-stu-id="f5648-124">[personal contact](../resources/contact.md)</span></span> | <span data-ttu-id="f5648-125">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5648-125">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="f5648-126">пользователь</span><span class="sxs-lookup"><span data-stu-id="f5648-126">user</span></span>](../resources/user.md) | <span data-ttu-id="f5648-127">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f5648-127">Directory.AccessAsUser.All</span></span> | | |

## <a name="http-request"></a><span data-ttu-id="f5648-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5648-128">HTTP request</span></span>
<span data-ttu-id="f5648-129">В запросе идентифицируйте экземпляр ресурса, воспользуйтесь свойством навигации **extensions** этого экземпляра, чтобы определить расширение, и укажите метод `DELETE` для этого экземпляра расширения.</span><span class="sxs-lookup"><span data-stu-id="f5648-129">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/extensions/{extensionId}
DELETE /groups/{id}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
DELETE /organization/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/extensions/{extensionId}
```

><span data-ttu-id="f5648-p102">**Примечание.** В приведенном выше синтаксисе показаны некоторые распространенные способы определения экземпляра ресурса, чье расширение нужно удалить. Все другие варианты синтаксиса, позволяющие определить эти экземпляры ресурса, поддерживают удаление открытых расширений этих экземпляров подобным образом.</span><span class="sxs-lookup"><span data-stu-id="f5648-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="f5648-132">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="f5648-132">Path parameters</span></span>
|<span data-ttu-id="f5648-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="f5648-133">Parameter</span></span>|<span data-ttu-id="f5648-134">Тип</span><span class="sxs-lookup"><span data-stu-id="f5648-134">Type</span></span>|<span data-ttu-id="f5648-135">Описание</span><span class="sxs-lookup"><span data-stu-id="f5648-135">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f5648-136">id</span><span class="sxs-lookup"><span data-stu-id="f5648-136">id</span></span>|<span data-ttu-id="f5648-137">строка</span><span class="sxs-lookup"><span data-stu-id="f5648-137">string</span></span>|<span data-ttu-id="f5648-p103">Уникальный идентификатор экземпляра в соответствующей коллекции. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5648-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="f5648-140">extensionId</span><span class="sxs-lookup"><span data-stu-id="f5648-140">extensionId</span></span>|<span data-ttu-id="f5648-141">строка</span><span class="sxs-lookup"><span data-stu-id="f5648-141">string</span></span>|<span data-ttu-id="f5648-p104">Этот параметр может быть именем расширения, которое представляет собой уникальный текстовый идентификатор для расширения, либо полным именем, в котором сцеплены тип расширения и уникальный текстовый идентификатор. Полное имя возвращается в свойстве `id` при создании расширения. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5648-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="f5648-145">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5648-145">Request headers</span></span>
| <span data-ttu-id="f5648-146">Имя</span><span class="sxs-lookup"><span data-stu-id="f5648-146">Name</span></span>       | <span data-ttu-id="f5648-147">Значение</span><span class="sxs-lookup"><span data-stu-id="f5648-147">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="f5648-148">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5648-148">Authorization</span></span> | <span data-ttu-id="f5648-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5648-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5648-151">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5648-151">Request body</span></span>
<span data-ttu-id="f5648-152">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f5648-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5648-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5648-153">Response</span></span>

<span data-ttu-id="f5648-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f5648-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5648-156">Пример</span><span class="sxs-lookup"><span data-stu-id="f5648-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5648-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5648-157">Request</span></span>
<span data-ttu-id="f5648-158">В первом примере показано, как сослаться на расширение по его имени и удалить расширение в указанном сообщении.</span><span class="sxs-lookup"><span data-stu-id="f5648-158">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="f5648-159">Во втором примере показано, как удалить расширение в событии указанной группы.</span><span class="sxs-lookup"><span data-stu-id="f5648-159">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="f5648-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5648-160">Response</span></span>
<span data-ttu-id="f5648-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f5648-161">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->