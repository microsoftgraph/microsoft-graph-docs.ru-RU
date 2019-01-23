---
title: Перечисление объектов deviceCompliancePolicySettingStateSummary
description: Список свойств и связей объектов deviceCompliancePolicySettingStateSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7f079f75b8583cc5c057bad26ccf79ce734beed7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406845"
---
# <a name="list-devicecompliancepolicysettingstatesummaries"></a><span data-ttu-id="5e4ad-103">Перечисление объектов deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="5e4ad-103">List deviceCompliancePolicySettingStateSummaries</span></span>

> <span data-ttu-id="5e4ad-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5e4ad-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5e4ad-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e4ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e4ad-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e4ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e4ad-107">Список свойств и связей объектов [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="5e4ad-107">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e4ad-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5e4ad-108">Prerequisites</span></span>
<span data-ttu-id="5e4ad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5e4ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5e4ad-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e4ad-111">Permission type</span></span>|<span data-ttu-id="5e4ad-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e4ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e4ad-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e4ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e4ad-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e4ad-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5e4ad-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e4ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e4ad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e4ad-116">Not supported.</span></span>|
|<span data-ttu-id="5e4ad-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e4ad-117">Application</span></span>|<span data-ttu-id="5e4ad-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e4ad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e4ad-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e4ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="5e4ad-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e4ad-120">Request headers</span></span>
|<span data-ttu-id="5e4ad-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e4ad-121">Header</span></span>|<span data-ttu-id="5e4ad-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5e4ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e4ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e4ad-123">Authorization</span></span>|<span data-ttu-id="5e4ad-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5e4ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e4ad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5e4ad-125">Accept</span></span>|<span data-ttu-id="5e4ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e4ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e4ad-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e4ad-127">Request body</span></span>
<span data-ttu-id="5e4ad-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5e4ad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e4ad-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e4ad-129">Response</span></span>
<span data-ttu-id="5e4ad-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e4ad-130">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e4ad-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5e4ad-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e4ad-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e4ad-132">Request</span></span>
<span data-ttu-id="5e4ad-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e4ad-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="5e4ad-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e4ad-134">Response</span></span>
<span data-ttu-id="5e4ad-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5e4ad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




