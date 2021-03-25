---
title: УправлениеAllDeviceCertificateState
description: Чтение свойств и связей объекта managedAllDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7c52b786981d9562a215b31d8756a74724dd23d0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155150"
---
# <a name="get-managedalldevicecertificatestate"></a><span data-ttu-id="1098d-103">УправлениеAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="1098d-103">Get managedAllDeviceCertificateState</span></span>

<span data-ttu-id="1098d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1098d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1098d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1098d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1098d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1098d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1098d-107">Чтение свойств и связей [объекта managedAllDeviceCertificateState.](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)</span><span class="sxs-lookup"><span data-stu-id="1098d-107">Read properties and relationships of the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1098d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1098d-108">Prerequisites</span></span>
<span data-ttu-id="1098d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1098d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1098d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1098d-111">Permission type</span></span>|<span data-ttu-id="1098d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1098d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1098d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1098d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1098d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1098d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1098d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1098d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1098d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1098d-116">Not supported.</span></span>|
|<span data-ttu-id="1098d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1098d-117">Application</span></span>|<span data-ttu-id="1098d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1098d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1098d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1098d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1098d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1098d-120">Optional query parameters</span></span>
<span data-ttu-id="1098d-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1098d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1098d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1098d-122">Request headers</span></span>
|<span data-ttu-id="1098d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1098d-123">Header</span></span>|<span data-ttu-id="1098d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="1098d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1098d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1098d-125">Authorization</span></span>|<span data-ttu-id="1098d-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1098d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1098d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1098d-127">Accept</span></span>|<span data-ttu-id="1098d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1098d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1098d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1098d-129">Request body</span></span>
<span data-ttu-id="1098d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1098d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1098d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1098d-131">Response</span></span>
<span data-ttu-id="1098d-132">В случае успешной работы этот метод возвращает код ответа и `200 OK` [управляемый объект ManagedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1098d-132">If successful, this method returns a `200 OK` response code and [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1098d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1098d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1098d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1098d-134">Request</span></span>
<span data-ttu-id="1098d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1098d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="1098d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1098d-136">Response</span></span>
<span data-ttu-id="1098d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1098d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 916

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
    "id": "987c6a17-6a17-987c-176a-7c98176a7c98",
    "certificateRevokeStatus": "pending",
    "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:34.9547208-08:00",
    "managedDeviceDisplayName": "Managed Device Display Name value",
    "userPrincipalName": "User Principal Name value",
    "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
    "certificateIssuerName": "Certificate Issuer Name value",
    "certificateThumbprint": "Certificate Thumbprint value",
    "certificateSerialNumber": "Certificate Serial Number value",
    "certificateSubjectName": "Certificate Subject Name value",
    "certificateKeyUsages": 4,
    "certificateExtendedKeyUsages": "Certificate Extended Key Usages value",
    "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00"
  }
}
```




