---
title: List deviceComplianceUserStatuses
description: Перечисление свойств и связей объектов deviceComplianceUserStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8160e0bb4016c88ea8177c6f3f48729c15902de9
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949506"
---
# <a name="list-devicecomplianceuserstatuses"></a><span data-ttu-id="ea7ce-103">List deviceComplianceUserStatuses</span><span class="sxs-lookup"><span data-stu-id="ea7ce-103">List deviceComplianceUserStatuses</span></span>

> <span data-ttu-id="ea7ce-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea7ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea7ce-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea7ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea7ce-106">Перечисление свойств и связей объектов [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="ea7ce-106">List properties and relationships of the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea7ce-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ea7ce-107">Prerequisites</span></span>
<span data-ttu-id="ea7ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea7ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea7ce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea7ce-110">Permission type</span></span>|<span data-ttu-id="ea7ce-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea7ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea7ce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea7ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ea7ce-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea7ce-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ea7ce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea7ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea7ce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea7ce-115">Not supported.</span></span>|
|<span data-ttu-id="ea7ce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea7ce-116">Application</span></span>|<span data-ttu-id="ea7ce-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea7ce-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea7ce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea7ce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ea7ce-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ea7ce-119">Request headers</span></span>
|<span data-ttu-id="ea7ce-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea7ce-120">Header</span></span>|<span data-ttu-id="ea7ce-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ea7ce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea7ce-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea7ce-122">Authorization</span></span>|<span data-ttu-id="ea7ce-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea7ce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea7ce-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ea7ce-124">Accept</span></span>|<span data-ttu-id="ea7ce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ea7ce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea7ce-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ea7ce-126">Request body</span></span>
<span data-ttu-id="ea7ce-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea7ce-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea7ce-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea7ce-128">Response</span></span>
<span data-ttu-id="ea7ce-129">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ea7ce-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea7ce-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ea7ce-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea7ce-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea7ce-131">Request</span></span>
<span data-ttu-id="ea7ce-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea7ce-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="ea7ce-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea7ce-133">Response</span></span>
<span data-ttu-id="ea7ce-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea7ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 397

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
      "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





