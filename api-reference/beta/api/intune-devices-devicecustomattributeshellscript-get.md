---
title: Get deviceCustomAttributeShellScript
description: Чтение свойств и связей объекта deviceCustomAttributeShellScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 313560a9b2ef9066e025f6e68142a602f0d9cb77
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154422"
---
# <a name="get-devicecustomattributeshellscript"></a><span data-ttu-id="4efd5-103">Get deviceCustomAttributeShellScript</span><span class="sxs-lookup"><span data-stu-id="4efd5-103">Get deviceCustomAttributeShellScript</span></span>

<span data-ttu-id="4efd5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4efd5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4efd5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4efd5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4efd5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4efd5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4efd5-107">Чтение свойств и связей [объекта deviceCustomAttributeShellScript.](../resources/intune-devices-devicecustomattributeshellscript.md)</span><span class="sxs-lookup"><span data-stu-id="4efd5-107">Read properties and relationships of the [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4efd5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4efd5-108">Prerequisites</span></span>
<span data-ttu-id="4efd5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4efd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4efd5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4efd5-111">Permission type</span></span>|<span data-ttu-id="4efd5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4efd5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4efd5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4efd5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4efd5-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4efd5-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4efd5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4efd5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4efd5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4efd5-116">Not supported.</span></span>|
|<span data-ttu-id="4efd5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4efd5-117">Application</span></span>|<span data-ttu-id="4efd5-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4efd5-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4efd5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4efd5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4efd5-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4efd5-120">Optional query parameters</span></span>
<span data-ttu-id="4efd5-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4efd5-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4efd5-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4efd5-122">Request headers</span></span>
|<span data-ttu-id="4efd5-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4efd5-123">Header</span></span>|<span data-ttu-id="4efd5-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4efd5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4efd5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4efd5-125">Authorization</span></span>|<span data-ttu-id="4efd5-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4efd5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4efd5-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4efd5-127">Accept</span></span>|<span data-ttu-id="4efd5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4efd5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4efd5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4efd5-129">Request body</span></span>
<span data-ttu-id="4efd5-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4efd5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4efd5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4efd5-131">Response</span></span>
<span data-ttu-id="4efd5-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4efd5-132">If successful, this method returns a `200 OK` response code and [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4efd5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4efd5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4efd5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4efd5-134">Request</span></span>
<span data-ttu-id="4efd5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4efd5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}
```

### <a name="response"></a><span data-ttu-id="4efd5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4efd5-136">Response</span></span>
<span data-ttu-id="4efd5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4efd5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 632

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCustomAttributeShellScript",
    "id": "929d921b-921b-929d-1b92-9d921b929d92",
    "customAttributeName": "Custom Attribute Name value",
    "customAttributeType": "string",
    "displayName": "Display Name value",
    "description": "Description value",
    "scriptContent": "c2NyaXB0Q29udGVudA==",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "runAsAccount": "user",
    "fileName": "File Name value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




