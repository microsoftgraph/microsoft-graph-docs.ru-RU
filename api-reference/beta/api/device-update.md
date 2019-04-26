---
title: Обновление устройства
description: Обновление свойств устройства.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fee5f5a33a881801fa50ee5fae7a01ebbdf197cc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326038"
---
# <a name="update-device"></a><span data-ttu-id="7c7da-103">Обновление устройства</span><span class="sxs-lookup"><span data-stu-id="7c7da-103">Update device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c7da-104">Обновление свойств устройства.</span><span class="sxs-lookup"><span data-stu-id="7c7da-104">Update the properties of a device.</span></span>

<span data-ttu-id="7c7da-105">Лишь определенные свойства устройства можно обновить через утвержденные приложения для управления мобильными устройствами (MDM).</span><span class="sxs-lookup"><span data-stu-id="7c7da-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c7da-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c7da-106">Permissions</span></span>
<span data-ttu-id="7c7da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c7da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c7da-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c7da-109">Permission type</span></span>      | <span data-ttu-id="7c7da-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c7da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c7da-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c7da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7c7da-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7c7da-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="7c7da-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c7da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c7da-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c7da-114">Not supported.</span></span> |
|<span data-ttu-id="7c7da-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7c7da-115">Application</span></span> | <span data-ttu-id="7c7da-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c7da-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c7da-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c7da-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="7c7da-118">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="7c7da-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c7da-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c7da-119">Request headers</span></span>
| <span data-ttu-id="7c7da-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7c7da-120">Name</span></span>       | <span data-ttu-id="7c7da-121">Тип</span><span class="sxs-lookup"><span data-stu-id="7c7da-121">Type</span></span> | <span data-ttu-id="7c7da-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7c7da-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7c7da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c7da-123">Authorization</span></span>  | <span data-ttu-id="7c7da-124">string</span><span class="sxs-lookup"><span data-stu-id="7c7da-124">string</span></span>  | <span data-ttu-id="7c7da-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c7da-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c7da-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7c7da-127">Request body</span></span>

<span data-ttu-id="7c7da-128">Укажите в теле запроса значения обновляемых свойств [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="7c7da-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="7c7da-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="7c7da-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7c7da-130">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7c7da-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7c7da-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c7da-131">Property</span></span>     | <span data-ttu-id="7c7da-132">Тип</span><span class="sxs-lookup"><span data-stu-id="7c7da-132">Type</span></span>   |<span data-ttu-id="7c7da-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7c7da-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c7da-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="7c7da-134">accountEnabled</span></span>|<span data-ttu-id="7c7da-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c7da-135">Boolean</span></span>| <span data-ttu-id="7c7da-136">Если учетная запись обеспечена — значение **true**, в противном случае — **false**.</span><span class="sxs-lookup"><span data-stu-id="7c7da-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="7c7da-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="7c7da-137">operatingSystem</span></span>|<span data-ttu-id="7c7da-138">String</span><span class="sxs-lookup"><span data-stu-id="7c7da-138">String</span></span>|<span data-ttu-id="7c7da-139">Тип операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7c7da-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="7c7da-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="7c7da-140">operatingSystemVersion</span></span>|<span data-ttu-id="7c7da-141">String</span><span class="sxs-lookup"><span data-stu-id="7c7da-141">String</span></span>|<span data-ttu-id="7c7da-142">Версия операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="7c7da-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="7c7da-143">displayName</span><span class="sxs-lookup"><span data-stu-id="7c7da-143">displayName</span></span>|<span data-ttu-id="7c7da-144">String</span><span class="sxs-lookup"><span data-stu-id="7c7da-144">String</span></span>|<span data-ttu-id="7c7da-145">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="7c7da-145">The display name for the device.</span></span>|
|<span data-ttu-id="7c7da-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="7c7da-146">isCompliant</span></span>|<span data-ttu-id="7c7da-147">Логический</span><span class="sxs-lookup"><span data-stu-id="7c7da-147">Boolean</span></span>|<span data-ttu-id="7c7da-148">Используется значение **true**, если устройство соответствует требованиям политик управления мобильными устройствами (MDM). В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="7c7da-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="7c7da-149">С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS.</span><span class="sxs-lookup"><span data-stu-id="7c7da-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="7c7da-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="7c7da-150">isManaged</span></span>|<span data-ttu-id="7c7da-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c7da-151">Boolean</span></span>|<span data-ttu-id="7c7da-152">Используется значение **true**, если устройство контролируется с помощью приложения для управления мобильными устройствами (MDM), например Intune. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="7c7da-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="7c7da-153">С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS.</span><span class="sxs-lookup"><span data-stu-id="7c7da-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="7c7da-154">Так как ресурс **Device** поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, зависящие от приложения, в пользовательских свойствах расширения в существующем экземпляре **устройства** .</span><span class="sxs-lookup"><span data-stu-id="7c7da-154">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="7c7da-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c7da-155">Response</span></span>

<span data-ttu-id="7c7da-156">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7c7da-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7c7da-157">Пример</span><span class="sxs-lookup"><span data-stu-id="7c7da-157">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7c7da-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c7da-158">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="7c7da-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c7da-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="7c7da-160">См. также</span><span class="sxs-lookup"><span data-stu-id="7c7da-160">See also</span></span>

- [<span data-ttu-id="7c7da-161">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="7c7da-161">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7c7da-162">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="7c7da-162">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="7c7da-163">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="7c7da-163">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
