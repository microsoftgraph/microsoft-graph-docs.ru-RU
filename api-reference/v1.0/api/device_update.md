# <a name="update-device"></a><span data-ttu-id="5061d-101">Обновление устройства</span><span class="sxs-lookup"><span data-stu-id="5061d-101">Update device</span></span>

<span data-ttu-id="5061d-102">Обновление свойств зарегистрированного устройства.</span><span class="sxs-lookup"><span data-stu-id="5061d-102">Update the properties of a registered device.</span></span>

<span data-ttu-id="5061d-103">Лишь определенные свойства устройства можно обновить через утвержденные приложения для управления мобильными устройствами (MDM).</span><span class="sxs-lookup"><span data-stu-id="5061d-103">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="5061d-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5061d-104">Permissions</span></span>
<span data-ttu-id="5061d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5061d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5061d-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5061d-107">Permission type</span></span>      | <span data-ttu-id="5061d-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5061d-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5061d-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5061d-109">Delegated (work or school account)</span></span> | <span data-ttu-id="5061d-110">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5061d-110">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="5061d-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5061d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5061d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5061d-112">Not supported.</span></span> |
|<span data-ttu-id="5061d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5061d-113">Application</span></span> | <span data-ttu-id="5061d-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5061d-114">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="5061d-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5061d-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="5061d-116">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="5061d-116">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5061d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5061d-117">Request headers</span></span>
| <span data-ttu-id="5061d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5061d-118">Name</span></span>       | <span data-ttu-id="5061d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5061d-119">Type</span></span> | <span data-ttu-id="5061d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5061d-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5061d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5061d-121">Authorization</span></span>  | <span data-ttu-id="5061d-122">string</span><span class="sxs-lookup"><span data-stu-id="5061d-122">string</span></span>  | <span data-ttu-id="5061d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5061d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5061d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5061d-125">Request body</span></span>

<span data-ttu-id="5061d-126">Укажите в теле запроса значения обновляемых свойств [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="5061d-126">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="5061d-127">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="5061d-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5061d-128">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5061d-128">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5061d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5061d-129">Property</span></span>     | <span data-ttu-id="5061d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5061d-130">Type</span></span>   |<span data-ttu-id="5061d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5061d-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5061d-132">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="5061d-132">accountEnabled</span></span>|<span data-ttu-id="5061d-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="5061d-133">Boolean</span></span>| <span data-ttu-id="5061d-134">Если учетная запись обеспечена — значение **true**, в противном случае — **false**.</span><span class="sxs-lookup"><span data-stu-id="5061d-134">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="5061d-135">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="5061d-135">operatingSystem</span></span>|<span data-ttu-id="5061d-136">string</span><span class="sxs-lookup"><span data-stu-id="5061d-136">String</span></span>|<span data-ttu-id="5061d-137">Тип операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="5061d-137">The type of operating system on the device.</span></span>|
|<span data-ttu-id="5061d-138">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="5061d-138">operatingSystemVersion</span></span>|<span data-ttu-id="5061d-139">string</span><span class="sxs-lookup"><span data-stu-id="5061d-139">String</span></span>|<span data-ttu-id="5061d-140">Версия операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="5061d-140">The version of the operating system on the device</span></span>|
|<span data-ttu-id="5061d-141">displayName</span><span class="sxs-lookup"><span data-stu-id="5061d-141">displayName</span></span>|<span data-ttu-id="5061d-142">string</span><span class="sxs-lookup"><span data-stu-id="5061d-142">String</span></span>|<span data-ttu-id="5061d-143">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="5061d-143">The display name for the device.</span></span>|
|<span data-ttu-id="5061d-144">isCompliant</span><span class="sxs-lookup"><span data-stu-id="5061d-144">isCompliant</span></span>|<span data-ttu-id="5061d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5061d-145">Boolean</span></span>|<span data-ttu-id="5061d-146">Используется значение **true**, если устройство соответствует требованиям политик управления мобильными устройствами (MDM). В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="5061d-146">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="5061d-147">Это можно обновить только с помощью Intune для любого типа операционной системы устройства или с помощью [утвержденного приложения MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="5061d-147">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="5061d-148">isManaged</span><span class="sxs-lookup"><span data-stu-id="5061d-148">isManaged</span></span>|<span data-ttu-id="5061d-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="5061d-149">Boolean</span></span>|<span data-ttu-id="5061d-150">Используется значение **true**, если устройство контролируется с помощью приложения для управления мобильными устройствами (MDM). В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="5061d-150">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="5061d-151">Это можно обновить только с помощью Intune для любого типа операционной системы устройства или с помощью [утвержденного приложения MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="5061d-151">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

## <a name="response"></a><span data-ttu-id="5061d-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="5061d-152">Response</span></span>

<span data-ttu-id="5061d-153">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5061d-153">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5061d-154">Пример</span><span class="sxs-lookup"><span data-stu-id="5061d-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5061d-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="5061d-155">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/devices/{id}
Content-type: application/json
Content-length: 31

{
  "accountEnabled": false
}
```
##### <a name="response"></a><span data-ttu-id="5061d-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="5061d-156">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
