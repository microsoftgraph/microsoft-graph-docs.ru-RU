---
title: Получение объекта windowsDefenderAdvancedThreatProtectionConfiguration
description: Чтение свойств и связей объекта windowsDefenderAdvancedThreatProtectionConfiguration.
ms.openlocfilehash: e524ec023df72080277dee69d7bcf3de51059f0e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027297"
---
# <a name="get-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="8beab-103">Получение объекта windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="8beab-103">Get windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="8beab-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8beab-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8beab-105">Чтение свойств и связей объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8beab-105">Read properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8beab-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8beab-106">Prerequisites</span></span>
<span data-ttu-id="8beab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8beab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8beab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8beab-109">Permission type</span></span>|<span data-ttu-id="8beab-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8beab-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8beab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8beab-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8beab-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8beab-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8beab-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8beab-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8beab-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8beab-114">Not supported.</span></span>|
|<span data-ttu-id="8beab-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8beab-115">Application</span></span>|<span data-ttu-id="8beab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8beab-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8beab-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8beab-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8beab-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8beab-118">Optional query parameters</span></span>
<span data-ttu-id="8beab-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8beab-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8beab-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8beab-120">Request headers</span></span>
|<span data-ttu-id="8beab-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8beab-121">Header</span></span>|<span data-ttu-id="8beab-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8beab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8beab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8beab-123">Authorization</span></span>|<span data-ttu-id="8beab-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8beab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8beab-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8beab-125">Accept</span></span>|<span data-ttu-id="8beab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8beab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8beab-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8beab-127">Request body</span></span>
<span data-ttu-id="8beab-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8beab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8beab-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8beab-129">Response</span></span>
<span data-ttu-id="8beab-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8beab-130">If successful, this method returns a `200 OK` response code and [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8beab-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8beab-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8beab-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8beab-132">Request</span></span>
<span data-ttu-id="8beab-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8beab-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="8beab-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="8beab-134">Response</span></span>
<span data-ttu-id="8beab-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8beab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 476

{
  "value": {
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
}
```



