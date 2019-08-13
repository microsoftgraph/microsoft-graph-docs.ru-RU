---
title: Обновление устройства
description: Обновление свойств зарегистрированного устройства.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2bf3063a1011ad0f7e7fcdb5e5239ce3eecfa4db
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313027"
---
# <a name="update-device"></a><span data-ttu-id="beabd-103">Обновление устройства</span><span class="sxs-lookup"><span data-stu-id="beabd-103">Update device</span></span>

<span data-ttu-id="beabd-104">Обновление свойств зарегистрированного устройства.</span><span class="sxs-lookup"><span data-stu-id="beabd-104">Update the properties of a registered device.</span></span>

<span data-ttu-id="beabd-105">Лишь определенные свойства устройства можно обновить через утвержденные приложения для управления мобильными устройствами (MDM).</span><span class="sxs-lookup"><span data-stu-id="beabd-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="beabd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="beabd-106">Permissions</span></span>
<span data-ttu-id="beabd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beabd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="beabd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="beabd-109">Permission type</span></span>      | <span data-ttu-id="beabd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="beabd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="beabd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="beabd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="beabd-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="beabd-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="beabd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="beabd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="beabd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beabd-114">Not supported.</span></span> |
|<span data-ttu-id="beabd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="beabd-115">Application</span></span> | <span data-ttu-id="beabd-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="beabd-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="beabd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="beabd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="beabd-118">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="beabd-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="beabd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="beabd-119">Request headers</span></span>
| <span data-ttu-id="beabd-120">Имя</span><span class="sxs-lookup"><span data-stu-id="beabd-120">Name</span></span>       | <span data-ttu-id="beabd-121">Тип</span><span class="sxs-lookup"><span data-stu-id="beabd-121">Type</span></span> | <span data-ttu-id="beabd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="beabd-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="beabd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="beabd-123">Authorization</span></span>  | <span data-ttu-id="beabd-124">string</span><span class="sxs-lookup"><span data-stu-id="beabd-124">string</span></span>  | <span data-ttu-id="beabd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beabd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="beabd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="beabd-127">Request body</span></span>

<span data-ttu-id="beabd-128">Укажите в теле запроса значения обновляемых свойств [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="beabd-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="beabd-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="beabd-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="beabd-130">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="beabd-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="beabd-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="beabd-131">Property</span></span>     | <span data-ttu-id="beabd-132">Тип</span><span class="sxs-lookup"><span data-stu-id="beabd-132">Type</span></span>   |<span data-ttu-id="beabd-133">Описание</span><span class="sxs-lookup"><span data-stu-id="beabd-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="beabd-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="beabd-134">accountEnabled</span></span>|<span data-ttu-id="beabd-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="beabd-135">Boolean</span></span>| <span data-ttu-id="beabd-136">Если учетная запись обеспечена — значение **true**, в противном случае — **false**.</span><span class="sxs-lookup"><span data-stu-id="beabd-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="beabd-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="beabd-137">operatingSystem</span></span>|<span data-ttu-id="beabd-138">String</span><span class="sxs-lookup"><span data-stu-id="beabd-138">String</span></span>|<span data-ttu-id="beabd-139">Тип операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="beabd-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="beabd-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="beabd-140">operatingSystemVersion</span></span>|<span data-ttu-id="beabd-141">String</span><span class="sxs-lookup"><span data-stu-id="beabd-141">String</span></span>|<span data-ttu-id="beabd-142">Версия операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="beabd-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="beabd-143">displayName</span><span class="sxs-lookup"><span data-stu-id="beabd-143">displayName</span></span>|<span data-ttu-id="beabd-144">String</span><span class="sxs-lookup"><span data-stu-id="beabd-144">String</span></span>|<span data-ttu-id="beabd-145">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="beabd-145">The display name for the device.</span></span>|
|<span data-ttu-id="beabd-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="beabd-146">isCompliant</span></span>|<span data-ttu-id="beabd-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="beabd-147">Boolean</span></span>|<span data-ttu-id="beabd-148">Используется значение **true**, если устройство соответствует требованиям политик управления мобильными устройствами (MDM). В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="beabd-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="beabd-149">С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS.</span><span class="sxs-lookup"><span data-stu-id="beabd-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="beabd-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="beabd-150">isManaged</span></span>|<span data-ttu-id="beabd-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="beabd-151">Boolean</span></span>|<span data-ttu-id="beabd-152">Используется значение **true**, если устройство контролируется с помощью приложения для управления мобильными устройствами (MDM), например Intune. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="beabd-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="beabd-153">С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS.</span><span class="sxs-lookup"><span data-stu-id="beabd-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

## <a name="response"></a><span data-ttu-id="beabd-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="beabd-154">Response</span></span>

<span data-ttu-id="beabd-155">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="beabd-155">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="beabd-156">Пример</span><span class="sxs-lookup"><span data-stu-id="beabd-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="beabd-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="beabd-157">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="beabd-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="beabd-158">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="beabd-159">C#</span><span class="sxs-lookup"><span data-stu-id="beabd-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="beabd-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="beabd-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="beabd-161">Цель — C</span><span class="sxs-lookup"><span data-stu-id="beabd-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="beabd-162">Java</span><span class="sxs-lookup"><span data-stu-id="beabd-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="beabd-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="beabd-163">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
