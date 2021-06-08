---
title: Обновление устройства
description: Обновление свойств устройства.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3c895aa8d6122691520d17886ebcdb6f51a2a8c6
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786021"
---
# <a name="update-device"></a><span data-ttu-id="4c075-103">Обновление устройства</span><span class="sxs-lookup"><span data-stu-id="4c075-103">Update device</span></span>

<span data-ttu-id="4c075-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c075-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c075-105">Обновление свойств устройства.</span><span class="sxs-lookup"><span data-stu-id="4c075-105">Update the properties of a device.</span></span>

<span data-ttu-id="4c075-106">Лишь определенные свойства устройства можно обновить через утвержденные приложения для управления мобильными устройствами (MDM).</span><span class="sxs-lookup"><span data-stu-id="4c075-106">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c075-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c075-107">Permissions</span></span>
<span data-ttu-id="4c075-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c075-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c075-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c075-110">Permission type</span></span>      | <span data-ttu-id="4c075-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c075-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c075-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c075-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4c075-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4c075-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="4c075-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c075-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c075-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c075-115">Not supported.</span></span> |
|<span data-ttu-id="4c075-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4c075-116">Application</span></span> | <span data-ttu-id="4c075-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4c075-117">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c075-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c075-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="4c075-119">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="4c075-119">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c075-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c075-120">Request headers</span></span>
| <span data-ttu-id="4c075-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4c075-121">Name</span></span>       | <span data-ttu-id="4c075-122">Тип</span><span class="sxs-lookup"><span data-stu-id="4c075-122">Type</span></span> | <span data-ttu-id="4c075-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4c075-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4c075-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c075-124">Authorization</span></span>  | <span data-ttu-id="4c075-125">string</span><span class="sxs-lookup"><span data-stu-id="4c075-125">string</span></span>  | <span data-ttu-id="4c075-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c075-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c075-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c075-128">Request body</span></span>

<span data-ttu-id="4c075-129">Укажите в теле запроса значения обновляемых свойств [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="4c075-129">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="4c075-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="4c075-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4c075-131">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4c075-131">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4c075-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c075-132">Property</span></span>     | <span data-ttu-id="4c075-133">Тип</span><span class="sxs-lookup"><span data-stu-id="4c075-133">Type</span></span>   |<span data-ttu-id="4c075-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4c075-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c075-135">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="4c075-135">accountEnabled</span></span>|<span data-ttu-id="4c075-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c075-136">Boolean</span></span>| <span data-ttu-id="4c075-137">Значение **true** указывает, что учетная запись включена. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="4c075-137">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="4c075-138">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="4c075-138">operatingSystem</span></span>|<span data-ttu-id="4c075-139">String</span><span class="sxs-lookup"><span data-stu-id="4c075-139">String</span></span>|<span data-ttu-id="4c075-140">Тип операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4c075-140">The type of operating system on the device.</span></span>|
|<span data-ttu-id="4c075-141">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="4c075-141">operatingSystemVersion</span></span>|<span data-ttu-id="4c075-142">String</span><span class="sxs-lookup"><span data-stu-id="4c075-142">String</span></span>|<span data-ttu-id="4c075-143">Версия операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4c075-143">The version of the operating system on the device</span></span>|
|<span data-ttu-id="4c075-144">displayName</span><span class="sxs-lookup"><span data-stu-id="4c075-144">displayName</span></span>|<span data-ttu-id="4c075-145">String</span><span class="sxs-lookup"><span data-stu-id="4c075-145">String</span></span>|<span data-ttu-id="4c075-146">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="4c075-146">The display name for the device.</span></span>|
|<span data-ttu-id="4c075-147">isCompliant</span><span class="sxs-lookup"><span data-stu-id="4c075-147">isCompliant</span></span>|<span data-ttu-id="4c075-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c075-148">Boolean</span></span>|<span data-ttu-id="4c075-149">Используется значение **true**, если устройство соответствует требованиям политик управления мобильными устройствами (MDM). В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="4c075-149">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="4c075-150">Это может быть обновлено intune только для любого типа ОС устройства или утвержденного приложения [MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для Windows устройств ОС.</span><span class="sxs-lookup"><span data-stu-id="4c075-150">This can only be updated by Intune for any device OS type or by an [approved MDM app](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="4c075-151">isManaged</span><span class="sxs-lookup"><span data-stu-id="4c075-151">isManaged</span></span>|<span data-ttu-id="4c075-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c075-152">Boolean</span></span>|<span data-ttu-id="4c075-153">Используется значение **true**, если устройство контролируется с помощью приложения для управления мобильными устройствами (MDM), например Intune. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="4c075-153">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="4c075-154">Это может быть обновлено intune только для любого типа ОС устройства или утвержденного приложения [MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для Windows устройств ОС.</span><span class="sxs-lookup"><span data-stu-id="4c075-154">This can only be updated by Intune for any device OS type or by an [approved MDM app](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="4c075-155">Так как **ресурс устройства** поддерживает [расширения,](/graph/extensibility-overview)вы можете использовать операцию для добавления, обновления или удаления собственных данных, определенных приложениям, в настраиваемые свойства расширения в существующем экземпляре `PATCH` устройства. </span><span class="sxs-lookup"><span data-stu-id="4c075-155">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="4c075-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c075-156">Response</span></span>

<span data-ttu-id="4c075-157">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4c075-157">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4c075-158">Пример</span><span class="sxs-lookup"><span data-stu-id="4c075-158">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4c075-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c075-159">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4c075-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c075-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4c075-161">C#</span><span class="sxs-lookup"><span data-stu-id="4c075-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c075-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c075-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c075-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c075-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c075-164">Java</span><span class="sxs-lookup"><span data-stu-id="4c075-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4c075-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c075-165">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="4c075-166">См. также</span><span class="sxs-lookup"><span data-stu-id="4c075-166">See also</span></span>

- [<span data-ttu-id="4c075-167">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="4c075-167">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4c075-168">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="4c075-168">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="4c075-169">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="4c075-169">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
