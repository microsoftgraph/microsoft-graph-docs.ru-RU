---
title: Получение Манажеддевицеенкриптионстате
description: Чтение свойств и связей объекта Манажеддевицеенкриптионстате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e3efec1b2b80e8fe3ca6830369230ff2f0b8c4bd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709555"
---
# <a name="get-manageddeviceencryptionstate"></a><span data-ttu-id="c2e55-103">Получение Манажеддевицеенкриптионстате</span><span class="sxs-lookup"><span data-stu-id="c2e55-103">Get managedDeviceEncryptionState</span></span>

<span data-ttu-id="c2e55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2e55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2e55-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2e55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2e55-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2e55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2e55-107">Чтение свойств и связей объекта [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="c2e55-107">Read properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2e55-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c2e55-108">Prerequisites</span></span>
<span data-ttu-id="c2e55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2e55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2e55-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2e55-111">Permission type</span></span>|<span data-ttu-id="c2e55-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2e55-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2e55-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2e55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2e55-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2e55-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c2e55-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2e55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2e55-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2e55-116">Not supported.</span></span>|
|<span data-ttu-id="c2e55-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2e55-117">Application</span></span>|<span data-ttu-id="c2e55-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2e55-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2e55-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2e55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c2e55-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2e55-120">Optional query parameters</span></span>
<span data-ttu-id="c2e55-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c2e55-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2e55-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2e55-122">Request headers</span></span>
|<span data-ttu-id="c2e55-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2e55-123">Header</span></span>|<span data-ttu-id="c2e55-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c2e55-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2e55-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2e55-125">Authorization</span></span>|<span data-ttu-id="c2e55-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2e55-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2e55-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c2e55-127">Accept</span></span>|<span data-ttu-id="c2e55-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c2e55-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2e55-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c2e55-129">Request body</span></span>
<span data-ttu-id="c2e55-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2e55-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2e55-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2e55-131">Response</span></span>
<span data-ttu-id="c2e55-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2e55-132">If successful, this method returns a `200 OK` response code and [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2e55-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c2e55-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2e55-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2e55-134">Request</span></span>
<span data-ttu-id="c2e55-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2e55-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

### <a name="response"></a><span data-ttu-id="c2e55-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2e55-136">Response</span></span>
<span data-ttu-id="c2e55-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2e55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 810

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
    "id": "f09b4ab6-4ab6-f09b-b64a-9bf0b64a9bf0",
    "userPrincipalName": "User Principal Name value",
    "deviceType": "windowsRT",
    "osVersion": "Os Version value",
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "deviceName": "Device Name value",
    "encryptionReadinessState": "ready",
    "encryptionState": "encrypted",
    "encryptionPolicySettingState": "notApplicable",
    "advancedBitLockerStates": "noUserConsent",
    "fileVaultStates": "driveEncryptedByUser",
    "policyDetails": [
      {
        "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
        "policyId": "Policy Id value",
        "policyName": "Policy Name value"
      }
    ]
  }
}
```





