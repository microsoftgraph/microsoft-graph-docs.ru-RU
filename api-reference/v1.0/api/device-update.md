---
title: Обновление устройства
description: Обновление свойств зарегистрированного устройства.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2521530b8646eab3d2966ba42a101e13f774d97f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273295"
---
# <a name="update-device"></a><span data-ttu-id="03aa8-103">Обновление устройства</span><span class="sxs-lookup"><span data-stu-id="03aa8-103">Update device</span></span>

<span data-ttu-id="03aa8-104">Обновление свойств зарегистрированного устройства.</span><span class="sxs-lookup"><span data-stu-id="03aa8-104">Update the properties of a registered device.</span></span>

<span data-ttu-id="03aa8-105">Лишь определенные свойства устройства можно обновить через утвержденные приложения для управления мобильными устройствами (MDM).</span><span class="sxs-lookup"><span data-stu-id="03aa8-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="03aa8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03aa8-106">Permissions</span></span>
<span data-ttu-id="03aa8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03aa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03aa8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03aa8-109">Permission type</span></span>      | <span data-ttu-id="03aa8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03aa8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03aa8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03aa8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="03aa8-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="03aa8-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="03aa8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03aa8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03aa8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03aa8-114">Not supported.</span></span> |
|<span data-ttu-id="03aa8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03aa8-115">Application</span></span> | <span data-ttu-id="03aa8-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="03aa8-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="03aa8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03aa8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="03aa8-118">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="03aa8-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03aa8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03aa8-119">Request headers</span></span>
| <span data-ttu-id="03aa8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="03aa8-120">Name</span></span>       | <span data-ttu-id="03aa8-121">Тип</span><span class="sxs-lookup"><span data-stu-id="03aa8-121">Type</span></span> | <span data-ttu-id="03aa8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="03aa8-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="03aa8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03aa8-123">Authorization</span></span>  | <span data-ttu-id="03aa8-124">string</span><span class="sxs-lookup"><span data-stu-id="03aa8-124">string</span></span>  | <span data-ttu-id="03aa8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03aa8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03aa8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03aa8-127">Request body</span></span>

<span data-ttu-id="03aa8-128">Укажите в теле запроса значения обновляемых свойств [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="03aa8-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="03aa8-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="03aa8-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="03aa8-130">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="03aa8-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="03aa8-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="03aa8-131">Property</span></span>     | <span data-ttu-id="03aa8-132">Тип</span><span class="sxs-lookup"><span data-stu-id="03aa8-132">Type</span></span>   |<span data-ttu-id="03aa8-133">Описание</span><span class="sxs-lookup"><span data-stu-id="03aa8-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03aa8-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="03aa8-134">accountEnabled</span></span>|<span data-ttu-id="03aa8-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="03aa8-135">Boolean</span></span>| <span data-ttu-id="03aa8-136">Если учетная запись обеспечена — значение **true**, в противном случае — **false**.</span><span class="sxs-lookup"><span data-stu-id="03aa8-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="03aa8-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="03aa8-137">operatingSystem</span></span>|<span data-ttu-id="03aa8-138">String</span><span class="sxs-lookup"><span data-stu-id="03aa8-138">String</span></span>|<span data-ttu-id="03aa8-139">Тип операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="03aa8-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="03aa8-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="03aa8-140">operatingSystemVersion</span></span>|<span data-ttu-id="03aa8-141">String</span><span class="sxs-lookup"><span data-stu-id="03aa8-141">String</span></span>|<span data-ttu-id="03aa8-142">Версия операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="03aa8-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="03aa8-143">displayName</span><span class="sxs-lookup"><span data-stu-id="03aa8-143">displayName</span></span>|<span data-ttu-id="03aa8-144">String</span><span class="sxs-lookup"><span data-stu-id="03aa8-144">String</span></span>|<span data-ttu-id="03aa8-145">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="03aa8-145">The display name for the device.</span></span>|
|<span data-ttu-id="03aa8-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="03aa8-146">isCompliant</span></span>|<span data-ttu-id="03aa8-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="03aa8-147">Boolean</span></span>|<span data-ttu-id="03aa8-148">Используется значение **true**, если устройство соответствует требованиям политик управления мобильными устройствами (MDM). В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="03aa8-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="03aa8-149">С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS.</span><span class="sxs-lookup"><span data-stu-id="03aa8-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="03aa8-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="03aa8-150">isManaged</span></span>|<span data-ttu-id="03aa8-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="03aa8-151">Boolean</span></span>|<span data-ttu-id="03aa8-152">Используется значение **true**, если устройство контролируется с помощью приложения для управления мобильными устройствами (MDM), например Intune. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="03aa8-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="03aa8-153">С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS.</span><span class="sxs-lookup"><span data-stu-id="03aa8-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

## <a name="response"></a><span data-ttu-id="03aa8-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="03aa8-154">Response</span></span>

<span data-ttu-id="03aa8-155">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="03aa8-155">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="03aa8-156">Пример</span><span class="sxs-lookup"><span data-stu-id="03aa8-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03aa8-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="03aa8-157">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="03aa8-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="03aa8-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="03aa8-159">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="03aa8-159">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="03aa8-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="03aa8-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_device-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="03aa8-161">C#</span><span class="sxs-lookup"><span data-stu-id="03aa8-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_device-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="03aa8-162">Цель — C</span><span class="sxs-lookup"><span data-stu-id="03aa8-162">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_device-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/device-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/device-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/device-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
