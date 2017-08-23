# <a name="create-contact"></a><span data-ttu-id="fa16f-101">Создание объекта Contact</span><span class="sxs-lookup"><span data-stu-id="fa16f-101">Create Contact</span></span>

<span data-ttu-id="fa16f-102">Добавление контакта в корневую папку контактов или в конечную точку `contacts` другой папки контактов.</span><span class="sxs-lookup"><span data-stu-id="fa16f-102">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="fa16f-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa16f-103">Permissions</span></span>
<span data-ttu-id="fa16f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fa16f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fa16f-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa16f-106">Permission type</span></span>      | <span data-ttu-id="fa16f-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa16f-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="fa16f-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa16f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fa16f-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa16f-109">Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="fa16f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa16f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa16f-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa16f-111">Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="fa16f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa16f-112">Application</span></span> | <span data-ttu-id="fa16f-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa16f-113">Contacts.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fa16f-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa16f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="fa16f-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa16f-115">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="fa16f-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa16f-116">Request headers</span></span>
| <span data-ttu-id="fa16f-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa16f-117">Header</span></span>       | <span data-ttu-id="fa16f-118">Значение</span><span class="sxs-lookup"><span data-stu-id="fa16f-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fa16f-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa16f-119">Authorization</span></span>  | <span data-ttu-id="fa16f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa16f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fa16f-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa16f-122">Content-Type</span></span>  | <span data-ttu-id="fa16f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa16f-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fa16f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa16f-125">Request body</span></span>
<span data-ttu-id="fa16f-126">Предоставьте в тексте запроса описание объекта [Contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa16f-126">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fa16f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa16f-127">Response</span></span>

<span data-ttu-id="fa16f-128">В случае успеха этот метод возвращает код отклика `201, Created` и объект [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa16f-128">If successful, this method returns `201, Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa16f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fa16f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa16f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa16f-130">Request</span></span>
<span data-ttu-id="fa16f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa16f-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
<span data-ttu-id="fa16f-132">Предоставьте в тексте запроса описание объекта [contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa16f-132">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fa16f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa16f-133">Response</span></span>
<span data-ttu-id="fa16f-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fa16f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->