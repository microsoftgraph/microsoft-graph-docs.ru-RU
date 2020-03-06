---
title: Перечисление объектов managedDeviceMobileAppConfigurationUserStatus
description: Список свойств и связей объектов managedDeviceMobileAppConfigurationUserStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4afd7922a13bba4d8532e7525dfdb6dfceb42fe1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516231"
---
# <a name="list-manageddevicemobileappconfigurationuserstatuses"></a><span data-ttu-id="afbeb-103">Перечисление объектов managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="afbeb-103">List managedDeviceMobileAppConfigurationUserStatuses</span></span>

<span data-ttu-id="afbeb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afbeb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="afbeb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="afbeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afbeb-106">Список свойств и связей объектов [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="afbeb-106">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afbeb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="afbeb-107">Prerequisites</span></span>
<span data-ttu-id="afbeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afbeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afbeb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afbeb-110">Permission type</span></span>|<span data-ttu-id="afbeb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="afbeb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afbeb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afbeb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="afbeb-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="afbeb-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="afbeb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afbeb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afbeb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afbeb-115">Not supported.</span></span>|
|<span data-ttu-id="afbeb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="afbeb-116">Application</span></span>|<span data-ttu-id="afbeb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afbeb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afbeb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afbeb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="afbeb-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="afbeb-119">Request headers</span></span>
|<span data-ttu-id="afbeb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="afbeb-120">Header</span></span>|<span data-ttu-id="afbeb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="afbeb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afbeb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="afbeb-122">Authorization</span></span>|<span data-ttu-id="afbeb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="afbeb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afbeb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="afbeb-124">Accept</span></span>|<span data-ttu-id="afbeb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="afbeb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afbeb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="afbeb-126">Request body</span></span>
<span data-ttu-id="afbeb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="afbeb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afbeb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="afbeb-128">Response</span></span>
<span data-ttu-id="afbeb-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="afbeb-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afbeb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="afbeb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="afbeb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="afbeb-131">Request</span></span>
<span data-ttu-id="afbeb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="afbeb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="afbeb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="afbeb-133">Response</span></span>
<span data-ttu-id="afbeb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="afbeb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




