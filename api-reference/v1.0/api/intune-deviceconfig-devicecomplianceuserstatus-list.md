---
title: List deviceComplianceUserStatuses
description: Перечисление свойств и связей объектов deviceComplianceUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02f8c750b06e934d50ab60ac539ecae0e377b3da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574479"
---
# <a name="list-devicecomplianceuserstatuses"></a><span data-ttu-id="00d4b-103">List deviceComplianceUserStatuses</span><span class="sxs-lookup"><span data-stu-id="00d4b-103">List deviceComplianceUserStatuses</span></span>

> <span data-ttu-id="00d4b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00d4b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00d4b-105">Перечисление свойств и связей объектов [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="00d4b-105">List properties and relationships of the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00d4b-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="00d4b-106">Prerequisites</span></span>
<span data-ttu-id="00d4b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00d4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00d4b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00d4b-109">Permission type</span></span>|<span data-ttu-id="00d4b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00d4b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00d4b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00d4b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="00d4b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="00d4b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="00d4b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00d4b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00d4b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00d4b-114">Not supported.</span></span>|
|<span data-ttu-id="00d4b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00d4b-115">Application</span></span>|<span data-ttu-id="00d4b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00d4b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00d4b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00d4b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="00d4b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00d4b-118">Request headers</span></span>
|<span data-ttu-id="00d4b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00d4b-119">Header</span></span>|<span data-ttu-id="00d4b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="00d4b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00d4b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00d4b-121">Authorization</span></span>|<span data-ttu-id="00d4b-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00d4b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00d4b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="00d4b-123">Accept</span></span>|<span data-ttu-id="00d4b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="00d4b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00d4b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00d4b-125">Request body</span></span>
<span data-ttu-id="00d4b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00d4b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00d4b-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="00d4b-127">Response</span></span>
<span data-ttu-id="00d4b-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="00d4b-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00d4b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="00d4b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="00d4b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="00d4b-130">Request</span></span>
<span data-ttu-id="00d4b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00d4b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="00d4b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="00d4b-132">Response</span></span>
<span data-ttu-id="00d4b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00d4b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



