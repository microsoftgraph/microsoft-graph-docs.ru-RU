---
title: Перечисление объектов deviceCompliancePolicySettingStateSummary
description: Список свойств и связей объектов deviceCompliancePolicySettingStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aecf944340c285e1c24158f3ac31b2474d9652eb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443190"
---
# <a name="list-devicecompliancepolicysettingstatesummaries"></a><span data-ttu-id="86820-103">Перечисление объектов deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="86820-103">List deviceCompliancePolicySettingStateSummaries</span></span>

<span data-ttu-id="86820-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="86820-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86820-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86820-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86820-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86820-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86820-107">Список свойств и связей объектов [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="86820-107">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86820-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="86820-108">Prerequisites</span></span>
<span data-ttu-id="86820-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86820-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86820-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86820-111">Permission type</span></span>|<span data-ttu-id="86820-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="86820-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86820-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86820-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86820-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="86820-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="86820-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86820-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86820-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86820-116">Not supported.</span></span>|
|<span data-ttu-id="86820-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86820-117">Application</span></span>|<span data-ttu-id="86820-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="86820-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86820-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86820-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="86820-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="86820-120">Request headers</span></span>
|<span data-ttu-id="86820-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86820-121">Header</span></span>|<span data-ttu-id="86820-122">Значение</span><span class="sxs-lookup"><span data-stu-id="86820-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86820-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86820-123">Authorization</span></span>|<span data-ttu-id="86820-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86820-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86820-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86820-125">Accept</span></span>|<span data-ttu-id="86820-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86820-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86820-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86820-127">Request body</span></span>
<span data-ttu-id="86820-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86820-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86820-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="86820-129">Response</span></span>
<span data-ttu-id="86820-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="86820-130">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86820-131">Пример</span><span class="sxs-lookup"><span data-stu-id="86820-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="86820-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="86820-132">Request</span></span>
<span data-ttu-id="86820-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86820-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="86820-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="86820-134">Response</span></span>
<span data-ttu-id="86820-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86820-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 532

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
      "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "platformType": "androidForWork",
      "unknownDeviceCount": 2,
      "notApplicableDeviceCount": 8,
      "compliantDeviceCount": 4,
      "remediatedDeviceCount": 5,
      "nonCompliantDeviceCount": 7,
      "errorDeviceCount": 0,
      "conflictDeviceCount": 3
    }
  ]
}
```





