---
title: Создание объекта managedDeviceMobileAppConfigurationUserStatus
description: Создание объекта managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 31ba14dc9ceffebd0d30522e0dd9adba16990377
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892451"
---
# <a name="create-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="f0c86-103">Создание объекта managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="f0c86-103">Create managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="f0c86-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f0c86-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0c86-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0c86-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0c86-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f0c86-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0c86-107">Создание объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="f0c86-107">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0c86-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f0c86-108">Prerequisites</span></span>
<span data-ttu-id="f0c86-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0c86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0c86-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0c86-111">Permission type</span></span>|<span data-ttu-id="f0c86-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0c86-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0c86-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0c86-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0c86-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0c86-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f0c86-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0c86-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0c86-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0c86-116">Not supported.</span></span>|
|<span data-ttu-id="f0c86-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0c86-117">Application</span></span>|<span data-ttu-id="f0c86-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0c86-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0c86-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0c86-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="f0c86-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0c86-120">Request headers</span></span>
|<span data-ttu-id="f0c86-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0c86-121">Header</span></span>|<span data-ttu-id="f0c86-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f0c86-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0c86-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0c86-123">Authorization</span></span>|<span data-ttu-id="f0c86-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f0c86-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0c86-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0c86-125">Accept</span></span>|<span data-ttu-id="f0c86-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0c86-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0c86-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0c86-127">Request body</span></span>
<span data-ttu-id="f0c86-128">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationUserStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0c86-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationUserStatus object.</span></span>

<span data-ttu-id="f0c86-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="f0c86-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationUserStatus.</span></span>

|<span data-ttu-id="f0c86-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0c86-130">Property</span></span>|<span data-ttu-id="f0c86-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f0c86-131">Type</span></span>|<span data-ttu-id="f0c86-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f0c86-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0c86-133">id</span><span class="sxs-lookup"><span data-stu-id="f0c86-133">id</span></span>|<span data-ttu-id="f0c86-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f0c86-134">String</span></span>|<span data-ttu-id="f0c86-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f0c86-135">Key of the entity.</span></span>|
|<span data-ttu-id="f0c86-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f0c86-136">userDisplayName</span></span>|<span data-ttu-id="f0c86-137">String</span><span class="sxs-lookup"><span data-stu-id="f0c86-137">String</span></span>|<span data-ttu-id="f0c86-138">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="f0c86-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="f0c86-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="f0c86-139">devicesCount</span></span>|<span data-ttu-id="f0c86-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f0c86-140">Int32</span></span>|<span data-ttu-id="f0c86-141">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="f0c86-141">Devices count for that user.</span></span>|
|<span data-ttu-id="f0c86-142">status</span><span class="sxs-lookup"><span data-stu-id="f0c86-142">status</span></span>|[<span data-ttu-id="f0c86-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f0c86-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f0c86-144">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="f0c86-144">Compliance status of the policy report.</span></span> <span data-ttu-id="f0c86-145">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="f0c86-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f0c86-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0c86-146">lastReportedDateTime</span></span>|<span data-ttu-id="f0c86-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0c86-147">DateTimeOffset</span></span>|<span data-ttu-id="f0c86-148">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="f0c86-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="f0c86-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f0c86-149">userPrincipalName</span></span>|<span data-ttu-id="f0c86-150">String</span><span class="sxs-lookup"><span data-stu-id="f0c86-150">String</span></span>|<span data-ttu-id="f0c86-151">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="f0c86-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="f0c86-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0c86-152">Response</span></span>
<span data-ttu-id="f0c86-153">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f0c86-153">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0c86-154">Пример</span><span class="sxs-lookup"><span data-stu-id="f0c86-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0c86-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0c86-155">Request</span></span>
<span data-ttu-id="f0c86-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0c86-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="f0c86-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0c86-157">Response</span></span>
<span data-ttu-id="f0c86-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f0c86-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





