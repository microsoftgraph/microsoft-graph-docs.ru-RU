---
title: Обновление устройства
description: Обновление свойств устройства.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 70c5e6475f32f7e545371064411885d2690e4f0e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455217"
---
# <a name="update-device"></a><span data-ttu-id="fa2e4-103">Обновление устройства</span><span class="sxs-lookup"><span data-stu-id="fa2e4-103">Update device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa2e4-104">Обновление свойств устройства.</span><span class="sxs-lookup"><span data-stu-id="fa2e4-104">Update the properties of a device.</span></span>

<span data-ttu-id="fa2e4-105">Лишь определенные свойства устройства можно обновить через утвержденные приложения для управления мобильными устройствами (MDM).</span><span class="sxs-lookup"><span data-stu-id="fa2e4-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa2e4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa2e4-106">Permissions</span></span>
<span data-ttu-id="fa2e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa2e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa2e4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa2e4-109">Permission type</span></span>      | <span data-ttu-id="fa2e4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa2e4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa2e4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa2e4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fa2e4-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fa2e4-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="fa2e4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa2e4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa2e4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa2e4-114">Not supported.</span></span> |
|<span data-ttu-id="fa2e4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa2e4-115">Application</span></span> | <span data-ttu-id="fa2e4-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fa2e4-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa2e4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa2e4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="fa2e4-118">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="fa2e4-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa2e4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa2e4-119">Request headers</span></span>
| <span data-ttu-id="fa2e4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fa2e4-120">Name</span></span>       | <span data-ttu-id="fa2e4-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fa2e4-121">Type</span></span> | <span data-ttu-id="fa2e4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fa2e4-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fa2e4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa2e4-123">Authorization</span></span>  | <span data-ttu-id="fa2e4-124">string</span><span class="sxs-lookup"><span data-stu-id="fa2e4-124">string</span></span>  | <span data-ttu-id="fa2e4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa2e4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa2e4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa2e4-127">Request body</span></span>

<span data-ttu-id="fa2e4-128">Укажите в теле запроса значения обновляемых свойств [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="fa2e4-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="fa2e4-129">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="fa2e4-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="fa2e4-130">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="fa2e4-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fa2e4-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa2e4-131">Property</span></span>     | <span data-ttu-id="fa2e4-132">Тип</span><span class="sxs-lookup"><span data-stu-id="fa2e4-132">Type</span></span>   |<span data-ttu-id="fa2e4-133">Описание</span><span class="sxs-lookup"><span data-stu-id="fa2e4-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa2e4-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="fa2e4-134">accountEnabled</span></span>|<span data-ttu-id="fa2e4-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa2e4-135">Boolean</span></span>| <span data-ttu-id="fa2e4-136">Если учетная запись обеспечена — значение **true**, в противном случае — **false**.</span><span class="sxs-lookup"><span data-stu-id="fa2e4-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="fa2e4-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="fa2e4-137">operatingSystem</span></span>|<span data-ttu-id="fa2e4-138">Строка</span><span class="sxs-lookup"><span data-stu-id="fa2e4-138">String</span></span>|<span data-ttu-id="fa2e4-139">Тип операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="fa2e4-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="fa2e4-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="fa2e4-140">operatingSystemVersion</span></span>|<span data-ttu-id="fa2e4-141">String</span><span class="sxs-lookup"><span data-stu-id="fa2e4-141">String</span></span>|<span data-ttu-id="fa2e4-142">Версия операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="fa2e4-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="fa2e4-143">displayName</span><span class="sxs-lookup"><span data-stu-id="fa2e4-143">displayName</span></span>|<span data-ttu-id="fa2e4-144">String</span><span class="sxs-lookup"><span data-stu-id="fa2e4-144">String</span></span>|<span data-ttu-id="fa2e4-145">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="fa2e4-145">The display name for the device.</span></span>|
|<span data-ttu-id="fa2e4-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="fa2e4-146">isCompliant</span></span>|<span data-ttu-id="fa2e4-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa2e4-147">Boolean</span></span>|<span data-ttu-id="fa2e4-148">Используется значение **true**, если устройство соответствует требованиям политик управления мобильными устройствами (MDM). В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="fa2e4-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="fa2e4-149">С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS.</span><span class="sxs-lookup"><span data-stu-id="fa2e4-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="fa2e4-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="fa2e4-150">isManaged</span></span>|<span data-ttu-id="fa2e4-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa2e4-151">Boolean</span></span>|<span data-ttu-id="fa2e4-152">Используется значение **true**, если устройство контролируется с помощью приложения для управления мобильными устройствами (MDM), например Intune. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="fa2e4-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="fa2e4-153">С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS.</span><span class="sxs-lookup"><span data-stu-id="fa2e4-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="fa2e4-154">Так как ресурс **Device** поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, зависящие от приложения, в пользовательских свойствах расширения в существующем экземпляре **устройства** .</span><span class="sxs-lookup"><span data-stu-id="fa2e4-154">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="fa2e4-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa2e4-155">Response</span></span>

<span data-ttu-id="fa2e4-156">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fa2e4-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fa2e4-157">Пример</span><span class="sxs-lookup"><span data-stu-id="fa2e4-157">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fa2e4-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa2e4-158">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="fa2e4-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa2e4-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="fa2e4-160">См. также</span><span class="sxs-lookup"><span data-stu-id="fa2e4-160">See also</span></span>

- [<span data-ttu-id="fa2e4-161">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="fa2e4-161">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fa2e4-162">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="fa2e4-162">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="fa2e4-163">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="fa2e4-163">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/device-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
