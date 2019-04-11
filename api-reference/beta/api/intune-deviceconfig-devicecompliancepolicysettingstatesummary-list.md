---
title: Перечисление объектов deviceCompliancePolicySettingStateSummary
description: Список свойств и связей объектов deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 62108348a08f39fdcda741960edabaf38e539f70
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776950"
---
# <a name="list-devicecompliancepolicysettingstatesummaries"></a><span data-ttu-id="e5344-103">Перечисление объектов deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="e5344-103">List deviceCompliancePolicySettingStateSummaries</span></span>

> <span data-ttu-id="e5344-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5344-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5344-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5344-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5344-106">Список свойств и связей объектов [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e5344-106">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5344-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e5344-107">Prerequisites</span></span>
<span data-ttu-id="e5344-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5344-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5344-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5344-110">Permission type</span></span>|<span data-ttu-id="e5344-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5344-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5344-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5344-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5344-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5344-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e5344-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5344-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5344-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5344-115">Not supported.</span></span>|
|<span data-ttu-id="e5344-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5344-116">Application</span></span>|<span data-ttu-id="e5344-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5344-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5344-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5344-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="e5344-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5344-119">Request headers</span></span>
|<span data-ttu-id="e5344-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5344-120">Header</span></span>|<span data-ttu-id="e5344-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e5344-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5344-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5344-122">Authorization</span></span>|<span data-ttu-id="e5344-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5344-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5344-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e5344-124">Accept</span></span>|<span data-ttu-id="e5344-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5344-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5344-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5344-126">Request body</span></span>
<span data-ttu-id="e5344-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5344-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5344-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5344-128">Response</span></span>
<span data-ttu-id="e5344-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5344-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5344-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e5344-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5344-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5344-131">Request</span></span>
<span data-ttu-id="e5344-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5344-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="e5344-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5344-133">Response</span></span>
<span data-ttu-id="e5344-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5344-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





