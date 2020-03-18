---
title: Получение Манажедаллдевицецертификатестате
description: Чтение свойств и связей объекта Манажедаллдевицецертификатестате.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e0fea5b352ce273423754202f55aa3497140bfb4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42743578"
---
# <a name="get-managedalldevicecertificatestate"></a><span data-ttu-id="d58f0-103">Получение Манажедаллдевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="d58f0-103">Get managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="d58f0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d58f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d58f0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d58f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d58f0-106">Чтение свойств и связей объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="d58f0-106">Read properties and relationships of the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d58f0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d58f0-107">Prerequisites</span></span>
<span data-ttu-id="d58f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d58f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d58f0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d58f0-110">Permission type</span></span>|<span data-ttu-id="d58f0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d58f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d58f0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d58f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d58f0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d58f0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d58f0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d58f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d58f0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d58f0-115">Not supported.</span></span>|
|<span data-ttu-id="d58f0-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d58f0-116">Application</span></span>|<span data-ttu-id="d58f0-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d58f0-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d58f0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d58f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d58f0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d58f0-119">Optional query parameters</span></span>
<span data-ttu-id="d58f0-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d58f0-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d58f0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d58f0-121">Request headers</span></span>
|<span data-ttu-id="d58f0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d58f0-122">Header</span></span>|<span data-ttu-id="d58f0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d58f0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d58f0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d58f0-124">Authorization</span></span>|<span data-ttu-id="d58f0-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d58f0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d58f0-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d58f0-126">Accept</span></span>|<span data-ttu-id="d58f0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d58f0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d58f0-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d58f0-128">Request body</span></span>
<span data-ttu-id="d58f0-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d58f0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d58f0-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d58f0-130">Response</span></span>
<span data-ttu-id="d58f0-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d58f0-131">If successful, this method returns a `200 OK` response code and [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d58f0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d58f0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d58f0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d58f0-133">Request</span></span>
<span data-ttu-id="d58f0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d58f0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="d58f0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d58f0-135">Response</span></span>
<span data-ttu-id="d58f0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d58f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 829

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
    "id": "987c6a17-6a17-987c-176a-7c98176a7c98",
    "certificateRevokeStatus": "pending",
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




