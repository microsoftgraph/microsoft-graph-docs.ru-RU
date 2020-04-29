---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9ff722318d1cc4fff866cd309f08d8ef9c6f60df
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411238"
---
# <a name="update-user"></a><span data-ttu-id="24681-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="24681-103">Update user</span></span>

<span data-ttu-id="24681-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24681-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24681-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24681-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24681-106">Обновление свойств объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="24681-106">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24681-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="24681-107">Prerequisites</span></span>
<span data-ttu-id="24681-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24681-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24681-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24681-110">Permission type</span></span>|<span data-ttu-id="24681-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24681-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24681-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24681-112">Delegated (work or school account)</span></span>| <span data-ttu-id="24681-113">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="24681-113">_varies by context_</span></span>|
| <span data-ttu-id="24681-114">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="24681-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="24681-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24681-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="24681-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="24681-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="24681-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24681-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="24681-118">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="24681-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="24681-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24681-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="24681-120">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="24681-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="24681-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24681-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="24681-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24681-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24681-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24681-123">Not supported.</span></span>|
|<span data-ttu-id="24681-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24681-124">Application</span></span>|<span data-ttu-id="24681-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24681-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24681-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24681-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="24681-127">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="24681-127">Request headers</span></span>
|<span data-ttu-id="24681-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24681-128">Header</span></span>|<span data-ttu-id="24681-129">Значение</span><span class="sxs-lookup"><span data-stu-id="24681-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24681-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24681-130">Authorization</span></span>|<span data-ttu-id="24681-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24681-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24681-132">Accept</span><span class="sxs-lookup"><span data-stu-id="24681-132">Accept</span></span>|<span data-ttu-id="24681-133">application/json</span><span class="sxs-lookup"><span data-stu-id="24681-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24681-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="24681-134">Request body</span></span>
<span data-ttu-id="24681-135">В теле запроса добавьте представление объекта [user](../resources/intune-shared-user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24681-135">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="24681-136">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="24681-136">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="24681-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="24681-137">Property</span></span>|<span data-ttu-id="24681-138">Тип</span><span class="sxs-lookup"><span data-stu-id="24681-138">Type</span></span>|<span data-ttu-id="24681-139">Описание</span><span class="sxs-lookup"><span data-stu-id="24681-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24681-140">id</span><span class="sxs-lookup"><span data-stu-id="24681-140">id</span></span>|<span data-ttu-id="24681-141">String</span><span class="sxs-lookup"><span data-stu-id="24681-141">String</span></span>|<span data-ttu-id="24681-142">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="24681-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="24681-143">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="24681-143">**Onboarding**</span></span>|
|<span data-ttu-id="24681-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="24681-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="24681-145">Int32</span><span class="sxs-lookup"><span data-stu-id="24681-145">Int32</span></span>|<span data-ttu-id="24681-146">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="24681-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="24681-147">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="24681-147">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="24681-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="24681-148">Response</span></span>
<span data-ttu-id="24681-149">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="24681-149">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24681-150">Пример</span><span class="sxs-lookup"><span data-stu-id="24681-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="24681-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="24681-151">Request</span></span>
<span data-ttu-id="24681-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24681-152">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="24681-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="24681-153">Response</span></span>
<span data-ttu-id="24681-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24681-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```






