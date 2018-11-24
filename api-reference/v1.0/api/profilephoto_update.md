# <a name="update-profilephoto"></a><span data-ttu-id="7ef2e-101">Обновление объекта profilephoto</span><span class="sxs-lookup"><span data-stu-id="7ef2e-101">Update profilephoto</span></span>

<span data-ttu-id="7ef2e-p101">Обновление фотографии вошедшего **пользователя** либо указанной **группы** или **контакта**. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемой фотографии не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="7ef2e-p101">Update the photo for the signed-in **user**, or the specified **group** or **contact**. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="7ef2e-104">В версии 1.0 для этой операции можно использовать запросы PATCH и PUT.</span><span class="sxs-lookup"><span data-stu-id="7ef2e-104">You can use either PATCH or PUT for this operation in version 1.0.</span></span>

> <span data-ttu-id="7ef2e-105">**Примечание.** Эта операция в версии 1.0 поддерживает только рабочие или учебные почтовые ящики пользователя (не личные).</span><span class="sxs-lookup"><span data-stu-id="7ef2e-105">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ef2e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ef2e-106">Permissions</span></span>
<span data-ttu-id="7ef2e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7ef2e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="7ef2e-109">Фотография профиля вошедшего **пользователя**: User.ReadWrite, User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="7ef2e-109">Profile photo of the signed-in **user** - User.ReadWrite, User.ReadWrite.All</span></span>
- <span data-ttu-id="7ef2e-110">Фотография профиля **группы**: Group.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="7ef2e-110">Profile photo of a **group** - Group.ReadWrite.All</span></span>
- <span data-ttu-id="7ef2e-111">Фотография **контакта**: Contacts.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="7ef2e-111">Photo of a **contact** - Contacts.ReadWrite</span></span>

> <span data-ttu-id="7ef2e-p103">**Примечание.** Чтобы обновить фотографию какого-либо пользователя в организации, ваше приложение должно получить разрешение User.ReadWrite.All приложения и вызвать API с применением собственного идентификатора, не от имени пользователя. Дополнительные сведения см. в статье [Получение доступа без пользователя](../../../concepts/auth_v2_service.md).</span><span class="sxs-lookup"><span data-stu-id="7ef2e-p103">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user. To learn more, see [get access without a signed-in user](../../../concepts/auth_v2_service.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="7ef2e-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ef2e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/photo/$value
PATCH /users/{id | userPrincipalName}/photo/$value
PATCH /groups/{id}/photo/$value
PATCH /me/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PATCH /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value

PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="request-headers"></a><span data-ttu-id="7ef2e-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ef2e-115">Request headers</span></span>
| <span data-ttu-id="7ef2e-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ef2e-116">Header</span></span>       | <span data-ttu-id="7ef2e-117">Значение</span><span class="sxs-lookup"><span data-stu-id="7ef2e-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7ef2e-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ef2e-118">Authorization</span></span>  | <span data-ttu-id="7ef2e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ef2e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7ef2e-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ef2e-121">Content-Type</span></span>  | <span data-ttu-id="7ef2e-p105">image/jpeg. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ef2e-p105">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7ef2e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ef2e-124">Request body</span></span>
<span data-ttu-id="7ef2e-125">Включите в текст запроса двоичные данные фотографии.</span><span class="sxs-lookup"><span data-stu-id="7ef2e-125">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="7ef2e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ef2e-126">Response</span></span>

<span data-ttu-id="7ef2e-127">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="7ef2e-127">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="7ef2e-128">Пример</span><span class="sxs-lookup"><span data-stu-id="7ef2e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ef2e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ef2e-129">Request</span></span>
<span data-ttu-id="7ef2e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ef2e-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/v1.0/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="7ef2e-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ef2e-131">Response</span></span>
<span data-ttu-id="7ef2e-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7ef2e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
