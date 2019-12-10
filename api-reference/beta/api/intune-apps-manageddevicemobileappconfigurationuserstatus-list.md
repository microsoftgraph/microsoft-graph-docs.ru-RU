---
title: Перечисление объектов managedDeviceMobileAppConfigurationUserStatus
description: Список свойств и связей объектов managedDeviceMobileAppConfigurationUserStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 405a51d1ef98bdd84baefc8f84bba41a5512f39b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39936894"
---
# <a name="list-manageddevicemobileappconfigurationuserstatuses"></a><span data-ttu-id="83f14-103">Перечисление объектов managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="83f14-103">List managedDeviceMobileAppConfigurationUserStatuses</span></span>

> <span data-ttu-id="83f14-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83f14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83f14-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83f14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83f14-106">Список свойств и связей объектов [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="83f14-106">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83f14-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="83f14-107">Prerequisites</span></span>
<span data-ttu-id="83f14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83f14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83f14-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83f14-110">Permission type</span></span>|<span data-ttu-id="83f14-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="83f14-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83f14-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83f14-112">Delegated (work or school account)</span></span>|<span data-ttu-id="83f14-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="83f14-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="83f14-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83f14-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83f14-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83f14-115">Not supported.</span></span>|
|<span data-ttu-id="83f14-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83f14-116">Application</span></span>|<span data-ttu-id="83f14-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="83f14-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83f14-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83f14-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="83f14-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="83f14-119">Request headers</span></span>
|<span data-ttu-id="83f14-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="83f14-120">Header</span></span>|<span data-ttu-id="83f14-121">Значение</span><span class="sxs-lookup"><span data-stu-id="83f14-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83f14-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83f14-122">Authorization</span></span>|<span data-ttu-id="83f14-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83f14-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83f14-124">Accept</span><span class="sxs-lookup"><span data-stu-id="83f14-124">Accept</span></span>|<span data-ttu-id="83f14-125">application/json</span><span class="sxs-lookup"><span data-stu-id="83f14-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83f14-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="83f14-126">Request body</span></span>
<span data-ttu-id="83f14-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="83f14-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83f14-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="83f14-128">Response</span></span>
<span data-ttu-id="83f14-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="83f14-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83f14-130">Пример</span><span class="sxs-lookup"><span data-stu-id="83f14-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="83f14-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="83f14-131">Request</span></span>
<span data-ttu-id="83f14-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83f14-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="83f14-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="83f14-133">Response</span></span>
<span data-ttu-id="83f14-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83f14-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





