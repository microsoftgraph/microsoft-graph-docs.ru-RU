---
title: Перечисление объектов deviceCompliancePolicySettingStateSummary
description: Список свойств и связей объектов deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7362e21bfd6be96e3864cf82e98e1e7dbaa16e37
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142534"
---
# <a name="list-devicecompliancepolicysettingstatesummaries"></a><span data-ttu-id="b666a-103">Перечисление объектов deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="b666a-103">List deviceCompliancePolicySettingStateSummaries</span></span>

> <span data-ttu-id="b666a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b666a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b666a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b666a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b666a-106">Список свойств и связей объектов [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="b666a-106">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b666a-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b666a-107">Prerequisites</span></span>
<span data-ttu-id="b666a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b666a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b666a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b666a-110">Permission type</span></span>|<span data-ttu-id="b666a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b666a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b666a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b666a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b666a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b666a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b666a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b666a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b666a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b666a-115">Not supported.</span></span>|
|<span data-ttu-id="b666a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b666a-116">Application</span></span>|<span data-ttu-id="b666a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b666a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b666a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b666a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="b666a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b666a-119">Request headers</span></span>
|<span data-ttu-id="b666a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b666a-120">Header</span></span>|<span data-ttu-id="b666a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b666a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b666a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b666a-122">Authorization</span></span>|<span data-ttu-id="b666a-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b666a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b666a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b666a-124">Accept</span></span>|<span data-ttu-id="b666a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b666a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b666a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b666a-126">Request body</span></span>
<span data-ttu-id="b666a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b666a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b666a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b666a-128">Response</span></span>
<span data-ttu-id="b666a-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b666a-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b666a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b666a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b666a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b666a-131">Request</span></span>
<span data-ttu-id="b666a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b666a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="b666a-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="b666a-133">Response</span></span>
<span data-ttu-id="b666a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b666a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




