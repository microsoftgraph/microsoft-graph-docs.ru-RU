---
title: Перечисление объектов windowsDefenderAdvancedThreatProtectionConfiguration
description: Список свойств и связей объектов windowsDefenderAdvancedThreatProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 822dbf8431b9b5932bbfa75113de300f4367960c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462042"
---
# <a name="list-windowsdefenderadvancedthreatprotectionconfigurations"></a><span data-ttu-id="c288b-103">Перечисление объектов windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="c288b-103">List windowsDefenderAdvancedThreatProtectionConfigurations</span></span>

<span data-ttu-id="c288b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c288b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c288b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c288b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c288b-106">Список свойств и связей объектов [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c288b-106">List properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c288b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c288b-107">Prerequisites</span></span>
<span data-ttu-id="c288b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c288b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c288b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c288b-110">Permission type</span></span>|<span data-ttu-id="c288b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c288b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c288b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c288b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c288b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c288b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c288b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c288b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c288b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c288b-115">Not supported.</span></span>|
|<span data-ttu-id="c288b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c288b-116">Application</span></span>|<span data-ttu-id="c288b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c288b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c288b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c288b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c288b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c288b-119">Request headers</span></span>
|<span data-ttu-id="c288b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c288b-120">Header</span></span>|<span data-ttu-id="c288b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c288b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c288b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c288b-122">Authorization</span></span>|<span data-ttu-id="c288b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c288b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c288b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c288b-124">Accept</span></span>|<span data-ttu-id="c288b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c288b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c288b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c288b-126">Request body</span></span>
<span data-ttu-id="c288b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c288b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c288b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c288b-128">Response</span></span>
<span data-ttu-id="c288b-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c288b-129">If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c288b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c288b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c288b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c288b-131">Request</span></span>
<span data-ttu-id="c288b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c288b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="c288b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c288b-133">Response</span></span>
<span data-ttu-id="c288b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c288b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 508

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
      "id": "294373aa-73aa-2943-aa73-4329aa734329",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "allowSampleSharing": true,
      "enableExpeditedTelemetryReporting": true
    }
  ]
}
```






