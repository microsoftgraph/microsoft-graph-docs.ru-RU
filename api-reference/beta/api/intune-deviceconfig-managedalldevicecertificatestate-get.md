---
title: Получение Манажедаллдевицецертификатестате
description: Чтение свойств и связей объекта Манажедаллдевицецертификатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 879c030e3668c25aef1a18d011c87a22c70f0134
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726127"
---
# <a name="get-managedalldevicecertificatestate"></a><span data-ttu-id="4e043-103">Получение Манажедаллдевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="4e043-103">Get managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="4e043-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e043-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e043-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e043-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e043-106">Чтение свойств и связей объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="4e043-106">Read properties and relationships of the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e043-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4e043-107">Prerequisites</span></span>
<span data-ttu-id="4e043-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e043-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e043-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e043-110">Permission type</span></span>|<span data-ttu-id="4e043-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e043-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e043-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e043-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e043-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e043-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4e043-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e043-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e043-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e043-115">Not supported.</span></span>|
|<span data-ttu-id="4e043-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e043-116">Application</span></span>|<span data-ttu-id="4e043-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e043-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e043-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e043-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e043-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4e043-119">Optional query parameters</span></span>
<span data-ttu-id="4e043-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4e043-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e043-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e043-121">Request headers</span></span>
|<span data-ttu-id="4e043-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e043-122">Header</span></span>|<span data-ttu-id="4e043-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4e043-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e043-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e043-124">Authorization</span></span>|<span data-ttu-id="4e043-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e043-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e043-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4e043-126">Accept</span></span>|<span data-ttu-id="4e043-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4e043-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e043-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e043-128">Request body</span></span>
<span data-ttu-id="4e043-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e043-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e043-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e043-130">Response</span></span>
<span data-ttu-id="4e043-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e043-131">If successful, this method returns a `200 OK` response code and [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e043-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4e043-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e043-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e043-133">Request</span></span>
<span data-ttu-id="4e043-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e043-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="4e043-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e043-135">Response</span></span>
<span data-ttu-id="4e043-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e043-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





