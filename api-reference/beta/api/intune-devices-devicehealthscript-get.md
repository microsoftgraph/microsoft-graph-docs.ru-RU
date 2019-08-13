---
title: Получение Девицехеалсскрипт
description: Чтение свойств и связей объекта Девицехеалсскрипт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: efa373bea2430dc85533904487d0525c069d053a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36311739"
---
# <a name="get-devicehealthscript"></a><span data-ttu-id="9e6f1-103">Получение Девицехеалсскрипт</span><span class="sxs-lookup"><span data-stu-id="9e6f1-103">Get deviceHealthScript</span></span>

> <span data-ttu-id="9e6f1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e6f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e6f1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9e6f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e6f1-106">Чтение свойств и связей объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="9e6f1-106">Read properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e6f1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9e6f1-107">Prerequisites</span></span>
<span data-ttu-id="9e6f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e6f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e6f1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e6f1-110">Permission type</span></span>|<span data-ttu-id="9e6f1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e6f1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e6f1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e6f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e6f1-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e6f1-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9e6f1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e6f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e6f1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e6f1-115">Not supported.</span></span>|
|<span data-ttu-id="9e6f1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e6f1-116">Application</span></span>|<span data-ttu-id="9e6f1-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e6f1-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e6f1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e6f1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e6f1-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9e6f1-119">Optional query parameters</span></span>
<span data-ttu-id="9e6f1-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9e6f1-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e6f1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e6f1-121">Request headers</span></span>
|<span data-ttu-id="9e6f1-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9e6f1-122">Header</span></span>|<span data-ttu-id="9e6f1-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9e6f1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e6f1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e6f1-124">Authorization</span></span>|<span data-ttu-id="9e6f1-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e6f1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e6f1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9e6f1-126">Accept</span></span>|<span data-ttu-id="9e6f1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9e6f1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e6f1-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9e6f1-128">Request body</span></span>
<span data-ttu-id="9e6f1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e6f1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e6f1-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e6f1-130">Response</span></span>
<span data-ttu-id="9e6f1-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e6f1-131">If successful, this method returns a `200 OK` response code and [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e6f1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9e6f1-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e6f1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e6f1-133">Request</span></span>
<span data-ttu-id="9e6f1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e6f1-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

### <a name="response"></a><span data-ttu-id="9e6f1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e6f1-135">Response</span></span>
<span data-ttu-id="9e6f1-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e6f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 986

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceHealthScript",
    "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
    "displayName": "Display Name value",
    "description": "Description value",
    "runSchedule": {
      "@odata.type": "microsoft.graph.runSchedule"
    },
    "scriptContent": "c2NyaXB0Q29udGVudA==",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "runAsAccount": "user",
    "enforceSignatureCheck": true,
    "fileName": "File Name value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "runAs32Bit": true,
    "complianceRule": {
      "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
      "detectionType": "string",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    },
    "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
    "runRemediationScript": true
  }
}
```






