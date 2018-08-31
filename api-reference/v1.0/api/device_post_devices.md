# <a name="create-device"></a><span data-ttu-id="48058-101">Создание устройства</span><span class="sxs-lookup"><span data-stu-id="48058-101">Create device</span></span>

<span data-ttu-id="48058-102">Создание и регистрация нового устройства в организации.</span><span class="sxs-lookup"><span data-stu-id="48058-102">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="48058-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48058-103">Permissions</span></span>
<span data-ttu-id="48058-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="48058-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="48058-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48058-106">Permission type</span></span>      | <span data-ttu-id="48058-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48058-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48058-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48058-108">Delegated (work or school account)</span></span> | <span data-ttu-id="48058-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="48058-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="48058-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48058-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48058-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48058-111">Not supported.</span></span>    |
|<span data-ttu-id="48058-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48058-112">Application</span></span> | <span data-ttu-id="48058-113">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48058-113">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48058-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48058-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="48058-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48058-115">Request headers</span></span>
| <span data-ttu-id="48058-116">Имя</span><span class="sxs-lookup"><span data-stu-id="48058-116">Name</span></span>       | <span data-ttu-id="48058-117">Тип</span><span class="sxs-lookup"><span data-stu-id="48058-117">Type</span></span> | <span data-ttu-id="48058-118">Описание</span><span class="sxs-lookup"><span data-stu-id="48058-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="48058-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48058-119">Authorization</span></span>  | <span data-ttu-id="48058-120">string (строка)</span><span class="sxs-lookup"><span data-stu-id="48058-120">string</span></span>  | <span data-ttu-id="48058-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48058-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="48058-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48058-123">Content-type</span></span> | <span data-ttu-id="48058-124">string (строка)</span><span class="sxs-lookup"><span data-stu-id="48058-124">string</span></span> | <span data-ttu-id="48058-125">application/json</span><span class="sxs-lookup"><span data-stu-id="48058-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="48058-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48058-126">Request body</span></span>
<span data-ttu-id="48058-127">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48058-127">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="48058-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="48058-128">Response</span></span>

<span data-ttu-id="48058-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48058-129">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48058-130">Пример</span><span class="sxs-lookup"><span data-stu-id="48058-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48058-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="48058-131">Request</span></span>
<span data-ttu-id="48058-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48058-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"base64Y3YxN2E1MWFlYw=="
    }
  ],
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```
<span data-ttu-id="48058-133">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48058-133">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="48058-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="48058-134">Response</span></span>
<span data-ttu-id="48058-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48058-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"base64Y3YxN2E1MWFlYw=="
    }
  ],
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "id": "id-value",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
