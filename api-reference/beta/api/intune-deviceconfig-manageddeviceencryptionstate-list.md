---
title: Список Манажеддевицеенкриптионстатес
description: Список свойств и связей объектов Манажеддевицеенкриптионстате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b41d70a4456934edef1e42a8e060d8afe00fc49a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518193"
---
# <a name="list-manageddeviceencryptionstates"></a><span data-ttu-id="c774e-103">Список Манажеддевицеенкриптионстатес</span><span class="sxs-lookup"><span data-stu-id="c774e-103">List managedDeviceEncryptionStates</span></span>

> <span data-ttu-id="c774e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c774e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c774e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c774e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c774e-106">Список свойств и связей объектов [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="c774e-106">List properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c774e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c774e-107">Prerequisites</span></span>
<span data-ttu-id="c774e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c774e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c774e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c774e-110">Permission type</span></span>|<span data-ttu-id="c774e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c774e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c774e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c774e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c774e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c774e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c774e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c774e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c774e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c774e-115">Not supported.</span></span>|
|<span data-ttu-id="c774e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c774e-116">Application</span></span>|<span data-ttu-id="c774e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c774e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c774e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c774e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceEncryptionStates
```

## <a name="request-headers"></a><span data-ttu-id="c774e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c774e-119">Request headers</span></span>
|<span data-ttu-id="c774e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c774e-120">Header</span></span>|<span data-ttu-id="c774e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c774e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c774e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c774e-122">Authorization</span></span>|<span data-ttu-id="c774e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c774e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c774e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c774e-124">Accept</span></span>|<span data-ttu-id="c774e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c774e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c774e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c774e-126">Request body</span></span>
<span data-ttu-id="c774e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c774e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c774e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c774e-128">Response</span></span>
<span data-ttu-id="c774e-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c774e-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c774e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c774e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c774e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c774e-131">Request</span></span>
<span data-ttu-id="c774e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c774e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates
```

### <a name="response"></a><span data-ttu-id="c774e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c774e-133">Response</span></span>
<span data-ttu-id="c774e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c774e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 812

{
  "value": [
    {
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
  ]
}
```





