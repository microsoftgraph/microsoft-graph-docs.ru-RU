---
title: Обновление устройства
description: Обновление свойств устройства.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 24925761ecb7f32408c16f7027725d897811e6b7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260923"
---
# <a name="update-device"></a><span data-ttu-id="e2de4-103">Обновление устройства</span><span class="sxs-lookup"><span data-stu-id="e2de4-103">Update device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2de4-104">Обновление свойств устройства.</span><span class="sxs-lookup"><span data-stu-id="e2de4-104">Update the properties of a device.</span></span>

<span data-ttu-id="e2de4-105">Лишь определенные свойства устройства можно обновить через утвержденные приложения для управления мобильными устройствами (MDM).</span><span class="sxs-lookup"><span data-stu-id="e2de4-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2de4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2de4-106">Permissions</span></span>
<span data-ttu-id="e2de4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2de4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2de4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2de4-109">Permission type</span></span>      | <span data-ttu-id="e2de4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2de4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2de4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2de4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e2de4-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e2de4-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e2de4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2de4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2de4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2de4-114">Not supported.</span></span> |
|<span data-ttu-id="e2de4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2de4-115">Application</span></span> | <span data-ttu-id="e2de4-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e2de4-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2de4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2de4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="e2de4-118">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="e2de4-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2de4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2de4-119">Request headers</span></span>
| <span data-ttu-id="e2de4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e2de4-120">Name</span></span>       | <span data-ttu-id="e2de4-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e2de4-121">Type</span></span> | <span data-ttu-id="e2de4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e2de4-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e2de4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2de4-123">Authorization</span></span>  | <span data-ttu-id="e2de4-124">string</span><span class="sxs-lookup"><span data-stu-id="e2de4-124">string</span></span>  | <span data-ttu-id="e2de4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2de4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2de4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e2de4-127">Request body</span></span>

<span data-ttu-id="e2de4-128">Укажите в теле запроса значения обновляемых свойств [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="e2de4-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="e2de4-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="e2de4-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e2de4-130">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e2de4-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e2de4-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2de4-131">Property</span></span>     | <span data-ttu-id="e2de4-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e2de4-132">Type</span></span>   |<span data-ttu-id="e2de4-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e2de4-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2de4-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="e2de4-134">accountEnabled</span></span>|<span data-ttu-id="e2de4-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2de4-135">Boolean</span></span>| <span data-ttu-id="e2de4-136">Если учетная запись обеспечена — значение **true**, в противном случае — **false**.</span><span class="sxs-lookup"><span data-stu-id="e2de4-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="e2de4-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="e2de4-137">operatingSystem</span></span>|<span data-ttu-id="e2de4-138">String</span><span class="sxs-lookup"><span data-stu-id="e2de4-138">String</span></span>|<span data-ttu-id="e2de4-139">Тип операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e2de4-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="e2de4-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="e2de4-140">operatingSystemVersion</span></span>|<span data-ttu-id="e2de4-141">String</span><span class="sxs-lookup"><span data-stu-id="e2de4-141">String</span></span>|<span data-ttu-id="e2de4-142">Версия операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e2de4-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="e2de4-143">displayName</span><span class="sxs-lookup"><span data-stu-id="e2de4-143">displayName</span></span>|<span data-ttu-id="e2de4-144">String</span><span class="sxs-lookup"><span data-stu-id="e2de4-144">String</span></span>|<span data-ttu-id="e2de4-145">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="e2de4-145">The display name for the device.</span></span>|
|<span data-ttu-id="e2de4-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="e2de4-146">isCompliant</span></span>|<span data-ttu-id="e2de4-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2de4-147">Boolean</span></span>|<span data-ttu-id="e2de4-148">Используется значение **true**, если устройство соответствует требованиям политик управления мобильными устройствами (MDM). В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="e2de4-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="e2de4-149">С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS.</span><span class="sxs-lookup"><span data-stu-id="e2de4-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="e2de4-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="e2de4-150">isManaged</span></span>|<span data-ttu-id="e2de4-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2de4-151">Boolean</span></span>|<span data-ttu-id="e2de4-152">Используется значение **true**, если устройство контролируется с помощью приложения для управления мобильными устройствами (MDM), например Intune. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="e2de4-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="e2de4-153">С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS.</span><span class="sxs-lookup"><span data-stu-id="e2de4-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="e2de4-154">Так как ресурс **Device** поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, зависящие от приложения, в пользовательских свойствах расширения в существующем экземпляре **устройства** .</span><span class="sxs-lookup"><span data-stu-id="e2de4-154">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="e2de4-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2de4-155">Response</span></span>

<span data-ttu-id="e2de4-156">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e2de4-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e2de4-157">Пример</span><span class="sxs-lookup"><span data-stu-id="e2de4-157">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e2de4-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2de4-158">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/beta/devices/{id}
Content-type: application/json
Content-length: 31

{
  "accountEnabled": false
}
```
##### <a name="response"></a><span data-ttu-id="e2de4-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2de4-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e2de4-160">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="e2de4-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e2de4-161">C#</span><span class="sxs-lookup"><span data-stu-id="e2de4-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_device-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2de4-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="e2de4-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_device-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e2de4-163">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e2de4-163">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_device-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="e2de4-164">См. также</span><span class="sxs-lookup"><span data-stu-id="e2de4-164">See also</span></span>

- [<span data-ttu-id="e2de4-165">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="e2de4-165">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e2de4-166">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e2de4-166">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="e2de4-167">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e2de4-167">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/device-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/device-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
