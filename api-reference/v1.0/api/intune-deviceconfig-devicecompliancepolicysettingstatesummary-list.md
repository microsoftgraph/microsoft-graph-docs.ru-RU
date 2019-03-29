---
title: Перечисление объектов deviceCompliancePolicySettingStateSummary
description: Список свойств и связей объектов deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29f64028604c3f3402c12d4b08170f5925d1cd8e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973805"
---
# <a name="list-devicecompliancepolicysettingstatesummaries"></a><span data-ttu-id="efb61-103">Перечисление объектов deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="efb61-103">List deviceCompliancePolicySettingStateSummaries</span></span>

> <span data-ttu-id="efb61-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="efb61-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efb61-105">Список свойств и связей объектов [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="efb61-105">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efb61-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="efb61-106">Prerequisites</span></span>
<span data-ttu-id="efb61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efb61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efb61-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efb61-109">Permission type</span></span>|<span data-ttu-id="efb61-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="efb61-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efb61-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efb61-111">Delegated (work or school account)</span></span>|<span data-ttu-id="efb61-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="efb61-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="efb61-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efb61-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efb61-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efb61-114">Not supported.</span></span>|
|<span data-ttu-id="efb61-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efb61-115">Application</span></span>|<span data-ttu-id="efb61-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efb61-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efb61-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efb61-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="efb61-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="efb61-118">Request headers</span></span>
|<span data-ttu-id="efb61-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="efb61-119">Header</span></span>|<span data-ttu-id="efb61-120">Значение</span><span class="sxs-lookup"><span data-stu-id="efb61-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efb61-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efb61-121">Authorization</span></span>|<span data-ttu-id="efb61-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efb61-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efb61-123">Accept</span><span class="sxs-lookup"><span data-stu-id="efb61-123">Accept</span></span>|<span data-ttu-id="efb61-124">application/json</span><span class="sxs-lookup"><span data-stu-id="efb61-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efb61-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efb61-125">Request body</span></span>
<span data-ttu-id="efb61-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="efb61-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efb61-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="efb61-127">Response</span></span>
<span data-ttu-id="efb61-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="efb61-128">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efb61-129">Пример</span><span class="sxs-lookup"><span data-stu-id="efb61-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="efb61-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="efb61-130">Request</span></span>
<span data-ttu-id="efb61-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efb61-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="efb61-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="efb61-132">Response</span></span>
<span data-ttu-id="efb61-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efb61-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 521

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
      "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "platformType": "iOS",
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



