# <a name="create-registereduser"></a><span data-ttu-id="6e0f9-101">Создание объекта registeredUser</span><span class="sxs-lookup"><span data-stu-id="6e0f9-101">Create registeredUser</span></span>

<span data-ttu-id="6e0f9-102">Добавление зарегистрированного пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="6e0f9-102">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e0f9-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e0f9-103">Permissions</span></span>
<span data-ttu-id="6e0f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6e0f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="6e0f9-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e0f9-106">Permission type</span></span>      | <span data-ttu-id="6e0f9-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e0f9-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="6e0f9-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e0f9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6e0f9-109">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6e0f9-109">Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="6e0f9-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e0f9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e0f9-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e0f9-111">Not supported.</span></span>    | 
|<span data-ttu-id="6e0f9-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e0f9-112">Application</span></span> | <span data-ttu-id="6e0f9-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e0f9-113">Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6e0f9-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e0f9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers

```
## <a name="request-headers"></a><span data-ttu-id="6e0f9-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e0f9-115">Request headers</span></span>
| <span data-ttu-id="6e0f9-116">Имя</span><span class="sxs-lookup"><span data-stu-id="6e0f9-116">Name</span></span>       | <span data-ttu-id="6e0f9-117">Тип</span><span class="sxs-lookup"><span data-stu-id="6e0f9-117">Type</span></span> | <span data-ttu-id="6e0f9-118">Описание</span><span class="sxs-lookup"><span data-stu-id="6e0f9-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6e0f9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e0f9-119">Authorization</span></span>  | <span data-ttu-id="6e0f9-120">string</span><span class="sxs-lookup"><span data-stu-id="6e0f9-120">string</span></span>  | <span data-ttu-id="6e0f9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e0f9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e0f9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e0f9-123">Request body</span></span>
<span data-ttu-id="6e0f9-124">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e0f9-124">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6e0f9-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e0f9-125">Response</span></span>

<span data-ttu-id="6e0f9-126">В случае успеха этот метод возвращает код отклика `201, Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6e0f9-126">If successful, this method returns `201, Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e0f9-127">Пример</span><span class="sxs-lookup"><span data-stu-id="6e0f9-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e0f9-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e0f9-128">Request</span></span>
<span data-ttu-id="6e0f9-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e0f9-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="6e0f9-130">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e0f9-130">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6e0f9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e0f9-131">Response</span></span>
<span data-ttu-id="6e0f9-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6e0f9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create registeredUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->