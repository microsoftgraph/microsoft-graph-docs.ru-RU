---
title: Создание объекта managedDeviceMobileAppConfigurationUserStatus
description: Создание объекта managedDeviceMobileAppConfigurationUserStatus.
ms.openlocfilehash: 94a3cc37cfed0faf36ab0d96026cc61a33b76668
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028087"
---
# <a name="create-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="ddcfa-103">Создание объекта managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ddcfa-103">Create managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="ddcfa-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddcfa-105">Создание объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="ddcfa-105">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ddcfa-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ddcfa-106">Prerequisites</span></span>
<span data-ttu-id="ddcfa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddcfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddcfa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddcfa-109">Permission type</span></span>|<span data-ttu-id="ddcfa-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddcfa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddcfa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddcfa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ddcfa-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddcfa-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ddcfa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddcfa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddcfa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-114">Not supported.</span></span>|
|<span data-ttu-id="ddcfa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddcfa-115">Application</span></span>|<span data-ttu-id="ddcfa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddcfa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddcfa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ddcfa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddcfa-118">Request headers</span></span>
|<span data-ttu-id="ddcfa-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ddcfa-119">Header</span></span>|<span data-ttu-id="ddcfa-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ddcfa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddcfa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddcfa-121">Authorization</span></span>|<span data-ttu-id="ddcfa-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ddcfa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddcfa-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ddcfa-123">Accept</span></span>|<span data-ttu-id="ddcfa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ddcfa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddcfa-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddcfa-125">Request body</span></span>
<span data-ttu-id="ddcfa-126">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationUserStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationUserStatus object.</span></span>

<span data-ttu-id="ddcfa-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationUserStatus.</span></span>

|<span data-ttu-id="ddcfa-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ddcfa-128">Property</span></span>|<span data-ttu-id="ddcfa-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ddcfa-129">Type</span></span>|<span data-ttu-id="ddcfa-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ddcfa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddcfa-131">id</span><span class="sxs-lookup"><span data-stu-id="ddcfa-131">id</span></span>|<span data-ttu-id="ddcfa-132">String</span><span class="sxs-lookup"><span data-stu-id="ddcfa-132">String</span></span>|<span data-ttu-id="ddcfa-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-133">Key of the entity.</span></span>|
|<span data-ttu-id="ddcfa-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ddcfa-134">userDisplayName</span></span>|<span data-ttu-id="ddcfa-135">String</span><span class="sxs-lookup"><span data-stu-id="ddcfa-135">String</span></span>|<span data-ttu-id="ddcfa-136">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="ddcfa-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="ddcfa-137">devicesCount</span></span>|<span data-ttu-id="ddcfa-138">Int32</span><span class="sxs-lookup"><span data-stu-id="ddcfa-138">Int32</span></span>|<span data-ttu-id="ddcfa-139">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-139">Devices count for that user.</span></span>|
|<span data-ttu-id="ddcfa-140">status</span><span class="sxs-lookup"><span data-stu-id="ddcfa-140">status</span></span>|[<span data-ttu-id="ddcfa-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="ddcfa-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ddcfa-142">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-142">Compliance status of the policy report.</span></span> <span data-ttu-id="ddcfa-143">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ddcfa-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddcfa-144">lastReportedDateTime</span></span>|<span data-ttu-id="ddcfa-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddcfa-145">DateTimeOffset</span></span>|<span data-ttu-id="ddcfa-146">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="ddcfa-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ddcfa-147">userPrincipalName</span></span>|<span data-ttu-id="ddcfa-148">String</span><span class="sxs-lookup"><span data-stu-id="ddcfa-148">String</span></span>|<span data-ttu-id="ddcfa-149">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="ddcfa-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddcfa-150">Response</span></span>
<span data-ttu-id="ddcfa-151">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-151">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddcfa-152">Пример</span><span class="sxs-lookup"><span data-stu-id="ddcfa-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="ddcfa-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddcfa-153">Request</span></span>
<span data-ttu-id="ddcfa-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddcfa-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ddcfa-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="ddcfa-155">Response</span></span>
<span data-ttu-id="ddcfa-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ddcfa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



