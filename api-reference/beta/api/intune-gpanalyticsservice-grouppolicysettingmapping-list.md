---
title: Список Граупполицисеттингмаппингс
description: Список свойств и связей объектов Граупполицисеттингмаппинг.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3f3c4e48f5eb122f1cbd8d4d7762ac28307cf907
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454845"
---
# <a name="list-grouppolicysettingmappings"></a><span data-ttu-id="d58b1-103">Список Граупполицисеттингмаппингс</span><span class="sxs-lookup"><span data-stu-id="d58b1-103">List groupPolicySettingMappings</span></span>

<span data-ttu-id="d58b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d58b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d58b1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d58b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d58b1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d58b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d58b1-107">Список свойств и связей объектов [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="d58b1-107">List properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d58b1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d58b1-108">Prerequisites</span></span>
<span data-ttu-id="d58b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d58b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d58b1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d58b1-111">Permission type</span></span>|<span data-ttu-id="d58b1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d58b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d58b1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d58b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d58b1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d58b1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d58b1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d58b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d58b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d58b1-116">Not supported.</span></span>|
|<span data-ttu-id="d58b1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d58b1-117">Application</span></span>|<span data-ttu-id="d58b1-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d58b1-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d58b1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d58b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

## <a name="request-headers"></a><span data-ttu-id="d58b1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d58b1-120">Request headers</span></span>
|<span data-ttu-id="d58b1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d58b1-121">Header</span></span>|<span data-ttu-id="d58b1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d58b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d58b1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d58b1-123">Authorization</span></span>|<span data-ttu-id="d58b1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d58b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d58b1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d58b1-125">Accept</span></span>|<span data-ttu-id="d58b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d58b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d58b1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d58b1-127">Request body</span></span>
<span data-ttu-id="d58b1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d58b1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d58b1-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d58b1-129">Response</span></span>
<span data-ttu-id="d58b1-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d58b1-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d58b1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d58b1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d58b1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d58b1-132">Request</span></span>
<span data-ttu-id="d58b1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d58b1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

### <a name="response"></a><span data-ttu-id="d58b1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d58b1-134">Response</span></span>
<span data-ttu-id="d58b1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d58b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1139

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
      "intuneSettingDefinitionId": "Intune Setting Definition Id value"
    }
  ]
}
```



