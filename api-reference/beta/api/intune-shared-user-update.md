---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f981816f3f59e48e1f4a13d3c06bc442d190950d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49303785"
---
# <a name="update-user"></a><span data-ttu-id="fb86c-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="fb86c-103">Update user</span></span>

<span data-ttu-id="fb86c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb86c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb86c-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fb86c-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fb86c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb86c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb86c-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb86c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb86c-108">Обновление свойств объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="fb86c-108">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb86c-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fb86c-109">Prerequisites</span></span>

<span data-ttu-id="fb86c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb86c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb86c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb86c-112">Permission type</span></span>|<span data-ttu-id="fb86c-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb86c-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb86c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb86c-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fb86c-115">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="fb86c-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="fb86c-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb86c-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="fb86c-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="fb86c-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="fb86c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb86c-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="fb86c-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="fb86c-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="fb86c-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb86c-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="fb86c-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="fb86c-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="fb86c-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb86c-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fb86c-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb86c-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb86c-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb86c-124">Not supported.</span></span>|
|<span data-ttu-id="fb86c-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb86c-125">Application</span></span>||
| <span data-ttu-id="fb86c-126">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="fb86c-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="fb86c-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb86c-127">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="fb86c-128">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="fb86c-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="fb86c-129">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb86c-129">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="fb86c-130">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="fb86c-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="fb86c-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb86c-131">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="fb86c-132">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="fb86c-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="fb86c-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb86c-133">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb86c-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb86c-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="fb86c-135">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fb86c-135">Request headers</span></span>

|<span data-ttu-id="fb86c-136">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb86c-136">Header</span></span>|<span data-ttu-id="fb86c-137">Значение</span><span class="sxs-lookup"><span data-stu-id="fb86c-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb86c-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb86c-138">Authorization</span></span>|<span data-ttu-id="fb86c-139">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb86c-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb86c-140">Accept</span><span class="sxs-lookup"><span data-stu-id="fb86c-140">Accept</span></span>|<span data-ttu-id="fb86c-141">application/json</span><span class="sxs-lookup"><span data-stu-id="fb86c-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb86c-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb86c-142">Request body</span></span>

<span data-ttu-id="fb86c-143">В теле запроса добавьте представление объекта [user](../resources/intune-shared-user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb86c-143">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="fb86c-144">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="fb86c-144">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="fb86c-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb86c-145">Property</span></span>|<span data-ttu-id="fb86c-146">Тип</span><span class="sxs-lookup"><span data-stu-id="fb86c-146">Type</span></span>|<span data-ttu-id="fb86c-147">Описание</span><span class="sxs-lookup"><span data-stu-id="fb86c-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb86c-148">id</span><span class="sxs-lookup"><span data-stu-id="fb86c-148">id</span></span>|<span data-ttu-id="fb86c-149">String</span><span class="sxs-lookup"><span data-stu-id="fb86c-149">String</span></span>|<span data-ttu-id="fb86c-150">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="fb86c-150">Unique identifier of the user.</span></span>|
|<span data-ttu-id="fb86c-151">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="fb86c-151">**Onboarding**</span></span>|
|<span data-ttu-id="fb86c-152">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="fb86c-152">deviceEnrollmentLimit</span></span>|<span data-ttu-id="fb86c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="fb86c-153">Int32</span></span>|<span data-ttu-id="fb86c-154">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="fb86c-154">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="fb86c-155">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="fb86c-155">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="fb86c-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb86c-156">Response</span></span>

<span data-ttu-id="fb86c-157">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fb86c-157">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb86c-158">Пример</span><span class="sxs-lookup"><span data-stu-id="fb86c-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb86c-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb86c-159">Request</span></span>

<span data-ttu-id="fb86c-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb86c-160">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="fb86c-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb86c-161">Response</span></span>

<span data-ttu-id="fb86c-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb86c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```










