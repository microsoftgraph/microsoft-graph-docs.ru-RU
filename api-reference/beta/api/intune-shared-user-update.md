---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3c50772b1c461c37b2152e9451bf6c746a8c8278
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865070"
---
# <a name="update-user"></a><span data-ttu-id="c1588-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="c1588-103">Update user</span></span>

<span data-ttu-id="c1588-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1588-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1588-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="c1588-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c1588-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1588-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1588-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1588-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1588-108">Обновление свойств объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="c1588-108">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1588-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c1588-109">Prerequisites</span></span>

<span data-ttu-id="c1588-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1588-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1588-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1588-112">Permission type</span></span>|<span data-ttu-id="c1588-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1588-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1588-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1588-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c1588-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c1588-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c1588-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1588-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="c1588-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c1588-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c1588-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1588-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c1588-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c1588-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c1588-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1588-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="c1588-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="c1588-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c1588-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1588-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c1588-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1588-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1588-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1588-124">Not supported.</span></span>|
|<span data-ttu-id="c1588-125">Для приложения</span><span class="sxs-lookup"><span data-stu-id="c1588-125">Application</span></span>||
| <span data-ttu-id="c1588-126">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c1588-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c1588-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1588-127">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="c1588-128">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c1588-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c1588-129">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1588-129">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c1588-130">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c1588-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c1588-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1588-131">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="c1588-132">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="c1588-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c1588-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1588-133">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1588-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1588-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="c1588-135">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c1588-135">Request headers</span></span>

|<span data-ttu-id="c1588-136">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1588-136">Header</span></span>|<span data-ttu-id="c1588-137">Значение</span><span class="sxs-lookup"><span data-stu-id="c1588-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1588-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1588-138">Authorization</span></span>|<span data-ttu-id="c1588-139">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1588-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1588-140">Accept</span><span class="sxs-lookup"><span data-stu-id="c1588-140">Accept</span></span>|<span data-ttu-id="c1588-141">application/json</span><span class="sxs-lookup"><span data-stu-id="c1588-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1588-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1588-142">Request body</span></span>

<span data-ttu-id="c1588-143">В теле запроса добавьте представление объекта [user](../resources/intune-shared-user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1588-143">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="c1588-144">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="c1588-144">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="c1588-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1588-145">Property</span></span>|<span data-ttu-id="c1588-146">Тип</span><span class="sxs-lookup"><span data-stu-id="c1588-146">Type</span></span>|<span data-ttu-id="c1588-147">Описание</span><span class="sxs-lookup"><span data-stu-id="c1588-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1588-148">id</span><span class="sxs-lookup"><span data-stu-id="c1588-148">id</span></span>|<span data-ttu-id="c1588-149">String</span><span class="sxs-lookup"><span data-stu-id="c1588-149">String</span></span>|<span data-ttu-id="c1588-150">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="c1588-150">Unique identifier of the user.</span></span>|
|<span data-ttu-id="c1588-151">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c1588-151">**Onboarding**</span></span>|
|<span data-ttu-id="c1588-152">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="c1588-152">deviceEnrollmentLimit</span></span>|<span data-ttu-id="c1588-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c1588-153">Int32</span></span>|<span data-ttu-id="c1588-154">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="c1588-154">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="c1588-155">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="c1588-155">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="c1588-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1588-156">Response</span></span>

<span data-ttu-id="c1588-157">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c1588-157">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1588-158">Пример</span><span class="sxs-lookup"><span data-stu-id="c1588-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1588-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1588-159">Request</span></span>

<span data-ttu-id="c1588-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1588-160">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="c1588-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1588-161">Response</span></span>

<span data-ttu-id="c1588-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1588-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```










