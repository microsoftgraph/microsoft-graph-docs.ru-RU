---
title: Список Манажедаллдевицецертификатестатес
description: Список свойств и связей объектов Манажедаллдевицецертификатестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40ecaa24fe803b56fbf4fd94f45df77ed6c15e2b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48065846"
---
# <a name="list-managedalldevicecertificatestates"></a><span data-ttu-id="738cf-103">Список Манажедаллдевицецертификатестатес</span><span class="sxs-lookup"><span data-stu-id="738cf-103">List managedAllDeviceCertificateStates</span></span>

<span data-ttu-id="738cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="738cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="738cf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="738cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="738cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="738cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="738cf-107">Список свойств и связей объектов [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="738cf-107">List properties and relationships of the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="738cf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="738cf-108">Prerequisites</span></span>
<span data-ttu-id="738cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="738cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="738cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="738cf-111">Permission type</span></span>|<span data-ttu-id="738cf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="738cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="738cf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="738cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="738cf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="738cf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="738cf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="738cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="738cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="738cf-116">Not supported.</span></span>|
|<span data-ttu-id="738cf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="738cf-117">Application</span></span>|<span data-ttu-id="738cf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="738cf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="738cf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="738cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="738cf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="738cf-120">Request headers</span></span>
|<span data-ttu-id="738cf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="738cf-121">Header</span></span>|<span data-ttu-id="738cf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="738cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="738cf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="738cf-123">Authorization</span></span>|<span data-ttu-id="738cf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="738cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="738cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="738cf-125">Accept</span></span>|<span data-ttu-id="738cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="738cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="738cf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="738cf-127">Request body</span></span>
<span data-ttu-id="738cf-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="738cf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="738cf-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="738cf-129">Response</span></span>
<span data-ttu-id="738cf-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="738cf-130">If successful, this method returns a `200 OK` response code and a collection of [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="738cf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="738cf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="738cf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="738cf-132">Request</span></span>
<span data-ttu-id="738cf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="738cf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

### <a name="response"></a><span data-ttu-id="738cf-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="738cf-134">Response</span></span>
<span data-ttu-id="738cf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="738cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 958

{
  "value": [
    {
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
  ]
}
```






