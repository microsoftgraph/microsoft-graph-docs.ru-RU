---
title: Создание объекта deviceConfigurationUserStatus
description: Создание объекта deviceConfigurationUserStatus.
author: tfitzmac
ms.openlocfilehash: 2d12b141fd45b89e7330595594f1110c65f8b4d4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311650"
---
# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="48e46-103">Создание объекта deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="48e46-103">Create deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="48e46-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="48e46-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48e46-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48e46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48e46-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="48e46-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48e46-107">Создание объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="48e46-107">Create a new [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="48e46-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="48e46-108">Prerequisites</span></span>
<span data-ttu-id="48e46-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48e46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48e46-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48e46-111">Permission type</span></span>|<span data-ttu-id="48e46-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48e46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48e46-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48e46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48e46-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48e46-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="48e46-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48e46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48e46-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48e46-116">Not supported.</span></span>|
|<span data-ttu-id="48e46-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48e46-117">Application</span></span>|<span data-ttu-id="48e46-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48e46-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48e46-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48e46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="48e46-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48e46-120">Request headers</span></span>
|<span data-ttu-id="48e46-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48e46-121">Header</span></span>|<span data-ttu-id="48e46-122">Значение</span><span class="sxs-lookup"><span data-stu-id="48e46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48e46-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48e46-123">Authorization</span></span>|<span data-ttu-id="48e46-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="48e46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48e46-125">Accept</span><span class="sxs-lookup"><span data-stu-id="48e46-125">Accept</span></span>|<span data-ttu-id="48e46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48e46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48e46-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48e46-127">Request body</span></span>
<span data-ttu-id="48e46-128">В тексте запроса добавьте представление объекта deviceConfigurationUserStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48e46-128">In the request body, supply a JSON representation for the deviceConfigurationUserStatus object.</span></span>

<span data-ttu-id="48e46-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="48e46-129">The following table shows the properties that are required when you create the deviceConfigurationUserStatus.</span></span>

|<span data-ttu-id="48e46-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="48e46-130">Property</span></span>|<span data-ttu-id="48e46-131">Тип</span><span class="sxs-lookup"><span data-stu-id="48e46-131">Type</span></span>|<span data-ttu-id="48e46-132">Описание</span><span class="sxs-lookup"><span data-stu-id="48e46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48e46-133">id</span><span class="sxs-lookup"><span data-stu-id="48e46-133">id</span></span>|<span data-ttu-id="48e46-134">Строка</span><span class="sxs-lookup"><span data-stu-id="48e46-134">String</span></span>|<span data-ttu-id="48e46-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="48e46-135">Key of the entity.</span></span>|
|<span data-ttu-id="48e46-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="48e46-136">userDisplayName</span></span>|<span data-ttu-id="48e46-137">String</span><span class="sxs-lookup"><span data-stu-id="48e46-137">String</span></span>|<span data-ttu-id="48e46-138">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="48e46-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="48e46-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="48e46-139">devicesCount</span></span>|<span data-ttu-id="48e46-140">Int32</span><span class="sxs-lookup"><span data-stu-id="48e46-140">Int32</span></span>|<span data-ttu-id="48e46-141">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="48e46-141">Devices count for that user.</span></span>|
|<span data-ttu-id="48e46-142">status</span><span class="sxs-lookup"><span data-stu-id="48e46-142">status</span></span>|[<span data-ttu-id="48e46-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="48e46-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="48e46-144">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="48e46-144">Compliance status of the policy report.</span></span> <span data-ttu-id="48e46-145">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="48e46-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="48e46-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="48e46-146">lastReportedDateTime</span></span>|<span data-ttu-id="48e46-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48e46-147">DateTimeOffset</span></span>|<span data-ttu-id="48e46-148">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="48e46-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="48e46-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="48e46-149">userPrincipalName</span></span>|<span data-ttu-id="48e46-150">String</span><span class="sxs-lookup"><span data-stu-id="48e46-150">String</span></span>|<span data-ttu-id="48e46-151">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="48e46-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="48e46-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="48e46-152">Response</span></span>
<span data-ttu-id="48e46-153">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48e46-153">If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48e46-154">Пример</span><span class="sxs-lookup"><span data-stu-id="48e46-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="48e46-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="48e46-155">Request</span></span>
<span data-ttu-id="48e46-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48e46-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="48e46-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="48e46-157">Response</span></span>
<span data-ttu-id="48e46-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="48e46-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





