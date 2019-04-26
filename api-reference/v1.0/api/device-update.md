---
title: Обновление устройства
description: Обновление свойств зарегистрированного устройства.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f24372e122045eee9d79cde6334038f0dc1ccddf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583510"
---
# <a name="update-device"></a><span data-ttu-id="2d8bd-103">Обновление устройства</span><span class="sxs-lookup"><span data-stu-id="2d8bd-103">Update device</span></span>

<span data-ttu-id="2d8bd-104">Обновление свойств зарегистрированного устройства.</span><span class="sxs-lookup"><span data-stu-id="2d8bd-104">Update the properties of a registered device.</span></span>

<span data-ttu-id="2d8bd-105">Лишь определенные свойства устройства можно обновить через утвержденные приложения для управления мобильными устройствами (MDM).</span><span class="sxs-lookup"><span data-stu-id="2d8bd-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d8bd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d8bd-106">Permissions</span></span>
<span data-ttu-id="2d8bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d8bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d8bd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d8bd-109">Permission type</span></span>      | <span data-ttu-id="2d8bd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d8bd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d8bd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d8bd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2d8bd-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2d8bd-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="2d8bd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d8bd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d8bd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d8bd-114">Not supported.</span></span> |
|<span data-ttu-id="2d8bd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d8bd-115">Application</span></span> | <span data-ttu-id="2d8bd-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2d8bd-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d8bd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d8bd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="2d8bd-118">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="2d8bd-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d8bd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d8bd-119">Request headers</span></span>
| <span data-ttu-id="2d8bd-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2d8bd-120">Name</span></span>       | <span data-ttu-id="2d8bd-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2d8bd-121">Type</span></span> | <span data-ttu-id="2d8bd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2d8bd-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2d8bd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d8bd-123">Authorization</span></span>  | <span data-ttu-id="2d8bd-124">string</span><span class="sxs-lookup"><span data-stu-id="2d8bd-124">string</span></span>  | <span data-ttu-id="2d8bd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d8bd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d8bd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d8bd-127">Request body</span></span>

<span data-ttu-id="2d8bd-128">Укажите в теле запроса значения обновляемых свойств [device](../resources/device.md).</span><span class="sxs-lookup"><span data-stu-id="2d8bd-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="2d8bd-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="2d8bd-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2d8bd-130">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2d8bd-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2d8bd-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d8bd-131">Property</span></span>     | <span data-ttu-id="2d8bd-132">Тип</span><span class="sxs-lookup"><span data-stu-id="2d8bd-132">Type</span></span>   |<span data-ttu-id="2d8bd-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2d8bd-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d8bd-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="2d8bd-134">accountEnabled</span></span>|<span data-ttu-id="2d8bd-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d8bd-135">Boolean</span></span>| <span data-ttu-id="2d8bd-136">Если учетная запись обеспечена — значение **true**, в противном случае — **false**.</span><span class="sxs-lookup"><span data-stu-id="2d8bd-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="2d8bd-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="2d8bd-137">operatingSystem</span></span>|<span data-ttu-id="2d8bd-138">String</span><span class="sxs-lookup"><span data-stu-id="2d8bd-138">String</span></span>|<span data-ttu-id="2d8bd-139">Тип операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2d8bd-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="2d8bd-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="2d8bd-140">operatingSystemVersion</span></span>|<span data-ttu-id="2d8bd-141">String</span><span class="sxs-lookup"><span data-stu-id="2d8bd-141">String</span></span>|<span data-ttu-id="2d8bd-142">Версия операционной системы на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2d8bd-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="2d8bd-143">displayName</span><span class="sxs-lookup"><span data-stu-id="2d8bd-143">displayName</span></span>|<span data-ttu-id="2d8bd-144">String</span><span class="sxs-lookup"><span data-stu-id="2d8bd-144">String</span></span>|<span data-ttu-id="2d8bd-145">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="2d8bd-145">The display name for the device.</span></span>|
|<span data-ttu-id="2d8bd-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="2d8bd-146">isCompliant</span></span>|<span data-ttu-id="2d8bd-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d8bd-147">Boolean</span></span>|<span data-ttu-id="2d8bd-148">Используется значение **true**, если устройство соответствует требованиям политик управления мобильными устройствами (MDM). В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="2d8bd-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="2d8bd-149">С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS.</span><span class="sxs-lookup"><span data-stu-id="2d8bd-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="2d8bd-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="2d8bd-150">isManaged</span></span>|<span data-ttu-id="2d8bd-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d8bd-151">Boolean</span></span>|<span data-ttu-id="2d8bd-152">Используется значение **true**, если устройство контролируется с помощью приложения для управления мобильными устройствами (MDM), например Intune. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="2d8bd-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="2d8bd-153">С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS.</span><span class="sxs-lookup"><span data-stu-id="2d8bd-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

## <a name="response"></a><span data-ttu-id="2d8bd-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d8bd-154">Response</span></span>

<span data-ttu-id="2d8bd-155">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2d8bd-155">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2d8bd-156">Пример</span><span class="sxs-lookup"><span data-stu-id="2d8bd-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d8bd-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d8bd-157">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="2d8bd-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="2d8bd-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
