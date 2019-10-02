---
title: Создание объекта managedDeviceMobileAppConfigurationUserStatus
description: Создание объекта managedDeviceMobileAppConfigurationUserStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d93870efa0ec2e488fb56c01497b1754380a2100
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358573"
---
# <a name="create-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="72258-103">Создание объекта managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="72258-103">Create managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="72258-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72258-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72258-105">Создание объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="72258-105">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72258-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="72258-106">Prerequisites</span></span>
<span data-ttu-id="72258-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72258-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72258-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72258-109">Permission type</span></span>|<span data-ttu-id="72258-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="72258-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72258-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72258-111">Delegated (work or school account)</span></span>|<span data-ttu-id="72258-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72258-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="72258-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72258-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72258-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72258-114">Not supported.</span></span>|
|<span data-ttu-id="72258-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72258-115">Application</span></span>|<span data-ttu-id="72258-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72258-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72258-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72258-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="72258-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72258-118">Request headers</span></span>
|<span data-ttu-id="72258-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72258-119">Header</span></span>|<span data-ttu-id="72258-120">Значение</span><span class="sxs-lookup"><span data-stu-id="72258-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72258-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72258-121">Authorization</span></span>|<span data-ttu-id="72258-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72258-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72258-123">Accept</span><span class="sxs-lookup"><span data-stu-id="72258-123">Accept</span></span>|<span data-ttu-id="72258-124">application/json</span><span class="sxs-lookup"><span data-stu-id="72258-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72258-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72258-125">Request body</span></span>
<span data-ttu-id="72258-126">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationUserStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72258-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationUserStatus object.</span></span>

<span data-ttu-id="72258-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="72258-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationUserStatus.</span></span>

|<span data-ttu-id="72258-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="72258-128">Property</span></span>|<span data-ttu-id="72258-129">Тип</span><span class="sxs-lookup"><span data-stu-id="72258-129">Type</span></span>|<span data-ttu-id="72258-130">Описание</span><span class="sxs-lookup"><span data-stu-id="72258-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72258-131">id</span><span class="sxs-lookup"><span data-stu-id="72258-131">id</span></span>|<span data-ttu-id="72258-132">Строка</span><span class="sxs-lookup"><span data-stu-id="72258-132">String</span></span>|<span data-ttu-id="72258-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="72258-133">Key of the entity.</span></span>|
|<span data-ttu-id="72258-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="72258-134">userDisplayName</span></span>|<span data-ttu-id="72258-135">String</span><span class="sxs-lookup"><span data-stu-id="72258-135">String</span></span>|<span data-ttu-id="72258-136">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="72258-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="72258-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="72258-137">devicesCount</span></span>|<span data-ttu-id="72258-138">Int32</span><span class="sxs-lookup"><span data-stu-id="72258-138">Int32</span></span>|<span data-ttu-id="72258-139">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="72258-139">Devices count for that user.</span></span>|
|<span data-ttu-id="72258-140">status</span><span class="sxs-lookup"><span data-stu-id="72258-140">status</span></span>|[<span data-ttu-id="72258-141">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="72258-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="72258-142">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="72258-142">Compliance status of the policy report.</span></span> <span data-ttu-id="72258-143">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="72258-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="72258-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="72258-144">lastReportedDateTime</span></span>|<span data-ttu-id="72258-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72258-145">DateTimeOffset</span></span>|<span data-ttu-id="72258-146">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="72258-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="72258-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="72258-147">userPrincipalName</span></span>|<span data-ttu-id="72258-148">String</span><span class="sxs-lookup"><span data-stu-id="72258-148">String</span></span>|<span data-ttu-id="72258-149">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="72258-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="72258-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="72258-150">Response</span></span>
<span data-ttu-id="72258-151">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72258-151">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72258-152">Пример</span><span class="sxs-lookup"><span data-stu-id="72258-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="72258-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="72258-153">Request</span></span>
<span data-ttu-id="72258-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72258-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="72258-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="72258-155">Response</span></span>
<span data-ttu-id="72258-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72258-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "id": "44960944-0944-4496-4409-964444099644",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




