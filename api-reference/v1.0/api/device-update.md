---
title: Обновление устройства
description: Обновление свойств зарегистрированного устройства.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aaa8343307707142ca969c4257cc051e36a8cd7a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889539"
---
# <a name="update-device"></a><span data-ttu-id="1c5b0-103">Обновление устройства</span><span class="sxs-lookup"><span data-stu-id="1c5b0-103">Update device</span></span>

<span data-ttu-id="1c5b0-104">Обновление свойств зарегистрированного устройства.</span><span class="sxs-lookup"><span data-stu-id="1c5b0-104">Update the properties of a registered device.</span></span>

<span data-ttu-id="1c5b0-105">Лишь определенные свойства устройства можно обновить через утвержденные приложения для управления мобильными устройствами (MDM).</span><span class="sxs-lookup"><span data-stu-id="1c5b0-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c5b0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c5b0-106">Permissions</span></span>
<span data-ttu-id="1c5b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c5b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c5b0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c5b0-109">Permission type</span></span>      | <span data-ttu-id="1c5b0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c5b0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c5b0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c5b0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1c5b0-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1c5b0-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="1c5b0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c5b0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c5b0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c5b0-114">Not supported.</span></span> |
|<span data-ttu-id="1c5b0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c5b0-115">Application</span></span> | <span data-ttu-id="1c5b0-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1c5b0-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c5b0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c5b0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="1c5b0-118">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="1c5b0-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c5b0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c5b0-119">Request headers</span></span>
| <span data-ttu-id="1c5b0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1c5b0-120">Name</span></span>       | <span data-ttu-id="1c5b0-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1c5b0-121">Type</span></span> | <span data-ttu-id="1c5b0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1c5b0-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1c5b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c5b0-123">Authorization</span></span>  | <span data-ttu-id="1c5b0-124">string</span><span class="sxs-lookup"><span data-stu-id="1c5b0-124">string</span></span>  | <span data-ttu-id="1c5b0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c5b0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c5b0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c5b0-127">Request body</span></span>

<span data-ttu-id="1c5b0-128">Укажите в теле запроса значения обновляемых свойств [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="1c5b0-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="1c5b0-129">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="1c5b0-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1c5b0-130">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1c5b0-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1c5b0-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c5b0-131">Property</span></span>     | <span data-ttu-id="1c5b0-132">Тип</span><span class="sxs-lookup"><span data-stu-id="1c5b0-132">Type</span></span>   |<span data-ttu-id="1c5b0-133">Описание</span><span class="sxs-lookup"><span data-stu-id="1c5b0-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c5b0-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="1c5b0-134">accountEnabled</span></span>|<span data-ttu-id="1c5b0-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c5b0-135">Boolean</span></span>| <span data-ttu-id="1c5b0-136">Если учетная запись обеспечена — значение **true**, в противном случае — **false**.</span><span class="sxs-lookup"><span data-stu-id="1c5b0-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="1c5b0-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="1c5b0-137">operatingSystem</span></span>|<span data-ttu-id="1c5b0-138">String</span><span class="sxs-lookup"><span data-stu-id="1c5b0-138">String</span></span>|<span data-ttu-id="1c5b0-139">Тип операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="1c5b0-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="1c5b0-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="1c5b0-140">operatingSystemVersion</span></span>|<span data-ttu-id="1c5b0-141">String</span><span class="sxs-lookup"><span data-stu-id="1c5b0-141">String</span></span>|<span data-ttu-id="1c5b0-142">Версия операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="1c5b0-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="1c5b0-143">displayName</span><span class="sxs-lookup"><span data-stu-id="1c5b0-143">displayName</span></span>|<span data-ttu-id="1c5b0-144">String</span><span class="sxs-lookup"><span data-stu-id="1c5b0-144">String</span></span>|<span data-ttu-id="1c5b0-145">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="1c5b0-145">The display name for the device.</span></span>|
|<span data-ttu-id="1c5b0-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="1c5b0-146">isCompliant</span></span>|<span data-ttu-id="1c5b0-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c5b0-147">Boolean</span></span>|<span data-ttu-id="1c5b0-148">Используется значение **true**, если устройство соответствует требованиям политик управления мобильными устройствами (MDM). В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="1c5b0-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="1c5b0-149">Это можно обновить, путем Intune для любого типа операционная система устройства или [утвержденных MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="1c5b0-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="1c5b0-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="1c5b0-150">isManaged</span></span>|<span data-ttu-id="1c5b0-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c5b0-151">Boolean</span></span>|<span data-ttu-id="1c5b0-152">Используется значение **true**, если устройство контролируется с помощью приложения для управления мобильными устройствами (MDM). В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="1c5b0-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="1c5b0-153">Это можно обновить, путем Intune для любого типа операционная система устройства или [утвержденных MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="1c5b0-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

## <a name="response"></a><span data-ttu-id="1c5b0-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c5b0-154">Response</span></span>

<span data-ttu-id="1c5b0-155">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1c5b0-155">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1c5b0-156">Пример</span><span class="sxs-lookup"><span data-stu-id="1c5b0-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c5b0-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c5b0-157">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="1c5b0-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c5b0-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
