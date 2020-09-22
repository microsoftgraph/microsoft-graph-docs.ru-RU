---
title: Список Девицеманажементинтентс
description: Список свойств и связей объектов Девицеманажементинтент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b3e3bca19bdb9ca7e853822bd105555a46163961
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000702"
---
# <a name="list-devicemanagementintents"></a><span data-ttu-id="d6cd3-103">Список Девицеманажементинтентс</span><span class="sxs-lookup"><span data-stu-id="d6cd3-103">List deviceManagementIntents</span></span>

<span data-ttu-id="d6cd3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6cd3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6cd3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6cd3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6cd3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6cd3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6cd3-107">Список свойств и связей объектов [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) .</span><span class="sxs-lookup"><span data-stu-id="d6cd3-107">List properties and relationships of the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6cd3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d6cd3-108">Prerequisites</span></span>
<span data-ttu-id="d6cd3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6cd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6cd3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6cd3-111">Permission type</span></span>|<span data-ttu-id="d6cd3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6cd3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6cd3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6cd3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6cd3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6cd3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d6cd3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6cd3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6cd3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6cd3-116">Not supported.</span></span>|
|<span data-ttu-id="d6cd3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6cd3-117">Application</span></span>|<span data-ttu-id="d6cd3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6cd3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6cd3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6cd3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents
```

## <a name="request-headers"></a><span data-ttu-id="d6cd3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d6cd3-120">Request headers</span></span>
|<span data-ttu-id="d6cd3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6cd3-121">Header</span></span>|<span data-ttu-id="d6cd3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d6cd3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6cd3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6cd3-123">Authorization</span></span>|<span data-ttu-id="d6cd3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6cd3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6cd3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d6cd3-125">Accept</span></span>|<span data-ttu-id="d6cd3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6cd3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6cd3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d6cd3-127">Request body</span></span>
<span data-ttu-id="d6cd3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6cd3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6cd3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6cd3-129">Response</span></span>
<span data-ttu-id="d6cd3-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6cd3-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6cd3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d6cd3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6cd3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6cd3-132">Request</span></span>
<span data-ttu-id="d6cd3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6cd3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents
```

### <a name="response"></a><span data-ttu-id="d6cd3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6cd3-134">Response</span></span>
<span data-ttu-id="d6cd3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6cd3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 452

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntent",
      "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
      "displayName": "Display Name value",
      "description": "Description value",
      "isAssigned": true,
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "templateId": "Template Id value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```






