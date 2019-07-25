---
title: Обновление устройства
description: Обновление свойств зарегистрированного устройства.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 58f6271c2a9c29fe18755456f6e586aaec8da1ee
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883351"
---
# <a name="update-device"></a><span data-ttu-id="fab18-103">Обновление устройства</span><span class="sxs-lookup"><span data-stu-id="fab18-103">Update device</span></span>

<span data-ttu-id="fab18-104">Обновление свойств зарегистрированного устройства.</span><span class="sxs-lookup"><span data-stu-id="fab18-104">Update the properties of a registered device.</span></span>

<span data-ttu-id="fab18-105">Лишь определенные свойства устройства можно обновить через утвержденные приложения для управления мобильными устройствами (MDM).</span><span class="sxs-lookup"><span data-stu-id="fab18-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="fab18-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fab18-106">Permissions</span></span>
<span data-ttu-id="fab18-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fab18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fab18-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fab18-109">Permission type</span></span>      | <span data-ttu-id="fab18-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fab18-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fab18-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fab18-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fab18-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fab18-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="fab18-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fab18-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fab18-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fab18-114">Not supported.</span></span> |
|<span data-ttu-id="fab18-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fab18-115">Application</span></span> | <span data-ttu-id="fab18-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fab18-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="fab18-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fab18-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="fab18-118">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="fab18-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fab18-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fab18-119">Request headers</span></span>
| <span data-ttu-id="fab18-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fab18-120">Name</span></span>       | <span data-ttu-id="fab18-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fab18-121">Type</span></span> | <span data-ttu-id="fab18-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fab18-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fab18-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fab18-123">Authorization</span></span>  | <span data-ttu-id="fab18-124">string</span><span class="sxs-lookup"><span data-stu-id="fab18-124">string</span></span>  | <span data-ttu-id="fab18-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fab18-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fab18-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fab18-127">Request body</span></span>

<span data-ttu-id="fab18-128">Укажите в теле запроса значения обновляемых свойств [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="fab18-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="fab18-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="fab18-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="fab18-130">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="fab18-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fab18-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="fab18-131">Property</span></span>     | <span data-ttu-id="fab18-132">Тип</span><span class="sxs-lookup"><span data-stu-id="fab18-132">Type</span></span>   |<span data-ttu-id="fab18-133">Описание</span><span class="sxs-lookup"><span data-stu-id="fab18-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fab18-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="fab18-134">accountEnabled</span></span>|<span data-ttu-id="fab18-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="fab18-135">Boolean</span></span>| <span data-ttu-id="fab18-136">Если учетная запись обеспечена — значение **true**, в противном случае — **false**.</span><span class="sxs-lookup"><span data-stu-id="fab18-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="fab18-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="fab18-137">operatingSystem</span></span>|<span data-ttu-id="fab18-138">String</span><span class="sxs-lookup"><span data-stu-id="fab18-138">String</span></span>|<span data-ttu-id="fab18-139">Тип операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="fab18-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="fab18-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="fab18-140">operatingSystemVersion</span></span>|<span data-ttu-id="fab18-141">String</span><span class="sxs-lookup"><span data-stu-id="fab18-141">String</span></span>|<span data-ttu-id="fab18-142">Версия операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="fab18-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="fab18-143">displayName</span><span class="sxs-lookup"><span data-stu-id="fab18-143">displayName</span></span>|<span data-ttu-id="fab18-144">String</span><span class="sxs-lookup"><span data-stu-id="fab18-144">String</span></span>|<span data-ttu-id="fab18-145">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="fab18-145">The display name for the device.</span></span>|
|<span data-ttu-id="fab18-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="fab18-146">isCompliant</span></span>|<span data-ttu-id="fab18-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="fab18-147">Boolean</span></span>|<span data-ttu-id="fab18-148">Используется значение **true**, если устройство соответствует требованиям политик управления мобильными устройствами (MDM). В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="fab18-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="fab18-149">С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS.</span><span class="sxs-lookup"><span data-stu-id="fab18-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="fab18-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="fab18-150">isManaged</span></span>|<span data-ttu-id="fab18-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="fab18-151">Boolean</span></span>|<span data-ttu-id="fab18-152">Используется значение **true**, если устройство контролируется с помощью приложения для управления мобильными устройствами (MDM), например Intune. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="fab18-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="fab18-153">С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS.</span><span class="sxs-lookup"><span data-stu-id="fab18-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

## <a name="response"></a><span data-ttu-id="fab18-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="fab18-154">Response</span></span>

<span data-ttu-id="fab18-155">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fab18-155">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fab18-156">Пример</span><span class="sxs-lookup"><span data-stu-id="fab18-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fab18-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="fab18-157">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fab18-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="fab18-158">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="fab18-159">C#</span><span class="sxs-lookup"><span data-stu-id="fab18-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fab18-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="fab18-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fab18-161">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fab18-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fab18-162">Java</span><span class="sxs-lookup"><span data-stu-id="fab18-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fab18-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="fab18-163">Response</span></span>

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
