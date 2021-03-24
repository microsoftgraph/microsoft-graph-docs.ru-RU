---
title: Get deviceHealthScript
description: Чтение свойств и связей объекта deviceHealthScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f6eecdd41b2d96750f5739e0620d635bcf805fd4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146344"
---
# <a name="get-devicehealthscript"></a><span data-ttu-id="7b665-103">Get deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="7b665-103">Get deviceHealthScript</span></span>

<span data-ttu-id="7b665-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b665-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b665-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b665-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b665-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b665-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b665-107">Чтение свойств и связей [объекта deviceHealthScript.](../resources/intune-devices-devicehealthscript.md)</span><span class="sxs-lookup"><span data-stu-id="7b665-107">Read properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b665-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7b665-108">Prerequisites</span></span>
<span data-ttu-id="7b665-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b665-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b665-111">Permission type</span></span>|<span data-ttu-id="7b665-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b665-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b665-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b665-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b665-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b665-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b665-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b665-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b665-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b665-116">Not supported.</span></span>|
|<span data-ttu-id="7b665-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7b665-117">Application</span></span>|<span data-ttu-id="7b665-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b665-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b665-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b665-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b665-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7b665-120">Optional query parameters</span></span>
<span data-ttu-id="7b665-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7b665-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b665-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b665-122">Request headers</span></span>
|<span data-ttu-id="7b665-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b665-123">Header</span></span>|<span data-ttu-id="7b665-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7b665-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b665-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b665-125">Authorization</span></span>|<span data-ttu-id="7b665-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b665-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b665-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7b665-127">Accept</span></span>|<span data-ttu-id="7b665-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7b665-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b665-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b665-129">Request body</span></span>
<span data-ttu-id="7b665-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b665-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b665-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b665-131">Response</span></span>
<span data-ttu-id="7b665-132">В случае успеха этот метод возвращает код отклика и `200 OK` [объект deviceHealthScript](../resources/intune-devices-devicehealthscript.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7b665-132">If successful, this method returns a `200 OK` response code and [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b665-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7b665-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b665-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b665-134">Request</span></span>
<span data-ttu-id="7b665-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b665-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

### <a name="response"></a><span data-ttu-id="7b665-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b665-136">Response</span></span>
<span data-ttu-id="7b665-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b665-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1488

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceHealthScript",
    "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
    "publisher": "Publisher value",
    "version": "Version value",
    "displayName": "Display Name value",
    "description": "Description value",
    "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
    "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "runAsAccount": "user",
    "enforceSignatureCheck": true,
    "runAs32Bit": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "isGlobalScript": true,
    "highestAvailableVersion": "Highest Available Version value",
    "detectionScriptParameters": [
      {
        "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
        "name": "Name value",
        "description": "Description value",
        "isRequired": true,
        "applyDefaultValueWhenNotAssigned": true,
        "defaultValue": "Default Value value"
      }
    ],
    "remediationScriptParameters": [
      {
        "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
        "name": "Name value",
        "description": "Description value",
        "isRequired": true,
        "applyDefaultValueWhenNotAssigned": true,
        "defaultValue": "Default Value value"
      }
    ]
  }
}
```




