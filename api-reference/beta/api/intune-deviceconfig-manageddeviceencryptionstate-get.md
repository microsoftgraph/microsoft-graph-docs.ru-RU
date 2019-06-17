---
title: Получение Манажеддевицеенкриптионстате
description: Чтение свойств и связей объекта Манажеддевицеенкриптионстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: edc66636d0a7a781a0336e0e665eb4fdb7f7b182
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962955"
---
# <a name="get-manageddeviceencryptionstate"></a><span data-ttu-id="6fc53-103">Получение Манажеддевицеенкриптионстате</span><span class="sxs-lookup"><span data-stu-id="6fc53-103">Get managedDeviceEncryptionState</span></span>

> <span data-ttu-id="6fc53-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fc53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fc53-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6fc53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fc53-106">Чтение свойств и связей объекта [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="6fc53-106">Read properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fc53-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6fc53-107">Prerequisites</span></span>
<span data-ttu-id="6fc53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fc53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fc53-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6fc53-110">Permission type</span></span>|<span data-ttu-id="6fc53-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6fc53-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fc53-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6fc53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6fc53-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6fc53-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6fc53-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6fc53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fc53-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fc53-115">Not supported.</span></span>|
|<span data-ttu-id="6fc53-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6fc53-116">Application</span></span>|<span data-ttu-id="6fc53-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fc53-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fc53-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6fc53-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6fc53-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6fc53-119">Optional query parameters</span></span>
<span data-ttu-id="6fc53-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6fc53-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6fc53-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6fc53-121">Request headers</span></span>
|<span data-ttu-id="6fc53-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6fc53-122">Header</span></span>|<span data-ttu-id="6fc53-123">Значение</span><span class="sxs-lookup"><span data-stu-id="6fc53-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fc53-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6fc53-124">Authorization</span></span>|<span data-ttu-id="6fc53-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6fc53-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fc53-126">Accept</span><span class="sxs-lookup"><span data-stu-id="6fc53-126">Accept</span></span>|<span data-ttu-id="6fc53-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6fc53-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fc53-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6fc53-128">Request body</span></span>
<span data-ttu-id="6fc53-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6fc53-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fc53-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="6fc53-130">Response</span></span>
<span data-ttu-id="6fc53-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6fc53-131">If successful, this method returns a `200 OK` response code and [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fc53-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6fc53-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fc53-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6fc53-133">Request</span></span>
<span data-ttu-id="6fc53-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6fc53-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

### <a name="response"></a><span data-ttu-id="6fc53-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fc53-135">Response</span></span>
<span data-ttu-id="6fc53-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6fc53-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 762

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





