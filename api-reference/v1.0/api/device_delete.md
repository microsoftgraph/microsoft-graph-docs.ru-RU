# <a name="delete-device"></a><span data-ttu-id="60f1c-101">Удаление устройства</span><span class="sxs-lookup"><span data-stu-id="60f1c-101">Delete device</span></span>

<span data-ttu-id="60f1c-102">Удаление зарегистрированного устройства.</span><span class="sxs-lookup"><span data-stu-id="60f1c-102">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="60f1c-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60f1c-103">Permissions</span></span>
<span data-ttu-id="60f1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="60f1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="60f1c-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60f1c-106">Permission type</span></span>      | <span data-ttu-id="60f1c-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60f1c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60f1c-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60f1c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="60f1c-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="60f1c-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="60f1c-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60f1c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60f1c-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60f1c-111">Not supported.</span></span>    |
|<span data-ttu-id="60f1c-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60f1c-112">Application</span></span> | <span data-ttu-id="60f1c-113">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60f1c-113">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60f1c-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60f1c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="60f1c-115">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="60f1c-115">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="60f1c-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60f1c-116">Request headers</span></span>
| <span data-ttu-id="60f1c-117">Имя</span><span class="sxs-lookup"><span data-stu-id="60f1c-117">Name</span></span>       | <span data-ttu-id="60f1c-118">Тип</span><span class="sxs-lookup"><span data-stu-id="60f1c-118">Type</span></span> | <span data-ttu-id="60f1c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="60f1c-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="60f1c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="60f1c-120">Authorization</span></span>  | <span data-ttu-id="60f1c-121">string</span><span class="sxs-lookup"><span data-stu-id="60f1c-121">string</span></span>  | <span data-ttu-id="60f1c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60f1c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60f1c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60f1c-124">Request body</span></span>
<span data-ttu-id="60f1c-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60f1c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60f1c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="60f1c-126">Response</span></span>

<span data-ttu-id="60f1c-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="60f1c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60f1c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="60f1c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60f1c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="60f1c-130">Request</span></span>
<span data-ttu-id="60f1c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60f1c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="60f1c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="60f1c-132">Response</span></span>
<span data-ttu-id="60f1c-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="60f1c-133">Here is an example of the response.</span></span>
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
