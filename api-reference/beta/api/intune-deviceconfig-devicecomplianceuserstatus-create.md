---
title: Создание объекта deviceComplianceUserStatus
description: Создание объекта deviceComplianceUserStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9d54dab79522add6713320a7c7130202c4198c88
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949527"
---
# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="8c504-103">Создание объекта deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="8c504-103">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="8c504-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c504-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c504-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c504-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c504-106">Создание объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="8c504-106">Create a new [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c504-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8c504-107">Prerequisites</span></span>
<span data-ttu-id="8c504-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c504-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c504-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c504-110">Permission type</span></span>|<span data-ttu-id="8c504-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c504-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c504-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c504-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8c504-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c504-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8c504-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c504-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c504-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c504-115">Not supported.</span></span>|
|<span data-ttu-id="8c504-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c504-116">Application</span></span>|<span data-ttu-id="8c504-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c504-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c504-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c504-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="8c504-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8c504-119">Request headers</span></span>
|<span data-ttu-id="8c504-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c504-120">Header</span></span>|<span data-ttu-id="8c504-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8c504-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c504-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c504-122">Authorization</span></span>|<span data-ttu-id="8c504-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c504-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c504-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8c504-124">Accept</span></span>|<span data-ttu-id="8c504-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8c504-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c504-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8c504-126">Request body</span></span>
<span data-ttu-id="8c504-127">В тексте запроса добавьте представление объекта deviceComplianceUserStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c504-127">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="8c504-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="8c504-128">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="8c504-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c504-129">Property</span></span>|<span data-ttu-id="8c504-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8c504-130">Type</span></span>|<span data-ttu-id="8c504-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8c504-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c504-132">id</span><span class="sxs-lookup"><span data-stu-id="8c504-132">id</span></span>|<span data-ttu-id="8c504-133">Строка</span><span class="sxs-lookup"><span data-stu-id="8c504-133">String</span></span>|<span data-ttu-id="8c504-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8c504-134">Key of the entity.</span></span>|
|<span data-ttu-id="8c504-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8c504-135">userDisplayName</span></span>|<span data-ttu-id="8c504-136">String</span><span class="sxs-lookup"><span data-stu-id="8c504-136">String</span></span>|<span data-ttu-id="8c504-137">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="8c504-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="8c504-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="8c504-138">devicesCount</span></span>|<span data-ttu-id="8c504-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8c504-139">Int32</span></span>|<span data-ttu-id="8c504-140">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="8c504-140">Devices count for that user.</span></span>|
|<span data-ttu-id="8c504-141">status</span><span class="sxs-lookup"><span data-stu-id="8c504-141">status</span></span>|[<span data-ttu-id="8c504-142">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="8c504-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8c504-143">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="8c504-143">Compliance status of the policy report.</span></span> <span data-ttu-id="8c504-144">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="8c504-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8c504-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c504-145">lastReportedDateTime</span></span>|<span data-ttu-id="8c504-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c504-146">DateTimeOffset</span></span>|<span data-ttu-id="8c504-147">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="8c504-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="8c504-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8c504-148">userPrincipalName</span></span>|<span data-ttu-id="8c504-149">String</span><span class="sxs-lookup"><span data-stu-id="8c504-149">String</span></span>|<span data-ttu-id="8c504-150">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="8c504-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="8c504-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c504-151">Response</span></span>
<span data-ttu-id="8c504-152">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c504-152">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c504-153">Пример</span><span class="sxs-lookup"><span data-stu-id="8c504-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c504-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c504-154">Request</span></span>
<span data-ttu-id="8c504-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c504-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="8c504-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c504-156">Response</span></span>
<span data-ttu-id="8c504-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c504-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





