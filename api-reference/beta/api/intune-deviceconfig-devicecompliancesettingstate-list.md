---
title: List deviceComplianceSettingStates
description: Перечисление свойств и связей объектов deviceComplianceSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5de2830828c9f2d94e91fdd8bf102bbc32f5840d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171227"
---
# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="c76ee-103">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="c76ee-103">List deviceComplianceSettingStates</span></span>

> <span data-ttu-id="c76ee-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c76ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c76ee-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c76ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c76ee-106">Перечисление свойств и связей объектов [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="c76ee-106">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c76ee-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c76ee-107">Prerequisites</span></span>
<span data-ttu-id="c76ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c76ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c76ee-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c76ee-110">Permission type</span></span>|<span data-ttu-id="c76ee-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c76ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c76ee-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c76ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c76ee-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c76ee-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c76ee-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c76ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c76ee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c76ee-115">Not supported.</span></span>|
|<span data-ttu-id="c76ee-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c76ee-116">Application</span></span>|<span data-ttu-id="c76ee-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c76ee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c76ee-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c76ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="c76ee-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c76ee-119">Request headers</span></span>
|<span data-ttu-id="c76ee-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c76ee-120">Header</span></span>|<span data-ttu-id="c76ee-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c76ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c76ee-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c76ee-122">Authorization</span></span>|<span data-ttu-id="c76ee-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c76ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c76ee-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c76ee-124">Accept</span></span>|<span data-ttu-id="c76ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c76ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c76ee-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c76ee-126">Request body</span></span>
<span data-ttu-id="c76ee-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c76ee-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c76ee-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c76ee-128">Response</span></span>
<span data-ttu-id="c76ee-129">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c76ee-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c76ee-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c76ee-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c76ee-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c76ee-131">Request</span></span>
<span data-ttu-id="c76ee-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c76ee-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="c76ee-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c76ee-133">Response</span></span>
<span data-ttu-id="c76ee-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c76ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 687

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
      "id": "9905f955-f955-9905-55f9-059955f90599",
      "platformType": "windowsRT",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "userId": "User Id value",
      "userEmail": "User Email value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "deviceModel": "Device Model value",
      "state": "notApplicable",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
    }
  ]
}
```




