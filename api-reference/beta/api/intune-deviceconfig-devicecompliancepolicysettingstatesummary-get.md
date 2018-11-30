---
title: Get deviceCompliancePolicySettingStateSummary
description: Чтение свойств и связей объекта deviceCompliancePolicySettingStateSummary.
ms.openlocfilehash: e184d0e2890fb7fb7f7642ef56d7a6d1946b5a31
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076891"
---
# <a name="get-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="94e40-103">Get deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="94e40-103">Get deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="94e40-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="94e40-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94e40-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94e40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94e40-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="94e40-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94e40-107">Чтение свойств и связей объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="94e40-107">Read properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="94e40-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="94e40-108">Prerequisites</span></span>
<span data-ttu-id="94e40-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94e40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94e40-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94e40-111">Permission type</span></span>|<span data-ttu-id="94e40-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="94e40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94e40-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94e40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="94e40-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="94e40-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="94e40-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94e40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94e40-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94e40-116">Not supported.</span></span>|
|<span data-ttu-id="94e40-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94e40-117">Application</span></span>|<span data-ttu-id="94e40-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94e40-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94e40-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94e40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94e40-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="94e40-120">Optional query parameters</span></span>
<span data-ttu-id="94e40-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="94e40-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="94e40-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94e40-122">Request headers</span></span>
|<span data-ttu-id="94e40-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="94e40-123">Header</span></span>|<span data-ttu-id="94e40-124">Значение</span><span class="sxs-lookup"><span data-stu-id="94e40-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94e40-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="94e40-125">Authorization</span></span>|<span data-ttu-id="94e40-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="94e40-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94e40-127">Accept</span><span class="sxs-lookup"><span data-stu-id="94e40-127">Accept</span></span>|<span data-ttu-id="94e40-128">application/json</span><span class="sxs-lookup"><span data-stu-id="94e40-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94e40-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94e40-129">Request body</span></span>
<span data-ttu-id="94e40-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94e40-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94e40-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="94e40-131">Response</span></span>
<span data-ttu-id="94e40-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="94e40-132">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94e40-133">Пример</span><span class="sxs-lookup"><span data-stu-id="94e40-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="94e40-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="94e40-134">Request</span></span>
<span data-ttu-id="94e40-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94e40-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="94e40-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="94e40-136">Response</span></span>
<span data-ttu-id="94e40-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="94e40-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 494

{
  "value": {
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
}
```





