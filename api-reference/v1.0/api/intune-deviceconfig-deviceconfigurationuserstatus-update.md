---
title: Обновление объекта deviceConfigurationUserStatus
description: Обновление свойств объекта deviceConfigurationUserStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 29ac3e9459c915bdf133451cd88c99d1887dded7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514699"
---
# <a name="update-deviceconfigurationuserstatus"></a><span data-ttu-id="cd826-103">Обновление объекта deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="cd826-103">Update deviceConfigurationUserStatus</span></span>

<span data-ttu-id="cd826-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd826-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd826-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd826-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd826-106">Обновление свойств объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="cd826-106">Update the properties of a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd826-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cd826-107">Prerequisites</span></span>
<span data-ttu-id="cd826-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd826-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd826-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd826-110">Permission type</span></span>|<span data-ttu-id="cd826-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd826-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd826-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd826-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd826-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd826-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cd826-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd826-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd826-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd826-115">Not supported.</span></span>|
|<span data-ttu-id="cd826-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd826-116">Application</span></span>|<span data-ttu-id="cd826-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd826-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd826-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd826-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="cd826-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cd826-119">Request headers</span></span>
|<span data-ttu-id="cd826-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd826-120">Header</span></span>|<span data-ttu-id="cd826-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cd826-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd826-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd826-122">Authorization</span></span>|<span data-ttu-id="cd826-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd826-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd826-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cd826-124">Accept</span></span>|<span data-ttu-id="cd826-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd826-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd826-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd826-126">Request body</span></span>
<span data-ttu-id="cd826-127">В тексте запроса добавьте представление объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd826-127">In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="cd826-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="cd826-128">The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="cd826-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd826-129">Property</span></span>|<span data-ttu-id="cd826-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cd826-130">Type</span></span>|<span data-ttu-id="cd826-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cd826-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd826-132">id</span><span class="sxs-lookup"><span data-stu-id="cd826-132">id</span></span>|<span data-ttu-id="cd826-133">Строка</span><span class="sxs-lookup"><span data-stu-id="cd826-133">String</span></span>|<span data-ttu-id="cd826-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cd826-134">Key of the entity.</span></span>|
|<span data-ttu-id="cd826-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="cd826-135">userDisplayName</span></span>|<span data-ttu-id="cd826-136">String</span><span class="sxs-lookup"><span data-stu-id="cd826-136">String</span></span>|<span data-ttu-id="cd826-137">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="cd826-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="cd826-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="cd826-138">devicesCount</span></span>|<span data-ttu-id="cd826-139">Int32</span><span class="sxs-lookup"><span data-stu-id="cd826-139">Int32</span></span>|<span data-ttu-id="cd826-140">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd826-140">Devices count for that user.</span></span>|
|<span data-ttu-id="cd826-141">status</span><span class="sxs-lookup"><span data-stu-id="cd826-141">status</span></span>|[<span data-ttu-id="cd826-142">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="cd826-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="cd826-143">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="cd826-143">Compliance status of the policy report.</span></span> <span data-ttu-id="cd826-144">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="cd826-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="cd826-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd826-145">lastReportedDateTime</span></span>|<span data-ttu-id="cd826-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd826-146">DateTimeOffset</span></span>|<span data-ttu-id="cd826-147">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="cd826-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="cd826-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cd826-148">userPrincipalName</span></span>|<span data-ttu-id="cd826-149">String</span><span class="sxs-lookup"><span data-stu-id="cd826-149">String</span></span>|<span data-ttu-id="cd826-150">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd826-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="cd826-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd826-151">Response</span></span>
<span data-ttu-id="cd826-152">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cd826-152">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd826-153">Пример</span><span class="sxs-lookup"><span data-stu-id="cd826-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd826-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd826-154">Request</span></span>
<span data-ttu-id="cd826-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd826-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="cd826-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd826-156">Response</span></span>
<span data-ttu-id="cd826-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd826-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




