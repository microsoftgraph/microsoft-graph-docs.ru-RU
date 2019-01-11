---
title: Перечисление объектов managedDeviceMobileAppConfigurationUserStatus
description: Список свойств и связей объектов managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c55c2966aeae77a3f7dd206600f2066745b551b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822521"
---
# <a name="list-manageddevicemobileappconfigurationuserstatuses"></a><span data-ttu-id="f1bf5-103">Перечисление объектов managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="f1bf5-103">List managedDeviceMobileAppConfigurationUserStatuses</span></span>

> <span data-ttu-id="f1bf5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1bf5-105">Список свойств и связей объектов [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="f1bf5-105">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1bf5-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f1bf5-106">Prerequisites</span></span>
<span data-ttu-id="f1bf5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1bf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1bf5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1bf5-109">Permission type</span></span>|<span data-ttu-id="f1bf5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1bf5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1bf5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1bf5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f1bf5-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1bf5-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f1bf5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1bf5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1bf5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-114">Not supported.</span></span>|
|<span data-ttu-id="f1bf5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1bf5-115">Application</span></span>|<span data-ttu-id="f1bf5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1bf5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1bf5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="f1bf5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1bf5-118">Request headers</span></span>
|<span data-ttu-id="f1bf5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1bf5-119">Header</span></span>|<span data-ttu-id="f1bf5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f1bf5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1bf5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1bf5-121">Authorization</span></span>|<span data-ttu-id="f1bf5-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f1bf5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1bf5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f1bf5-123">Accept</span></span>|<span data-ttu-id="f1bf5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f1bf5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1bf5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f1bf5-125">Request body</span></span>
<span data-ttu-id="f1bf5-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1bf5-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1bf5-127">Response</span></span>
<span data-ttu-id="f1bf5-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-128">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1bf5-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f1bf5-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1bf5-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1bf5-130">Request</span></span>
<span data-ttu-id="f1bf5-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="f1bf5-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1bf5-132">Response</span></span>
<span data-ttu-id="f1bf5-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



