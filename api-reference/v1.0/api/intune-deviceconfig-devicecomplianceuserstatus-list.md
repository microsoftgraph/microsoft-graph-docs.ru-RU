---
title: List deviceComplianceUserStatuses
description: Перечисление свойств и связей объектов deviceComplianceUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0a4de93bc1779740a5c9d09ad48f5c25b99fc660
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252191"
---
# <a name="list-devicecomplianceuserstatuses"></a><span data-ttu-id="a0fdd-103">List deviceComplianceUserStatuses</span><span class="sxs-lookup"><span data-stu-id="a0fdd-103">List deviceComplianceUserStatuses</span></span>

> <span data-ttu-id="a0fdd-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0fdd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0fdd-105">Перечисление свойств и связей объектов [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a0fdd-105">List properties and relationships of the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0fdd-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a0fdd-106">Prerequisites</span></span>
<span data-ttu-id="a0fdd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a0fdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a0fdd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0fdd-109">Permission type</span></span>|<span data-ttu-id="a0fdd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0fdd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0fdd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0fdd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a0fdd-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0fdd-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a0fdd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0fdd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0fdd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0fdd-114">Not supported.</span></span>|
|<span data-ttu-id="a0fdd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0fdd-115">Application</span></span>|<span data-ttu-id="a0fdd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0fdd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0fdd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0fdd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a0fdd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0fdd-118">Request headers</span></span>
|<span data-ttu-id="a0fdd-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a0fdd-119">Header</span></span>|<span data-ttu-id="a0fdd-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a0fdd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0fdd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0fdd-121">Authorization</span></span>|<span data-ttu-id="a0fdd-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a0fdd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0fdd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a0fdd-123">Accept</span></span>|<span data-ttu-id="a0fdd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a0fdd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0fdd-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0fdd-125">Request body</span></span>
<span data-ttu-id="a0fdd-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0fdd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0fdd-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0fdd-127">Response</span></span>
<span data-ttu-id="a0fdd-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a0fdd-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0fdd-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a0fdd-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0fdd-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0fdd-130">Request</span></span>
<span data-ttu-id="a0fdd-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0fdd-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="a0fdd-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0fdd-132">Response</span></span>
<span data-ttu-id="a0fdd-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a0fdd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



