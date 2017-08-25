# <a name="update-device"></a><span data-ttu-id="bcf10-101">Обновление устройства</span><span class="sxs-lookup"><span data-stu-id="bcf10-101">Update device</span></span>

<span data-ttu-id="bcf10-102">Обновление свойств зарегистрированного устройства.</span><span class="sxs-lookup"><span data-stu-id="bcf10-102">Update the properties of a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcf10-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bcf10-103">Permissions</span></span>
<span data-ttu-id="bcf10-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bcf10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="bcf10-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcf10-106">Permission type</span></span>      | <span data-ttu-id="bcf10-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcf10-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="bcf10-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcf10-108">Delegated (work or school account)</span></span> | <span data-ttu-id="bcf10-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bcf10-109">Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="bcf10-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcf10-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcf10-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcf10-111">Not supported.</span></span>    | 
|<span data-ttu-id="bcf10-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcf10-112">Application</span></span> | <span data-ttu-id="bcf10-113">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcf10-113">Device.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bcf10-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcf10-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="bcf10-115">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="bcf10-115">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bcf10-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcf10-116">Request headers</span></span>
| <span data-ttu-id="bcf10-117">Имя</span><span class="sxs-lookup"><span data-stu-id="bcf10-117">Name</span></span>       | <span data-ttu-id="bcf10-118">Тип</span><span class="sxs-lookup"><span data-stu-id="bcf10-118">Type</span></span> | <span data-ttu-id="bcf10-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bcf10-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bcf10-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcf10-120">Authorization</span></span>  | <span data-ttu-id="bcf10-121">string</span><span class="sxs-lookup"><span data-stu-id="bcf10-121">string</span></span>  | <span data-ttu-id="bcf10-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcf10-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcf10-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bcf10-124">Request body</span></span>
<span data-ttu-id="bcf10-125">Укажите в тексте запроса значения обновляемых свойств объекта [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="bcf10-125">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span>

## <a name="response"></a><span data-ttu-id="bcf10-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcf10-126">Response</span></span>

<span data-ttu-id="bcf10-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bcf10-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bcf10-128">Пример</span><span class="sxs-lookup"><span data-stu-id="bcf10-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bcf10-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcf10-129">Request</span></span>
<span data-ttu-id="bcf10-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcf10-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/devices/{id}
Content-type: application/json

{
  "accountEnabled": true
}
```
##### <a name="response"></a><span data-ttu-id="bcf10-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="bcf10-131">Response</span></span>
<span data-ttu-id="bcf10-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bcf10-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
