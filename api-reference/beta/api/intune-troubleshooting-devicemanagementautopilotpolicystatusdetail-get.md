---
title: Получение Девицеманажементаутопилотполицистатусдетаил
description: Чтение свойств и связей объекта Девицеманажементаутопилотполицистатусдетаил.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4103f34951ef939be945f34b2d67da63a7280ee0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443404"
---
# <a name="get-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="6a818-103">Получение Девицеманажементаутопилотполицистатусдетаил</span><span class="sxs-lookup"><span data-stu-id="6a818-103">Get deviceManagementAutopilotPolicyStatusDetail</span></span>

<span data-ttu-id="6a818-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a818-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a818-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a818-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a818-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a818-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a818-107">Чтение свойств и связей объекта [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) .</span><span class="sxs-lookup"><span data-stu-id="6a818-107">Read properties and relationships of the [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a818-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6a818-108">Prerequisites</span></span>
<span data-ttu-id="6a818-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a818-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a818-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a818-111">Permission type</span></span>|<span data-ttu-id="6a818-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a818-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a818-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a818-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a818-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a818-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6a818-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a818-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a818-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a818-116">Not supported.</span></span>|
|<span data-ttu-id="6a818-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a818-117">Application</span></span>|<span data-ttu-id="6a818-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a818-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a818-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a818-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a818-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6a818-120">Optional query parameters</span></span>
<span data-ttu-id="6a818-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6a818-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a818-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a818-122">Request headers</span></span>
|<span data-ttu-id="6a818-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6a818-123">Header</span></span>|<span data-ttu-id="6a818-124">Значение</span><span class="sxs-lookup"><span data-stu-id="6a818-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a818-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a818-125">Authorization</span></span>|<span data-ttu-id="6a818-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a818-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a818-127">Accept</span><span class="sxs-lookup"><span data-stu-id="6a818-127">Accept</span></span>|<span data-ttu-id="6a818-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6a818-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a818-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6a818-129">Request body</span></span>
<span data-ttu-id="6a818-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6a818-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a818-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a818-131">Response</span></span>
<span data-ttu-id="6a818-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a818-132">If successful, this method returns a `200 OK` response code and [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a818-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6a818-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a818-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a818-134">Request</span></span>
<span data-ttu-id="6a818-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a818-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
```

### <a name="response"></a><span data-ttu-id="6a818-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a818-136">Response</span></span>
<span data-ttu-id="6a818-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a818-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 377

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
    "id": "dbe093ee-93ee-dbe0-ee93-e0dbee93e0db",
    "displayName": "Display Name value",
    "policyType": "application",
    "complianceStatus": "compliant",
    "trackedOnEnrollmentStatus": true,
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
  }
}
```



