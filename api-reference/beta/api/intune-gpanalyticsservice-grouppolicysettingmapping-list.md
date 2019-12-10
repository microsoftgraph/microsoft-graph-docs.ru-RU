---
title: Список Граупполицисеттингмаппингс
description: Список свойств и связей объектов Граупполицисеттингмаппинг.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: df72773a47b696f209eedf96f02311636fdeb9c1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943251"
---
# <a name="list-grouppolicysettingmappings"></a><span data-ttu-id="bd8c7-103">Список Граупполицисеттингмаппингс</span><span class="sxs-lookup"><span data-stu-id="bd8c7-103">List groupPolicySettingMappings</span></span>

> <span data-ttu-id="bd8c7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd8c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd8c7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd8c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd8c7-106">Список свойств и связей объектов [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) .</span><span class="sxs-lookup"><span data-stu-id="bd8c7-106">List properties and relationships of the [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd8c7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bd8c7-107">Prerequisites</span></span>
<span data-ttu-id="bd8c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd8c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd8c7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd8c7-110">Permission type</span></span>|<span data-ttu-id="bd8c7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd8c7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd8c7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd8c7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bd8c7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd8c7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bd8c7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd8c7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd8c7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd8c7-115">Not supported.</span></span>|
|<span data-ttu-id="bd8c7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd8c7-116">Application</span></span>|<span data-ttu-id="bd8c7-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd8c7-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd8c7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd8c7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

## <a name="request-headers"></a><span data-ttu-id="bd8c7-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bd8c7-119">Request headers</span></span>
|<span data-ttu-id="bd8c7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd8c7-120">Header</span></span>|<span data-ttu-id="bd8c7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bd8c7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd8c7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd8c7-122">Authorization</span></span>|<span data-ttu-id="bd8c7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd8c7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd8c7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bd8c7-124">Accept</span></span>|<span data-ttu-id="bd8c7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bd8c7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd8c7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bd8c7-126">Request body</span></span>
<span data-ttu-id="bd8c7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd8c7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd8c7-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="bd8c7-128">Response</span></span>
<span data-ttu-id="bd8c7-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполицисеттингмаппинг](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bd8c7-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd8c7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bd8c7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd8c7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd8c7-131">Request</span></span>
<span data-ttu-id="bd8c7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd8c7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

### <a name="response"></a><span data-ttu-id="bd8c7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd8c7-133">Response</span></span>
<span data-ttu-id="bd8c7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd8c7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1065

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
      ]
    }
  ]
}
```





