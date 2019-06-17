---
title: Get deviceComplianceUserStatus
description: Чтение свойств и связей объекта deviceComplianceUserStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 71a7288ef019386f347113e5d6b18a39cc75da12
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968079"
---
# <a name="get-devicecomplianceuserstatus"></a><span data-ttu-id="2c6f4-103">Get deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="2c6f4-103">Get deviceComplianceUserStatus</span></span>

> <span data-ttu-id="2c6f4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c6f4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c6f4-106">Чтение свойств и связей объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="2c6f4-106">Read properties and relationships of the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c6f4-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2c6f4-107">Prerequisites</span></span>
<span data-ttu-id="2c6f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c6f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c6f4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c6f4-110">Permission type</span></span>|<span data-ttu-id="2c6f4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c6f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c6f4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c6f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c6f4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c6f4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2c6f4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c6f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c6f4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-115">Not supported.</span></span>|
|<span data-ttu-id="2c6f4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c6f4-116">Application</span></span>|<span data-ttu-id="2c6f4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c6f4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c6f4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c6f4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2c6f4-119">Optional query parameters</span></span>
<span data-ttu-id="2c6f4-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c6f4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c6f4-121">Request headers</span></span>
|<span data-ttu-id="2c6f4-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c6f4-122">Header</span></span>|<span data-ttu-id="2c6f4-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2c6f4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c6f4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c6f4-124">Authorization</span></span>|<span data-ttu-id="2c6f4-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c6f4-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2c6f4-126">Accept</span></span>|<span data-ttu-id="2c6f4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2c6f4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c6f4-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2c6f4-128">Request body</span></span>
<span data-ttu-id="2c6f4-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c6f4-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="2c6f4-130">Response</span></span>
<span data-ttu-id="2c6f4-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-131">If successful, this method returns a `200 OK` response code and [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c6f4-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2c6f4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c6f4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c6f4-133">Request</span></span>
<span data-ttu-id="2c6f4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

### <a name="response"></a><span data-ttu-id="2c6f4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c6f4-135">Response</span></span>
<span data-ttu-id="2c6f4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





