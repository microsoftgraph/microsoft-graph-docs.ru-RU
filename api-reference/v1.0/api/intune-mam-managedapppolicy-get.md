---
title: Get managedAppPolicy
description: Чтение свойств и связей объекта managedAppPolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7c2bb4b6b9db1ba919c7407c42a381a49ee8af12
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43399061"
---
# <a name="get-managedapppolicy"></a><span data-ttu-id="91300-103">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="91300-103">Get managedAppPolicy</span></span>

<span data-ttu-id="91300-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91300-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91300-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91300-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91300-106">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="91300-106">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91300-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="91300-107">Prerequisites</span></span>
<span data-ttu-id="91300-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91300-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91300-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91300-110">Permission type</span></span>|<span data-ttu-id="91300-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="91300-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91300-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91300-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91300-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="91300-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="91300-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91300-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91300-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91300-115">Not supported.</span></span>|
|<span data-ttu-id="91300-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91300-116">Application</span></span>|<span data-ttu-id="91300-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91300-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91300-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91300-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91300-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="91300-119">Optional query parameters</span></span>
<span data-ttu-id="91300-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="91300-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91300-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91300-121">Request headers</span></span>
|<span data-ttu-id="91300-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91300-122">Header</span></span>|<span data-ttu-id="91300-123">Значение</span><span class="sxs-lookup"><span data-stu-id="91300-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91300-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="91300-124">Authorization</span></span>|<span data-ttu-id="91300-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91300-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91300-126">Accept</span><span class="sxs-lookup"><span data-stu-id="91300-126">Accept</span></span>|<span data-ttu-id="91300-127">application/json</span><span class="sxs-lookup"><span data-stu-id="91300-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91300-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="91300-128">Request body</span></span>
<span data-ttu-id="91300-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91300-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91300-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="91300-130">Response</span></span>
<span data-ttu-id="91300-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="91300-131">If successful, this method returns a `200 OK` response code and [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91300-132">Пример</span><span class="sxs-lookup"><span data-stu-id="91300-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="91300-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="91300-133">Request</span></span>
<span data-ttu-id="91300-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91300-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="91300-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="91300-135">Response</span></span>
<span data-ttu-id="91300-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91300-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 373

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppPolicy",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
    "version": "Version value"
  }
}
```






