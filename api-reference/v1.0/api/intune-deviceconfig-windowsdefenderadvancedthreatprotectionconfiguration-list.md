---
title: Перечисление объектов windowsDefenderAdvancedThreatProtectionConfiguration
description: Список свойств и связей объектов windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc02f74b2153ae3648e934982fc9ee16cf47b5bf
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259670"
---
# <a name="list-windowsdefenderadvancedthreatprotectionconfigurations"></a><span data-ttu-id="fd554-103">Перечисление объектов windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd554-103">List windowsDefenderAdvancedThreatProtectionConfigurations</span></span>

> <span data-ttu-id="fd554-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd554-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd554-105">Список свойств и связей объектов [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd554-105">List properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd554-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fd554-106">Prerequisites</span></span>
<span data-ttu-id="fd554-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fd554-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fd554-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd554-109">Permission type</span></span>|<span data-ttu-id="fd554-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd554-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd554-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd554-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fd554-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd554-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fd554-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd554-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd554-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd554-114">Not supported.</span></span>|
|<span data-ttu-id="fd554-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd554-115">Application</span></span>|<span data-ttu-id="fd554-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd554-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd554-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd554-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fd554-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd554-118">Request headers</span></span>
|<span data-ttu-id="fd554-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd554-119">Header</span></span>|<span data-ttu-id="fd554-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fd554-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd554-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd554-121">Authorization</span></span>|<span data-ttu-id="fd554-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fd554-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd554-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fd554-123">Accept</span></span>|<span data-ttu-id="fd554-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fd554-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd554-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd554-125">Request body</span></span>
<span data-ttu-id="fd554-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fd554-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd554-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd554-127">Response</span></span>
<span data-ttu-id="fd554-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fd554-128">If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd554-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fd554-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd554-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd554-130">Request</span></span>
<span data-ttu-id="fd554-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd554-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="fd554-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd554-132">Response</span></span>
<span data-ttu-id="fd554-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fd554-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



