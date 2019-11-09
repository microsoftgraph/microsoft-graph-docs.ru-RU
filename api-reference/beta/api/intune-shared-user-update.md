---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: afc9aed4595816766fe542c8f1a8af480bf0f2bc
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085523"
---
# <a name="update-user"></a><span data-ttu-id="7206d-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="7206d-103">Update user</span></span>

> <span data-ttu-id="7206d-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7206d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7206d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7206d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7206d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7206d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7206d-107">Обновление свойств объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="7206d-107">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7206d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7206d-108">Prerequisites</span></span>

<span data-ttu-id="7206d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7206d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7206d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7206d-111">Permission type</span></span>|<span data-ttu-id="7206d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7206d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7206d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7206d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7206d-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="7206d-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="7206d-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7206d-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="7206d-116">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="7206d-116">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="7206d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7206d-117">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="7206d-118">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="7206d-118">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7206d-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7206d-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="7206d-120">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="7206d-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="7206d-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7206d-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7206d-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7206d-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7206d-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7206d-123">Not supported.</span></span>|
|<span data-ttu-id="7206d-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7206d-124">Application</span></span>||
| <span data-ttu-id="7206d-125">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="7206d-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="7206d-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7206d-126">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="7206d-127">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="7206d-127">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="7206d-128">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7206d-128">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="7206d-129">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="7206d-129">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7206d-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7206d-130">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="7206d-131">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="7206d-131">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="7206d-132">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7206d-132">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7206d-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7206d-133">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="7206d-134">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7206d-134">Request headers</span></span>

|<span data-ttu-id="7206d-135">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7206d-135">Header</span></span>|<span data-ttu-id="7206d-136">Значение</span><span class="sxs-lookup"><span data-stu-id="7206d-136">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7206d-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7206d-137">Authorization</span></span>|<span data-ttu-id="7206d-138">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7206d-138">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7206d-139">Accept</span><span class="sxs-lookup"><span data-stu-id="7206d-139">Accept</span></span>|<span data-ttu-id="7206d-140">application/json</span><span class="sxs-lookup"><span data-stu-id="7206d-140">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7206d-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7206d-141">Request body</span></span>

<span data-ttu-id="7206d-142">В теле запроса добавьте представление объекта [user](../resources/intune-shared-user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7206d-142">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="7206d-143">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="7206d-143">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="7206d-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="7206d-144">Property</span></span>|<span data-ttu-id="7206d-145">Тип</span><span class="sxs-lookup"><span data-stu-id="7206d-145">Type</span></span>|<span data-ttu-id="7206d-146">Описание</span><span class="sxs-lookup"><span data-stu-id="7206d-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7206d-147">id</span><span class="sxs-lookup"><span data-stu-id="7206d-147">id</span></span>|<span data-ttu-id="7206d-148">String</span><span class="sxs-lookup"><span data-stu-id="7206d-148">String</span></span>|<span data-ttu-id="7206d-149">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="7206d-149">Unique identifier of the user.</span></span>|
|<span data-ttu-id="7206d-150">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="7206d-150">**Onboarding**</span></span>|
|<span data-ttu-id="7206d-151">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="7206d-151">deviceEnrollmentLimit</span></span>|<span data-ttu-id="7206d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7206d-152">Int32</span></span>|<span data-ttu-id="7206d-153">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="7206d-153">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="7206d-154">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="7206d-154">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="7206d-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="7206d-155">Response</span></span>

<span data-ttu-id="7206d-156">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7206d-156">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7206d-157">Пример</span><span class="sxs-lookup"><span data-stu-id="7206d-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="7206d-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="7206d-158">Request</span></span>

<span data-ttu-id="7206d-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7206d-159">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="7206d-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="7206d-160">Response</span></span>

<span data-ttu-id="7206d-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7206d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```












