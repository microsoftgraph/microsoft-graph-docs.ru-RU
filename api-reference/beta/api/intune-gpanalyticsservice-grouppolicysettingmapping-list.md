---
title: List groupPolicySettingMappings
description: Список свойств и связей объектов groupPolicySettingMapping.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ab76bf8c3fb5796c0c0c95f0a1472c6ae1c8a8de
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135462"
---
# <a name="list-grouppolicysettingmappings"></a><span data-ttu-id="28879-103">List groupPolicySettingMappings</span><span class="sxs-lookup"><span data-stu-id="28879-103">List groupPolicySettingMappings</span></span>

<span data-ttu-id="28879-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28879-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28879-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28879-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28879-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28879-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28879-107">Список свойств и связей объектов [groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)</span><span class="sxs-lookup"><span data-stu-id="28879-107">List properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28879-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="28879-108">Prerequisites</span></span>
<span data-ttu-id="28879-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28879-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28879-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28879-111">Permission type</span></span>|<span data-ttu-id="28879-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28879-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28879-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28879-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28879-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28879-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28879-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28879-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28879-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28879-116">Not supported.</span></span>|
|<span data-ttu-id="28879-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="28879-117">Application</span></span>|<span data-ttu-id="28879-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28879-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28879-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28879-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

## <a name="request-headers"></a><span data-ttu-id="28879-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="28879-120">Request headers</span></span>
|<span data-ttu-id="28879-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28879-121">Header</span></span>|<span data-ttu-id="28879-122">Значение</span><span class="sxs-lookup"><span data-stu-id="28879-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28879-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="28879-123">Authorization</span></span>|<span data-ttu-id="28879-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28879-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28879-125">Accept</span><span class="sxs-lookup"><span data-stu-id="28879-125">Accept</span></span>|<span data-ttu-id="28879-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28879-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28879-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28879-127">Request body</span></span>
<span data-ttu-id="28879-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28879-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28879-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="28879-129">Response</span></span>
<span data-ttu-id="28879-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="28879-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28879-131">Пример</span><span class="sxs-lookup"><span data-stu-id="28879-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="28879-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="28879-132">Request</span></span>
<span data-ttu-id="28879-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28879-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

### <a name="response"></a><span data-ttu-id="28879-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="28879-134">Response</span></span>
<span data-ttu-id="28879-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28879-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1209

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
      "id": "8fa04560-4560-8fa0-6045-a08f6045a08f",
      "parentId": "Parent Id value",
      "childIdList": [
        "Child Id List value"
      ],
      "settingName": "Setting Name value",
      "settingValue": "Setting Value value",
      "settingValueType": "Setting Value Type value",
      "settingDisplayName": "Setting Display Name value",
      "settingDisplayValue": "Setting Display Value value",
      "settingDisplayValueType": "Setting Display Value Type value",
      "settingValueDisplayUnits": "Setting Value Display Units value",
      "settingCategory": "Setting Category value",
      "mdmCspName": "Mdm Csp Name value",
      "mdmSettingUri": "Mdm Setting Uri value",
      "mdmMinimumOSVersion": 3,
      "settingType": "policy",
      "isMdmSupported": true,
      "mdmSupportedState": "supported",
      "settingScope": "device",
      "intuneSettingUriList": [
        "Intune Setting Uri List value"
      ],
      "intuneSettingDefinitionId": "Intune Setting Definition Id value",
      "admxSettingDefinitionId": "Admx Setting Definition Id value"
    }
  ]
}
```




