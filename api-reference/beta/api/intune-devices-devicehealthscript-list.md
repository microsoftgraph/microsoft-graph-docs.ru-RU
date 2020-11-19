---
title: Список Девицехеалсскриптс
description: Список свойств и связей объектов Девицехеалсскрипт.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e80ad3290796b0f4fe5627255fc96f3cf199e918
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49225840"
---
# <a name="list-devicehealthscripts"></a><span data-ttu-id="43227-103">Список Девицехеалсскриптс</span><span class="sxs-lookup"><span data-stu-id="43227-103">List deviceHealthScripts</span></span>

<span data-ttu-id="43227-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43227-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43227-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43227-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43227-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43227-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43227-107">Список свойств и связей объектов [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="43227-107">List properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43227-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="43227-108">Prerequisites</span></span>
<span data-ttu-id="43227-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43227-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43227-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43227-111">Permission type</span></span>|<span data-ttu-id="43227-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43227-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43227-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43227-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43227-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="43227-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="43227-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43227-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43227-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43227-116">Not supported.</span></span>|
|<span data-ttu-id="43227-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="43227-117">Application</span></span>|<span data-ttu-id="43227-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="43227-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43227-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43227-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts
```

## <a name="request-headers"></a><span data-ttu-id="43227-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="43227-120">Request headers</span></span>
|<span data-ttu-id="43227-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43227-121">Header</span></span>|<span data-ttu-id="43227-122">Значение</span><span class="sxs-lookup"><span data-stu-id="43227-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43227-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43227-123">Authorization</span></span>|<span data-ttu-id="43227-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43227-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43227-125">Accept</span><span class="sxs-lookup"><span data-stu-id="43227-125">Accept</span></span>|<span data-ttu-id="43227-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43227-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43227-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43227-127">Request body</span></span>
<span data-ttu-id="43227-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43227-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43227-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="43227-129">Response</span></span>
<span data-ttu-id="43227-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="43227-130">If successful, this method returns a `200 OK` response code and a collection of [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43227-131">Пример</span><span class="sxs-lookup"><span data-stu-id="43227-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="43227-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="43227-132">Request</span></span>
<span data-ttu-id="43227-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43227-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts
```

### <a name="response"></a><span data-ttu-id="43227-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="43227-134">Response</span></span>
<span data-ttu-id="43227-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43227-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1578

{
  "value": [
    {
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
  ]
}
```




