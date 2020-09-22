---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ae034d3dc0ea92e95d61d52fecda09c9627136e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038495"
---
# <a name="update-user"></a><span data-ttu-id="4cbfa-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="4cbfa-103">Update user</span></span>

<span data-ttu-id="4cbfa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cbfa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4cbfa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4cbfa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cbfa-106">Обновление свойств объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="4cbfa-106">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4cbfa-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4cbfa-107">Prerequisites</span></span>
<span data-ttu-id="4cbfa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cbfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cbfa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cbfa-110">Permission type</span></span>|<span data-ttu-id="4cbfa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cbfa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cbfa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cbfa-112">Delegated (work or school account)</span></span>| <span data-ttu-id="4cbfa-113">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="4cbfa-113">_varies by context_</span></span>|
| <span data-ttu-id="4cbfa-114">&nbsp;&nbsp;Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="4cbfa-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="4cbfa-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cbfa-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="4cbfa-116">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="4cbfa-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="4cbfa-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cbfa-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="4cbfa-118">&nbsp;Входящая миграция &nbsp;</span><span class="sxs-lookup"><span data-stu-id="4cbfa-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="4cbfa-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cbfa-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4cbfa-120">&nbsp;&nbsp;Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="4cbfa-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="4cbfa-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cbfa-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="4cbfa-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cbfa-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cbfa-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cbfa-123">Not supported.</span></span>|
|<span data-ttu-id="4cbfa-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cbfa-124">Application</span></span>|<span data-ttu-id="4cbfa-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cbfa-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cbfa-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cbfa-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="4cbfa-127">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4cbfa-127">Request headers</span></span>
|<span data-ttu-id="4cbfa-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4cbfa-128">Header</span></span>|<span data-ttu-id="4cbfa-129">Значение</span><span class="sxs-lookup"><span data-stu-id="4cbfa-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cbfa-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cbfa-130">Authorization</span></span>|<span data-ttu-id="4cbfa-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cbfa-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cbfa-132">Accept</span><span class="sxs-lookup"><span data-stu-id="4cbfa-132">Accept</span></span>|<span data-ttu-id="4cbfa-133">application/json</span><span class="sxs-lookup"><span data-stu-id="4cbfa-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cbfa-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4cbfa-134">Request body</span></span>
<span data-ttu-id="4cbfa-135">В теле запроса добавьте представление объекта [user](../resources/intune-shared-user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4cbfa-135">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="4cbfa-136">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="4cbfa-136">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="4cbfa-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cbfa-137">Property</span></span>|<span data-ttu-id="4cbfa-138">Тип</span><span class="sxs-lookup"><span data-stu-id="4cbfa-138">Type</span></span>|<span data-ttu-id="4cbfa-139">Описание</span><span class="sxs-lookup"><span data-stu-id="4cbfa-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cbfa-140">id</span><span class="sxs-lookup"><span data-stu-id="4cbfa-140">id</span></span>|<span data-ttu-id="4cbfa-141">String</span><span class="sxs-lookup"><span data-stu-id="4cbfa-141">String</span></span>|<span data-ttu-id="4cbfa-142">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="4cbfa-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="4cbfa-143">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="4cbfa-143">**Onboarding**</span></span>|
|<span data-ttu-id="4cbfa-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="4cbfa-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="4cbfa-145">Int32</span><span class="sxs-lookup"><span data-stu-id="4cbfa-145">Int32</span></span>|<span data-ttu-id="4cbfa-146">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="4cbfa-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="4cbfa-147">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="4cbfa-147">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="4cbfa-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cbfa-148">Response</span></span>
<span data-ttu-id="4cbfa-149">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4cbfa-149">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cbfa-150">Пример</span><span class="sxs-lookup"><span data-stu-id="4cbfa-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="4cbfa-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cbfa-151">Request</span></span>
<span data-ttu-id="4cbfa-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cbfa-152">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="4cbfa-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cbfa-153">Response</span></span>
<span data-ttu-id="4cbfa-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4cbfa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```









