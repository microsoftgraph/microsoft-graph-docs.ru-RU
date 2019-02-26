---
title: Создание объекта managedDeviceMobileAppConfigurationUserStatus
description: Создание объекта managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: da46008eee715c7ecff2057015cb0dacb37102b7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251449"
---
# <a name="create-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="012b1-103">Создание объекта managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="012b1-103">Create managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="012b1-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="012b1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="012b1-105">Создание объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="012b1-105">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="012b1-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="012b1-106">Prerequisites</span></span>
<span data-ttu-id="012b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="012b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="012b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="012b1-109">Permission type</span></span>|<span data-ttu-id="012b1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="012b1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="012b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="012b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="012b1-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="012b1-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="012b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="012b1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="012b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="012b1-114">Not supported.</span></span>|
|<span data-ttu-id="012b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="012b1-115">Application</span></span>|<span data-ttu-id="012b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="012b1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="012b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="012b1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="012b1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="012b1-118">Request headers</span></span>
|<span data-ttu-id="012b1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="012b1-119">Header</span></span>|<span data-ttu-id="012b1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="012b1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="012b1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="012b1-121">Authorization</span></span>|<span data-ttu-id="012b1-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="012b1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="012b1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="012b1-123">Accept</span></span>|<span data-ttu-id="012b1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="012b1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="012b1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="012b1-125">Request body</span></span>
<span data-ttu-id="012b1-126">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationUserStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="012b1-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationUserStatus object.</span></span>

<span data-ttu-id="012b1-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="012b1-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationUserStatus.</span></span>

|<span data-ttu-id="012b1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="012b1-128">Property</span></span>|<span data-ttu-id="012b1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="012b1-129">Type</span></span>|<span data-ttu-id="012b1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="012b1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="012b1-131">id</span><span class="sxs-lookup"><span data-stu-id="012b1-131">id</span></span>|<span data-ttu-id="012b1-132">Строка</span><span class="sxs-lookup"><span data-stu-id="012b1-132">String</span></span>|<span data-ttu-id="012b1-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="012b1-133">Key of the entity.</span></span>|
|<span data-ttu-id="012b1-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="012b1-134">userDisplayName</span></span>|<span data-ttu-id="012b1-135">String</span><span class="sxs-lookup"><span data-stu-id="012b1-135">String</span></span>|<span data-ttu-id="012b1-136">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="012b1-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="012b1-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="012b1-137">devicesCount</span></span>|<span data-ttu-id="012b1-138">Int32</span><span class="sxs-lookup"><span data-stu-id="012b1-138">Int32</span></span>|<span data-ttu-id="012b1-139">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="012b1-139">Devices count for that user.</span></span>|
|<span data-ttu-id="012b1-140">status</span><span class="sxs-lookup"><span data-stu-id="012b1-140">status</span></span>|[<span data-ttu-id="012b1-141">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="012b1-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="012b1-142">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="012b1-142">Compliance status of the policy report.</span></span> <span data-ttu-id="012b1-143">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="012b1-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="012b1-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="012b1-144">lastReportedDateTime</span></span>|<span data-ttu-id="012b1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="012b1-145">DateTimeOffset</span></span>|<span data-ttu-id="012b1-146">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="012b1-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="012b1-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="012b1-147">userPrincipalName</span></span>|<span data-ttu-id="012b1-148">String</span><span class="sxs-lookup"><span data-stu-id="012b1-148">String</span></span>|<span data-ttu-id="012b1-149">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="012b1-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="012b1-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="012b1-150">Response</span></span>
<span data-ttu-id="012b1-151">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="012b1-151">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="012b1-152">Пример</span><span class="sxs-lookup"><span data-stu-id="012b1-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="012b1-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="012b1-153">Request</span></span>
<span data-ttu-id="012b1-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="012b1-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="012b1-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="012b1-155">Response</span></span>
<span data-ttu-id="012b1-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="012b1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



