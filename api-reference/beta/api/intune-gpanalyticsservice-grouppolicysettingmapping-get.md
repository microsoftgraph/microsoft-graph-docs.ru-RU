---
title: Get groupPolicySettingMapping
description: Чтение свойств и связей объекта groupPolicySettingMapping.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 898bfe9e7a688a753a51d3f5536962a2eb383d85
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135497"
---
# <a name="get-grouppolicysettingmapping"></a><span data-ttu-id="b4023-103">Get groupPolicySettingMapping</span><span class="sxs-lookup"><span data-stu-id="b4023-103">Get groupPolicySettingMapping</span></span>

<span data-ttu-id="b4023-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4023-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4023-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4023-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4023-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4023-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4023-107">Чтение свойств и связей объекта [groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)</span><span class="sxs-lookup"><span data-stu-id="b4023-107">Read properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4023-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b4023-108">Prerequisites</span></span>
<span data-ttu-id="b4023-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4023-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4023-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4023-111">Permission type</span></span>|<span data-ttu-id="b4023-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4023-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4023-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4023-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4023-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4023-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4023-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4023-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4023-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4023-116">Not supported.</span></span>|
|<span data-ttu-id="b4023-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b4023-117">Application</span></span>|<span data-ttu-id="b4023-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4023-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4023-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4023-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b4023-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b4023-120">Optional query parameters</span></span>
<span data-ttu-id="b4023-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b4023-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4023-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4023-122">Request headers</span></span>
|<span data-ttu-id="b4023-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4023-123">Header</span></span>|<span data-ttu-id="b4023-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b4023-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4023-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4023-125">Authorization</span></span>|<span data-ttu-id="b4023-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4023-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4023-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b4023-127">Accept</span></span>|<span data-ttu-id="b4023-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b4023-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4023-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4023-129">Request body</span></span>
<span data-ttu-id="b4023-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4023-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4023-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4023-131">Response</span></span>
<span data-ttu-id="b4023-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b4023-132">If successful, this method returns a `200 OK` response code and [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4023-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b4023-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4023-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4023-134">Request</span></span>
<span data-ttu-id="b4023-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4023-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

### <a name="response"></a><span data-ttu-id="b4023-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4023-136">Response</span></span>
<span data-ttu-id="b4023-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4023-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1143

{
  "value": {
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
}
```




