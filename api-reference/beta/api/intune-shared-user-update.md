---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e2d2dde7b009e735c336ad3260cfb3064b33b6fb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053694"
---
# <a name="update-user"></a><span data-ttu-id="f82b7-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="f82b7-103">Update user</span></span>

<span data-ttu-id="f82b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f82b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f82b7-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f82b7-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f82b7-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f82b7-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f82b7-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f82b7-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f82b7-108">Обновление свойств объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="f82b7-108">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f82b7-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f82b7-109">Prerequisites</span></span>

<span data-ttu-id="f82b7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f82b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f82b7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f82b7-112">Permission type</span></span>|<span data-ttu-id="f82b7-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f82b7-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f82b7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f82b7-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f82b7-115">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="f82b7-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="f82b7-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f82b7-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="f82b7-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="f82b7-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="f82b7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f82b7-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="f82b7-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="f82b7-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f82b7-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f82b7-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="f82b7-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="f82b7-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="f82b7-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f82b7-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f82b7-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f82b7-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f82b7-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f82b7-124">Not supported.</span></span>|
|<span data-ttu-id="f82b7-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f82b7-125">Application</span></span>||
| <span data-ttu-id="f82b7-126">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="f82b7-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="f82b7-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f82b7-127">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="f82b7-128">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="f82b7-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="f82b7-129">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f82b7-129">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="f82b7-130">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="f82b7-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f82b7-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f82b7-131">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="f82b7-132">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="f82b7-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="f82b7-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f82b7-133">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f82b7-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f82b7-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="f82b7-135">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f82b7-135">Request headers</span></span>

|<span data-ttu-id="f82b7-136">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f82b7-136">Header</span></span>|<span data-ttu-id="f82b7-137">Значение</span><span class="sxs-lookup"><span data-stu-id="f82b7-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f82b7-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f82b7-138">Authorization</span></span>|<span data-ttu-id="f82b7-139">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f82b7-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f82b7-140">Accept</span><span class="sxs-lookup"><span data-stu-id="f82b7-140">Accept</span></span>|<span data-ttu-id="f82b7-141">application/json</span><span class="sxs-lookup"><span data-stu-id="f82b7-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f82b7-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f82b7-142">Request body</span></span>

<span data-ttu-id="f82b7-143">В теле запроса добавьте представление объекта [user](../resources/intune-shared-user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f82b7-143">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="f82b7-144">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="f82b7-144">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="f82b7-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="f82b7-145">Property</span></span>|<span data-ttu-id="f82b7-146">Тип</span><span class="sxs-lookup"><span data-stu-id="f82b7-146">Type</span></span>|<span data-ttu-id="f82b7-147">Описание</span><span class="sxs-lookup"><span data-stu-id="f82b7-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f82b7-148">id</span><span class="sxs-lookup"><span data-stu-id="f82b7-148">id</span></span>|<span data-ttu-id="f82b7-149">String</span><span class="sxs-lookup"><span data-stu-id="f82b7-149">String</span></span>|<span data-ttu-id="f82b7-150">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="f82b7-150">Unique identifier of the user.</span></span>|
|<span data-ttu-id="f82b7-151">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="f82b7-151">**Onboarding**</span></span>|
|<span data-ttu-id="f82b7-152">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="f82b7-152">deviceEnrollmentLimit</span></span>|<span data-ttu-id="f82b7-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f82b7-153">Int32</span></span>|<span data-ttu-id="f82b7-154">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="f82b7-154">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="f82b7-155">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="f82b7-155">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="f82b7-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="f82b7-156">Response</span></span>

<span data-ttu-id="f82b7-157">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f82b7-157">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f82b7-158">Пример</span><span class="sxs-lookup"><span data-stu-id="f82b7-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="f82b7-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="f82b7-159">Request</span></span>

<span data-ttu-id="f82b7-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f82b7-160">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="f82b7-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="f82b7-161">Response</span></span>

<span data-ttu-id="f82b7-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f82b7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```












