---
title: Get deviceComplianceUserStatus
description: Чтение свойств и связей объекта deviceComplianceUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc4fb8836979f4eee52e8883efe9f9f4d9a7020d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32469707"
---
# <a name="get-devicecomplianceuserstatus"></a><span data-ttu-id="8e429-103">Get deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="8e429-103">Get deviceComplianceUserStatus</span></span>

> <span data-ttu-id="8e429-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e429-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e429-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e429-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e429-106">Чтение свойств и связей объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="8e429-106">Read properties and relationships of the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e429-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8e429-107">Prerequisites</span></span>
<span data-ttu-id="8e429-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e429-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e429-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e429-110">Permission type</span></span>|<span data-ttu-id="8e429-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e429-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e429-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e429-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e429-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e429-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8e429-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e429-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e429-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e429-115">Not supported.</span></span>|
|<span data-ttu-id="8e429-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e429-116">Application</span></span>|<span data-ttu-id="8e429-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e429-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e429-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e429-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e429-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8e429-119">Optional query parameters</span></span>
<span data-ttu-id="8e429-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8e429-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e429-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e429-121">Request headers</span></span>
|<span data-ttu-id="8e429-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e429-122">Header</span></span>|<span data-ttu-id="8e429-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8e429-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e429-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e429-124">Authorization</span></span>|<span data-ttu-id="8e429-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e429-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e429-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8e429-126">Accept</span></span>|<span data-ttu-id="8e429-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8e429-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e429-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e429-128">Request body</span></span>
<span data-ttu-id="8e429-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e429-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e429-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e429-130">Response</span></span>
<span data-ttu-id="8e429-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8e429-131">If successful, this method returns a `200 OK` response code and [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e429-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8e429-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e429-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e429-133">Request</span></span>
<span data-ttu-id="8e429-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e429-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

### <a name="response"></a><span data-ttu-id="8e429-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e429-135">Response</span></span>
<span data-ttu-id="8e429-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e429-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





