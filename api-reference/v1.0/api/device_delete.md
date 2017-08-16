# <a name="delete-device"></a><span data-ttu-id="25ea6-101">Удаление устройства</span><span class="sxs-lookup"><span data-stu-id="25ea6-101">Delete device</span></span>

<span data-ttu-id="25ea6-102">Удаление зарегистрированного устройства.</span><span class="sxs-lookup"><span data-stu-id="25ea6-102">Delete a registered device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25ea6-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="25ea6-103">Prerequisites</span></span>
<span data-ttu-id="25ea6-104">Для применения этого API требуется одна из указанных ниже **областей**. *Directory.AccessAsUser.All*, *Device.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="25ea6-104">One of the following **scopes** is required to execute this API: *Directory.AccessAsUser.All*, *Device.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="25ea6-105">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25ea6-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="25ea6-106">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="25ea6-106">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25ea6-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25ea6-107">Request headers</span></span>
| <span data-ttu-id="25ea6-108">Имя</span><span class="sxs-lookup"><span data-stu-id="25ea6-108">Name</span></span>       | <span data-ttu-id="25ea6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="25ea6-109">Type</span></span> | <span data-ttu-id="25ea6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="25ea6-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="25ea6-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="25ea6-111">Authorization</span></span>  | <span data-ttu-id="25ea6-112">string</span><span class="sxs-lookup"><span data-stu-id="25ea6-112">string</span></span>  | <span data-ttu-id="25ea6-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25ea6-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25ea6-115">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25ea6-115">Request body</span></span>
<span data-ttu-id="25ea6-116">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25ea6-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25ea6-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="25ea6-117">Response</span></span>

<span data-ttu-id="25ea6-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="25ea6-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25ea6-120">Пример</span><span class="sxs-lookup"><span data-stu-id="25ea6-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25ea6-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="25ea6-121">Request</span></span>
<span data-ttu-id="25ea6-122">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25ea6-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="25ea6-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="25ea6-123">Response</span></span>
<span data-ttu-id="25ea6-124">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="25ea6-124">Here is an example of the response.</span></span>
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
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
