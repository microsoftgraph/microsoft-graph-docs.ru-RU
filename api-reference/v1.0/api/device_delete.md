# <a name="delete-device"></a><span data-ttu-id="ce89b-101">Удаление устройства</span><span class="sxs-lookup"><span data-stu-id="ce89b-101">Delete device</span></span>

<span data-ttu-id="ce89b-102">Удаление зарегистрированного устройства.</span><span class="sxs-lookup"><span data-stu-id="ce89b-102">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce89b-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce89b-103">Permissions</span></span>
<span data-ttu-id="ce89b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ce89b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="ce89b-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce89b-106">Permission type</span></span>      | <span data-ttu-id="ce89b-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce89b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce89b-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce89b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ce89b-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ce89b-109">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ce89b-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce89b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce89b-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce89b-111">Not supported.</span></span>    |
|<span data-ttu-id="ce89b-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce89b-112">Application</span></span> | <span data-ttu-id="ce89b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce89b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce89b-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce89b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="ce89b-115">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="ce89b-115">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce89b-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce89b-116">Request headers</span></span>
| <span data-ttu-id="ce89b-117">Имя</span><span class="sxs-lookup"><span data-stu-id="ce89b-117">Name</span></span>       | <span data-ttu-id="ce89b-118">Тип</span><span class="sxs-lookup"><span data-stu-id="ce89b-118">Type</span></span> | <span data-ttu-id="ce89b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ce89b-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ce89b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce89b-120">Authorization</span></span>  | <span data-ttu-id="ce89b-121">string</span><span class="sxs-lookup"><span data-stu-id="ce89b-121">string</span></span>  | <span data-ttu-id="ce89b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce89b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce89b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce89b-124">Request body</span></span>
<span data-ttu-id="ce89b-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce89b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce89b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce89b-126">Response</span></span>

<span data-ttu-id="ce89b-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ce89b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce89b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ce89b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce89b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce89b-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="ce89b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce89b-131">Response</span></span>

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
