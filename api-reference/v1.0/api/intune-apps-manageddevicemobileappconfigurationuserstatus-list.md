---
title: Перечисление объектов managedDeviceMobileAppConfigurationUserStatus
description: Список свойств и связей объектов managedDeviceMobileAppConfigurationUserStatus.
ms.openlocfilehash: 942847216d196eac94a5c7f55bc4f624989c59ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028084"
---
# <a name="list-manageddevicemobileappconfigurationuserstatuses"></a><span data-ttu-id="51955-103">Перечисление объектов managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="51955-103">List managedDeviceMobileAppConfigurationUserStatuses</span></span>

> <span data-ttu-id="51955-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="51955-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51955-105">Список свойств и связей объектов [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="51955-105">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51955-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="51955-106">Prerequisites</span></span>
<span data-ttu-id="51955-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51955-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51955-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51955-109">Permission type</span></span>|<span data-ttu-id="51955-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51955-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51955-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51955-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51955-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="51955-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="51955-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51955-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51955-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51955-114">Not supported.</span></span>|
|<span data-ttu-id="51955-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51955-115">Application</span></span>|<span data-ttu-id="51955-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51955-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51955-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51955-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="51955-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51955-118">Request headers</span></span>
|<span data-ttu-id="51955-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51955-119">Header</span></span>|<span data-ttu-id="51955-120">Значение</span><span class="sxs-lookup"><span data-stu-id="51955-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51955-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="51955-121">Authorization</span></span>|<span data-ttu-id="51955-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="51955-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51955-123">Accept</span><span class="sxs-lookup"><span data-stu-id="51955-123">Accept</span></span>|<span data-ttu-id="51955-124">application/json</span><span class="sxs-lookup"><span data-stu-id="51955-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51955-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51955-125">Request body</span></span>
<span data-ttu-id="51955-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51955-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51955-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="51955-127">Response</span></span>
<span data-ttu-id="51955-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51955-128">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51955-129">Пример</span><span class="sxs-lookup"><span data-stu-id="51955-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="51955-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="51955-130">Request</span></span>
<span data-ttu-id="51955-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51955-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="51955-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="51955-132">Response</span></span>
<span data-ttu-id="51955-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="51955-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



