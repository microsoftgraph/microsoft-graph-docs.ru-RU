---
title: Обновление объекта deviceComplianceUserStatus
description: Обновление свойств объекта deviceComplianceUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cf9d4e8f7da60dd51705f9fce8fd58ee655b4f00
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017632"
---
# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="26b1a-103">Обновление объекта deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="26b1a-103">Update deviceComplianceUserStatus</span></span>

> <span data-ttu-id="26b1a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26b1a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26b1a-105">Обновление свойств объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="26b1a-105">Update the properties of a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26b1a-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="26b1a-106">Prerequisites</span></span>
<span data-ttu-id="26b1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26b1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26b1a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26b1a-109">Permission type</span></span>|<span data-ttu-id="26b1a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="26b1a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26b1a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26b1a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="26b1a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b1a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26b1a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26b1a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26b1a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26b1a-114">Not supported.</span></span>|
|<span data-ttu-id="26b1a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26b1a-115">Application</span></span>|<span data-ttu-id="26b1a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26b1a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26b1a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26b1a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="26b1a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26b1a-118">Request headers</span></span>
|<span data-ttu-id="26b1a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26b1a-119">Header</span></span>|<span data-ttu-id="26b1a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="26b1a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26b1a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26b1a-121">Authorization</span></span>|<span data-ttu-id="26b1a-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26b1a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26b1a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="26b1a-123">Accept</span></span>|<span data-ttu-id="26b1a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="26b1a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26b1a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="26b1a-125">Request body</span></span>
<span data-ttu-id="26b1a-126">В тексте запроса добавьте представление объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26b1a-126">In the request body, supply a JSON representation for the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="26b1a-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="26b1a-127">The following table shows the properties that are required when you create the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

|<span data-ttu-id="26b1a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="26b1a-128">Property</span></span>|<span data-ttu-id="26b1a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="26b1a-129">Type</span></span>|<span data-ttu-id="26b1a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="26b1a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26b1a-131">id</span><span class="sxs-lookup"><span data-stu-id="26b1a-131">id</span></span>|<span data-ttu-id="26b1a-132">Строка</span><span class="sxs-lookup"><span data-stu-id="26b1a-132">String</span></span>|<span data-ttu-id="26b1a-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="26b1a-133">Key of the entity.</span></span>|
|<span data-ttu-id="26b1a-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="26b1a-134">userDisplayName</span></span>|<span data-ttu-id="26b1a-135">String</span><span class="sxs-lookup"><span data-stu-id="26b1a-135">String</span></span>|<span data-ttu-id="26b1a-136">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="26b1a-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="26b1a-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="26b1a-137">devicesCount</span></span>|<span data-ttu-id="26b1a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="26b1a-138">Int32</span></span>|<span data-ttu-id="26b1a-139">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="26b1a-139">Devices count for that user.</span></span>|
|<span data-ttu-id="26b1a-140">status</span><span class="sxs-lookup"><span data-stu-id="26b1a-140">status</span></span>|[<span data-ttu-id="26b1a-141">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="26b1a-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="26b1a-142">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="26b1a-142">Compliance status of the policy report.</span></span> <span data-ttu-id="26b1a-143">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="26b1a-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="26b1a-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="26b1a-144">lastReportedDateTime</span></span>|<span data-ttu-id="26b1a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26b1a-145">DateTimeOffset</span></span>|<span data-ttu-id="26b1a-146">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="26b1a-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="26b1a-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="26b1a-147">userPrincipalName</span></span>|<span data-ttu-id="26b1a-148">String</span><span class="sxs-lookup"><span data-stu-id="26b1a-148">String</span></span>|<span data-ttu-id="26b1a-149">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="26b1a-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="26b1a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="26b1a-150">Response</span></span>
<span data-ttu-id="26b1a-151">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="26b1a-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26b1a-152">Пример</span><span class="sxs-lookup"><span data-stu-id="26b1a-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="26b1a-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="26b1a-153">Request</span></span>
<span data-ttu-id="26b1a-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26b1a-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
Content-type: application/json
Content-length: 287

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="26b1a-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="26b1a-155">Response</span></span>
<span data-ttu-id="26b1a-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26b1a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 336

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



