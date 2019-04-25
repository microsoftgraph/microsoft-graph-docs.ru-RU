---
title: Get deviceComplianceUserStatus
description: Чтение свойств и связей объекта deviceComplianceUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dac610a6b8747f7e7b02c8dd857bb9291982cd51
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578045"
---
# <a name="get-devicecomplianceuserstatus"></a><span data-ttu-id="fd7db-103">Get deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="fd7db-103">Get deviceComplianceUserStatus</span></span>

> <span data-ttu-id="fd7db-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd7db-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd7db-105">Чтение свойств и связей объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="fd7db-105">Read properties and relationships of the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd7db-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fd7db-106">Prerequisites</span></span>
<span data-ttu-id="fd7db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd7db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd7db-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd7db-109">Permission type</span></span>|<span data-ttu-id="fd7db-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd7db-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd7db-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd7db-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fd7db-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd7db-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fd7db-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd7db-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd7db-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd7db-114">Not supported.</span></span>|
|<span data-ttu-id="fd7db-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd7db-115">Application</span></span>|<span data-ttu-id="fd7db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd7db-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd7db-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd7db-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd7db-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fd7db-118">Optional query parameters</span></span>
<span data-ttu-id="fd7db-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fd7db-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd7db-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd7db-120">Request headers</span></span>
|<span data-ttu-id="fd7db-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd7db-121">Header</span></span>|<span data-ttu-id="fd7db-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fd7db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd7db-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd7db-123">Authorization</span></span>|<span data-ttu-id="fd7db-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd7db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd7db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fd7db-125">Accept</span></span>|<span data-ttu-id="fd7db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fd7db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd7db-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd7db-127">Request body</span></span>
<span data-ttu-id="fd7db-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fd7db-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd7db-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd7db-129">Response</span></span>
<span data-ttu-id="fd7db-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fd7db-130">If successful, this method returns a `200 OK` response code and [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd7db-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fd7db-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd7db-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd7db-132">Request</span></span>
<span data-ttu-id="fd7db-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd7db-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

### <a name="response"></a><span data-ttu-id="fd7db-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd7db-134">Response</span></span>
<span data-ttu-id="fd7db-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd7db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 369

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
    "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
    "userDisplayName": "User Display Name value",
    "devicesCount": 12,
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



