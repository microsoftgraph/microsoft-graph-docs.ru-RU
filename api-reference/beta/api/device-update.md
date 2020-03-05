---
title: Обновление устройства
description: Обновление свойств устройства.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e44e28ea9d496e039d2820098ec8f1ce8caae643
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435558"
---
# <a name="update-device"></a><span data-ttu-id="36ba3-103">Обновление устройства</span><span class="sxs-lookup"><span data-stu-id="36ba3-103">Update device</span></span>

<span data-ttu-id="36ba3-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="36ba3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36ba3-105">Обновление свойств устройства.</span><span class="sxs-lookup"><span data-stu-id="36ba3-105">Update the properties of a device.</span></span>

<span data-ttu-id="36ba3-106">Лишь определенные свойства устройства можно обновить через утвержденные приложения для управления мобильными устройствами (MDM).</span><span class="sxs-lookup"><span data-stu-id="36ba3-106">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="36ba3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36ba3-107">Permissions</span></span>
<span data-ttu-id="36ba3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36ba3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36ba3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36ba3-110">Permission type</span></span>      | <span data-ttu-id="36ba3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36ba3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36ba3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36ba3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="36ba3-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="36ba3-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="36ba3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36ba3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36ba3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36ba3-115">Not supported.</span></span> |
|<span data-ttu-id="36ba3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36ba3-116">Application</span></span> | <span data-ttu-id="36ba3-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="36ba3-117">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="36ba3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36ba3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="36ba3-119">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="36ba3-119">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36ba3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36ba3-120">Request headers</span></span>
| <span data-ttu-id="36ba3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="36ba3-121">Name</span></span>       | <span data-ttu-id="36ba3-122">Тип</span><span class="sxs-lookup"><span data-stu-id="36ba3-122">Type</span></span> | <span data-ttu-id="36ba3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="36ba3-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="36ba3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="36ba3-124">Authorization</span></span>  | <span data-ttu-id="36ba3-125">string</span><span class="sxs-lookup"><span data-stu-id="36ba3-125">string</span></span>  | <span data-ttu-id="36ba3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36ba3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36ba3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36ba3-128">Request body</span></span>

<span data-ttu-id="36ba3-129">Укажите в теле запроса значения обновляемых свойств [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="36ba3-129">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="36ba3-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="36ba3-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="36ba3-131">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="36ba3-131">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="36ba3-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="36ba3-132">Property</span></span>     | <span data-ttu-id="36ba3-133">Тип</span><span class="sxs-lookup"><span data-stu-id="36ba3-133">Type</span></span>   |<span data-ttu-id="36ba3-134">Описание</span><span class="sxs-lookup"><span data-stu-id="36ba3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36ba3-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="36ba3-135">accountEnabled</span></span>|<span data-ttu-id="36ba3-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="36ba3-136">Boolean</span></span>| <span data-ttu-id="36ba3-137">Значение **true** указывает, что учетная запись включена. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="36ba3-137">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="36ba3-138">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="36ba3-138">operatingSystem</span></span>|<span data-ttu-id="36ba3-139">String</span><span class="sxs-lookup"><span data-stu-id="36ba3-139">String</span></span>|<span data-ttu-id="36ba3-140">Тип операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="36ba3-140">The type of operating system on the device.</span></span>|
|<span data-ttu-id="36ba3-141">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="36ba3-141">operatingSystemVersion</span></span>|<span data-ttu-id="36ba3-142">String</span><span class="sxs-lookup"><span data-stu-id="36ba3-142">String</span></span>|<span data-ttu-id="36ba3-143">Версия операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="36ba3-143">The version of the operating system on the device</span></span>|
|<span data-ttu-id="36ba3-144">displayName</span><span class="sxs-lookup"><span data-stu-id="36ba3-144">displayName</span></span>|<span data-ttu-id="36ba3-145">String</span><span class="sxs-lookup"><span data-stu-id="36ba3-145">String</span></span>|<span data-ttu-id="36ba3-146">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="36ba3-146">The display name for the device.</span></span>|
|<span data-ttu-id="36ba3-147">isCompliant</span><span class="sxs-lookup"><span data-stu-id="36ba3-147">isCompliant</span></span>|<span data-ttu-id="36ba3-148">Логический</span><span class="sxs-lookup"><span data-stu-id="36ba3-148">Boolean</span></span>|<span data-ttu-id="36ba3-149">Используется значение **true**, если устройство соответствует требованиям политик управления мобильными устройствами (MDM). В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="36ba3-149">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="36ba3-150">С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS.</span><span class="sxs-lookup"><span data-stu-id="36ba3-150">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="36ba3-151">isManaged</span><span class="sxs-lookup"><span data-stu-id="36ba3-151">isManaged</span></span>|<span data-ttu-id="36ba3-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="36ba3-152">Boolean</span></span>|<span data-ttu-id="36ba3-153">Используется значение **true**, если устройство контролируется с помощью приложения для управления мобильными устройствами (MDM), например Intune. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="36ba3-153">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="36ba3-154">С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS.</span><span class="sxs-lookup"><span data-stu-id="36ba3-154">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="36ba3-155">Так как ресурс **Device** поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, зависящие от приложения, в пользовательских свойствах расширения в существующем экземпляре **устройства** .</span><span class="sxs-lookup"><span data-stu-id="36ba3-155">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="36ba3-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="36ba3-156">Response</span></span>

<span data-ttu-id="36ba3-157">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="36ba3-157">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="36ba3-158">Пример</span><span class="sxs-lookup"><span data-stu-id="36ba3-158">Example</span></span>

##### <a name="request"></a><span data-ttu-id="36ba3-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="36ba3-159">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="36ba3-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="36ba3-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="36ba3-161">C#</span><span class="sxs-lookup"><span data-stu-id="36ba3-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36ba3-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36ba3-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36ba3-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36ba3-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="36ba3-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="36ba3-164">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="36ba3-165">См. также</span><span class="sxs-lookup"><span data-stu-id="36ba3-165">See also</span></span>

- [<span data-ttu-id="36ba3-166">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="36ba3-166">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="36ba3-167">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="36ba3-167">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="36ba3-168">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="36ba3-168">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
  ]
}
-->
