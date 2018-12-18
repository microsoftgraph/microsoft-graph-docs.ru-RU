---
title: Обновление устройства
description: Обновление свойств устройства.
author: tfitzmac
ms.openlocfilehash: df86581c1edb531e822204698486358fac29f106
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356562"
---
# <a name="update-device"></a><span data-ttu-id="b8434-103">Обновление устройства</span><span class="sxs-lookup"><span data-stu-id="b8434-103">Update device</span></span>

> <span data-ttu-id="b8434-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b8434-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8434-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8434-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8434-106">Обновление свойств устройства.</span><span class="sxs-lookup"><span data-stu-id="b8434-106">Update the properties of a device.</span></span>

<span data-ttu-id="b8434-107">Лишь определенные свойства устройства можно обновить через утвержденные приложения для управления мобильными устройствами (MDM).</span><span class="sxs-lookup"><span data-stu-id="b8434-107">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8434-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8434-108">Permissions</span></span>
<span data-ttu-id="b8434-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8434-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8434-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8434-111">Permission type</span></span>      | <span data-ttu-id="b8434-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8434-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8434-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8434-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b8434-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b8434-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="b8434-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8434-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8434-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8434-116">Not supported.</span></span> |
|<span data-ttu-id="b8434-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8434-117">Application</span></span> | <span data-ttu-id="b8434-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b8434-118">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8434-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8434-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="b8434-120">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="b8434-120">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8434-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8434-121">Request headers</span></span>
| <span data-ttu-id="b8434-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b8434-122">Name</span></span>       | <span data-ttu-id="b8434-123">Тип</span><span class="sxs-lookup"><span data-stu-id="b8434-123">Type</span></span> | <span data-ttu-id="b8434-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b8434-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b8434-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8434-125">Authorization</span></span>  | <span data-ttu-id="b8434-126">string</span><span class="sxs-lookup"><span data-stu-id="b8434-126">string</span></span>  | <span data-ttu-id="b8434-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8434-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8434-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8434-129">Request body</span></span>

<span data-ttu-id="b8434-130">Укажите в теле запроса значения обновляемых свойств [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="b8434-130">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="b8434-131">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="b8434-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b8434-132">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b8434-132">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b8434-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8434-133">Property</span></span>     | <span data-ttu-id="b8434-134">Тип</span><span class="sxs-lookup"><span data-stu-id="b8434-134">Type</span></span>   |<span data-ttu-id="b8434-135">Описание</span><span class="sxs-lookup"><span data-stu-id="b8434-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8434-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="b8434-136">accountEnabled</span></span>|<span data-ttu-id="b8434-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8434-137">Boolean</span></span>| <span data-ttu-id="b8434-138">Если учетная запись обеспечена — значение **true**, в противном случае — **false**.</span><span class="sxs-lookup"><span data-stu-id="b8434-138">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="b8434-139">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="b8434-139">operatingSystem</span></span>|<span data-ttu-id="b8434-140">String</span><span class="sxs-lookup"><span data-stu-id="b8434-140">String</span></span>|<span data-ttu-id="b8434-141">Тип операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b8434-141">The type of operating system on the device.</span></span>|
|<span data-ttu-id="b8434-142">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="b8434-142">operatingSystemVersion</span></span>|<span data-ttu-id="b8434-143">String</span><span class="sxs-lookup"><span data-stu-id="b8434-143">String</span></span>|<span data-ttu-id="b8434-144">Версия операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b8434-144">The version of the operating system on the device</span></span>|
|<span data-ttu-id="b8434-145">displayName</span><span class="sxs-lookup"><span data-stu-id="b8434-145">displayName</span></span>|<span data-ttu-id="b8434-146">String</span><span class="sxs-lookup"><span data-stu-id="b8434-146">String</span></span>|<span data-ttu-id="b8434-147">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="b8434-147">The display name for the device.</span></span>|
|<span data-ttu-id="b8434-148">isCompliant</span><span class="sxs-lookup"><span data-stu-id="b8434-148">isCompliant</span></span>|<span data-ttu-id="b8434-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8434-149">Boolean</span></span>|<span data-ttu-id="b8434-150">Используется значение **true**, если устройство соответствует требованиям политик управления мобильными устройствами (MDM). В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="b8434-150">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="b8434-151">Это можно обновить, путем Intune для любого типа операционная система устройства или [утвержденных MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="b8434-151">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="b8434-152">isManaged</span><span class="sxs-lookup"><span data-stu-id="b8434-152">isManaged</span></span>|<span data-ttu-id="b8434-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8434-153">Boolean</span></span>|<span data-ttu-id="b8434-154">Используется значение **true**, если устройство контролируется с помощью приложения для управления мобильными устройствами (MDM). В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="b8434-154">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="b8434-155">Это можно обновить, путем Intune для любого типа операционная система устройства или [утвержденных MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="b8434-155">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="b8434-156">Поскольку ресурсов **устройство** поддерживает [расширения](/graph/extensibility-overview), можно использовать `PATCH` операции для добавления, обновления или удаления данных конкретного приложения в настраиваемых свойств расширения в существующий экземпляр **устройства** .</span><span class="sxs-lookup"><span data-stu-id="b8434-156">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="b8434-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="b8434-157">Response</span></span>

<span data-ttu-id="b8434-158">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b8434-158">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b8434-159">Пример</span><span class="sxs-lookup"><span data-stu-id="b8434-159">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b8434-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8434-160">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="b8434-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="b8434-161">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="b8434-162">См. также</span><span class="sxs-lookup"><span data-stu-id="b8434-162">See also</span></span>

- [<span data-ttu-id="b8434-163">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="b8434-163">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b8434-164">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="b8434-164">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="b8434-165">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="b8434-165">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
