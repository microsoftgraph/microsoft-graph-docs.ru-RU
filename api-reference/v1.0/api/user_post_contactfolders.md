# <a name="create-contactfolder"></a><span data-ttu-id="37255-101">Создание объекта ContactFolder</span><span class="sxs-lookup"><span data-stu-id="37255-101">Create ContactFolder</span></span>

<span data-ttu-id="37255-102">Создание объекта contactFolder в стандартной папке контактов пользователя.</span><span class="sxs-lookup"><span data-stu-id="37255-102">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="37255-103">Вы также можете [создать экземпляр contactfolder в качестве дочернего для любой указанной папки контактов](contactfolder_post_childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="37255-103">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder_post_childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="37255-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37255-104">Permissions</span></span>
<span data-ttu-id="37255-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="37255-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="37255-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37255-107">Permission type</span></span>      | <span data-ttu-id="37255-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37255-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37255-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37255-109">Delegated (work or school account)</span></span> | <span data-ttu-id="37255-110">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37255-110">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="37255-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37255-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37255-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37255-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="37255-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37255-113">Application</span></span> | <span data-ttu-id="37255-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37255-114">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="37255-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37255-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="37255-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37255-116">Request headers</span></span>
| <span data-ttu-id="37255-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37255-117">Header</span></span>       | <span data-ttu-id="37255-118">Значение</span><span class="sxs-lookup"><span data-stu-id="37255-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="37255-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37255-119">Authorization</span></span>  | <span data-ttu-id="37255-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37255-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="37255-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37255-122">Content-Type</span></span>  | <span data-ttu-id="37255-123">application/json</span><span class="sxs-lookup"><span data-stu-id="37255-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="37255-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37255-124">Request body</span></span>
<span data-ttu-id="37255-125">Предоставьте в тексте запроса описание объекта [ContactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37255-125">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="37255-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="37255-126">Response</span></span>

<span data-ttu-id="37255-127">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="37255-127">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37255-128">Пример</span><span class="sxs-lookup"><span data-stu-id="37255-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37255-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="37255-129">Request</span></span>
<span data-ttu-id="37255-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37255-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
<span data-ttu-id="37255-131">Предоставьте в тексте запроса описание объекта [contactFolder](../resources/contactfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37255-131">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="37255-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="37255-132">Response</span></span>
<span data-ttu-id="37255-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="37255-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
