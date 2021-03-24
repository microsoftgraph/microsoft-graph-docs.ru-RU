---
title: Перечисление объектов deviceCompliancePolicySettingStateSummary
description: Список свойств и связей объектов deviceCompliancePolicySettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b61db256b524753a723daa609378069d60bb2881
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130177"
---
# <a name="list-devicecompliancepolicysettingstatesummaries"></a><span data-ttu-id="ce94d-103">Перечисление объектов deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="ce94d-103">List deviceCompliancePolicySettingStateSummaries</span></span>

<span data-ttu-id="ce94d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce94d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce94d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce94d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce94d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce94d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce94d-107">Список свойств и связей объектов [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ce94d-107">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce94d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ce94d-108">Prerequisites</span></span>
<span data-ttu-id="ce94d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce94d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce94d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce94d-111">Permission type</span></span>|<span data-ttu-id="ce94d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce94d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce94d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce94d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce94d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce94d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ce94d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce94d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce94d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce94d-116">Not supported.</span></span>|
|<span data-ttu-id="ce94d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ce94d-117">Application</span></span>|<span data-ttu-id="ce94d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce94d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce94d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce94d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="ce94d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ce94d-120">Request headers</span></span>
|<span data-ttu-id="ce94d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce94d-121">Header</span></span>|<span data-ttu-id="ce94d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ce94d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce94d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce94d-123">Authorization</span></span>|<span data-ttu-id="ce94d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce94d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce94d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ce94d-125">Accept</span></span>|<span data-ttu-id="ce94d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce94d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce94d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce94d-127">Request body</span></span>
<span data-ttu-id="ce94d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce94d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce94d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce94d-129">Response</span></span>
<span data-ttu-id="ce94d-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ce94d-130">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce94d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ce94d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce94d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce94d-132">Request</span></span>
<span data-ttu-id="ce94d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce94d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="ce94d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce94d-134">Response</span></span>
<span data-ttu-id="ce94d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce94d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




