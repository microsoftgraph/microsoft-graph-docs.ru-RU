# <a name="send-a-sharing-invitation"></a><span data-ttu-id="fc96e-101">Отправка приглашения к совместному использованию</span><span class="sxs-lookup"><span data-stu-id="fc96e-101">Send a sharing invitation</span></span>

<span data-ttu-id="fc96e-p101">Отправляет приглашение к совместному использованию ресурса **DriveItem**. Приглашение к совместному использованию предоставляет получателям разрешения и при необходимости отправляет им на электронную почту уведомления, что к элементу был предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="fc96e-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc96e-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc96e-104">Permissions</span></span>
<span data-ttu-id="fc96e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fc96e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fc96e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc96e-107">Permission type</span></span>      | <span data-ttu-id="fc96e-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc96e-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="fc96e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc96e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="fc96e-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc96e-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="fc96e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc96e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc96e-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc96e-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="fc96e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc96e-113">Application</span></span> | <span data-ttu-id="fc96e-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc96e-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fc96e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc96e-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{item-id}/invite
POST /drive/items/{item-id}/invite
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
```

## <a name="request-body"></a><span data-ttu-id="fc96e-116">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc96e-116">Request body</span></span>
<span data-ttu-id="fc96e-117">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fc96e-117">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fc96e-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="fc96e-118">Parameter</span></span>        | <span data-ttu-id="fc96e-119">Тип</span><span class="sxs-lookup"><span data-stu-id="fc96e-119">Type</span></span>                                            | <span data-ttu-id="fc96e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fc96e-120">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="fc96e-121">recipients</span><span class="sxs-lookup"><span data-stu-id="fc96e-121">recipients</span></span>       | <span data-ttu-id="fc96e-122">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="fc96e-122">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="fc96e-123">Коллекция получателей, которые будут получать доступ и приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="fc96e-123">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="fc96e-124">message</span><span class="sxs-lookup"><span data-stu-id="fc96e-124">message</span></span>          | <span data-ttu-id="fc96e-125">String</span><span class="sxs-lookup"><span data-stu-id="fc96e-125">String</span></span>                                          | <span data-ttu-id="fc96e-p103">Сообщение с обычным форматированным текстом, включенное в приглашение на доступ. Максимальная длина составляет 2000 символов.</span><span class="sxs-lookup"><span data-stu-id="fc96e-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="fc96e-128">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="fc96e-128">requireSignIn</span></span>    | <span data-ttu-id="fc96e-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc96e-129">Boolean</span></span>                                         | <span data-ttu-id="fc96e-130">Указывает, куда должен зайти получатель приглашения, чтобы просмотреть элемент, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="fc96e-130">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="fc96e-131">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="fc96e-131">sendInvitation</span></span>   | <span data-ttu-id="fc96e-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc96e-132">Boolean</span></span>                                         | <span data-ttu-id="fc96e-133">Указывает, создано ли электронное письмо или запись (false) или разрешение (true).</span><span class="sxs-lookup"><span data-stu-id="fc96e-133">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="fc96e-134">roles</span><span class="sxs-lookup"><span data-stu-id="fc96e-134">roles</span></span>            | <span data-ttu-id="fc96e-135">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="fc96e-135">Collection(String)</span></span>                              | <span data-ttu-id="fc96e-136">Указывают роли, которые предоставляются получателям приглашения на доступ.</span><span class="sxs-lookup"><span data-stu-id="fc96e-136">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <a name="response"></a><span data-ttu-id="fc96e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc96e-137">Response</span></span>

<span data-ttu-id="fc96e-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект коллекции [permission](../resources/permission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc96e-138">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc96e-139">Пример</span><span class="sxs-lookup"><span data-stu-id="fc96e-139">Example</span></span>
<span data-ttu-id="fc96e-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="fc96e-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="fc96e-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc96e-141">Request</span></span>
<span data-ttu-id="fc96e-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc96e-142">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "item_invite"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ]
}
```

##### <a name="response"></a><span data-ttu-id="fc96e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc96e-143">Response</span></span>
<span data-ttu-id="fc96e-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc96e-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="fc96e-145">Заметки</span><span class="sxs-lookup"><span data-stu-id="fc96e-145">Remarks</span></span>

* <span data-ttu-id="fc96e-146">[Диски](../resources/drive.md), у которых для свойства **driveType** задано значение `personal` (личное хранилище OneDrive), не могут создавать и изменять разрешения в корневом ресурсе DriveItem.</span><span class="sxs-lookup"><span data-stu-id="fc96e-146">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 
* <span data-ttu-id="fc96e-147">Список доступных ролей см. в таблице [Перечисление ролей](../resources/permission.md#roles-enumeration).</span><span class="sxs-lookup"><span data-stu-id="fc96e-147">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "item: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
