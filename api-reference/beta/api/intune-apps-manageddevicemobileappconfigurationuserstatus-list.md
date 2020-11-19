---
title: Перечисление объектов managedDeviceMobileAppConfigurationUserStatus
description: Список свойств и связей объектов managedDeviceMobileAppConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5bdcb1a2fee42c4b44c51a9671a5f61623dbaf7d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49250004"
---
# <a name="list-manageddevicemobileappconfigurationuserstatuses"></a><span data-ttu-id="48104-103">Перечисление объектов managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="48104-103">List managedDeviceMobileAppConfigurationUserStatuses</span></span>

<span data-ttu-id="48104-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48104-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48104-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48104-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48104-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48104-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48104-107">Список свойств и связей объектов [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="48104-107">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48104-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="48104-108">Prerequisites</span></span>
<span data-ttu-id="48104-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48104-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48104-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48104-111">Permission type</span></span>|<span data-ttu-id="48104-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48104-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48104-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48104-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48104-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="48104-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="48104-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48104-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48104-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48104-116">Not supported.</span></span>|
|<span data-ttu-id="48104-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="48104-117">Application</span></span>|<span data-ttu-id="48104-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="48104-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48104-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48104-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="48104-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="48104-120">Request headers</span></span>
|<span data-ttu-id="48104-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48104-121">Header</span></span>|<span data-ttu-id="48104-122">Значение</span><span class="sxs-lookup"><span data-stu-id="48104-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48104-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48104-123">Authorization</span></span>|<span data-ttu-id="48104-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48104-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48104-125">Accept</span><span class="sxs-lookup"><span data-stu-id="48104-125">Accept</span></span>|<span data-ttu-id="48104-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48104-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48104-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48104-127">Request body</span></span>
<span data-ttu-id="48104-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48104-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48104-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="48104-129">Response</span></span>
<span data-ttu-id="48104-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48104-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48104-131">Пример</span><span class="sxs-lookup"><span data-stu-id="48104-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="48104-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="48104-132">Request</span></span>
<span data-ttu-id="48104-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48104-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="48104-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="48104-134">Response</span></span>
<span data-ttu-id="48104-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48104-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 416

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
      "id": "44960944-0944-4496-4409-964444099644",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




