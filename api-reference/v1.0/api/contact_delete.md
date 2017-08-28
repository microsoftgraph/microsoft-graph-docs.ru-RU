# <a name="delete-contact"></a><span data-ttu-id="fb8b8-101">Удаление контакта</span><span class="sxs-lookup"><span data-stu-id="fb8b8-101">Delete contact</span></span>

<span data-ttu-id="fb8b8-102">Удаление контакта.</span><span class="sxs-lookup"><span data-stu-id="fb8b8-102">Delete a contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="fb8b8-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb8b8-103">Permissions</span></span>
<span data-ttu-id="fb8b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fb8b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fb8b8-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb8b8-106">Permission type</span></span>      | <span data-ttu-id="fb8b8-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb8b8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb8b8-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb8b8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fb8b8-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb8b8-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="fb8b8-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb8b8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb8b8-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb8b8-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="fb8b8-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb8b8-112">Application</span></span> | <span data-ttu-id="fb8b8-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb8b8-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb8b8-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb8b8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="fb8b8-115">Объект [contact](../resources/contact.md) из стандартной пользовательской папки [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="fb8b8-115">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="fb8b8-116">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="fb8b8-116">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="fb8b8-p102">Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md). Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="fb8b8-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fb8b8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb8b8-119">Request headers</span></span>
| <span data-ttu-id="fb8b8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb8b8-120">Header</span></span>       | <span data-ttu-id="fb8b8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fb8b8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fb8b8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb8b8-122">Authorization</span></span>  | <span data-ttu-id="fb8b8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb8b8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fb8b8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb8b8-125">Request body</span></span>
<span data-ttu-id="fb8b8-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb8b8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb8b8-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb8b8-127">Response</span></span>

<span data-ttu-id="fb8b8-p104">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="fb8b8-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb8b8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fb8b8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb8b8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb8b8-131">Request</span></span>
<span data-ttu-id="fb8b8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb8b8-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="fb8b8-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb8b8-133">Response</span></span>
<span data-ttu-id="fb8b8-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fb8b8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
