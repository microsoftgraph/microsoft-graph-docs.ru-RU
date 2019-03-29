---
title: Получение объекта managedDeviceMobileAppConfiguration
description: Чтение свойств и связей объекта managedDeviceMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: efc1c1bfe263adcf9d559fc3985bfd766525ca9d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957803"
---
# <a name="get-manageddevicemobileappconfiguration"></a><span data-ttu-id="d5fa2-103">Получение объекта managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5fa2-103">Get managedDeviceMobileAppConfiguration</span></span>

> <span data-ttu-id="d5fa2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5fa2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5fa2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5fa2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5fa2-106">Чтение свойств и связей объекта [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5fa2-106">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5fa2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d5fa2-107">Prerequisites</span></span>
<span data-ttu-id="d5fa2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5fa2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5fa2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5fa2-110">Permission type</span></span>|<span data-ttu-id="d5fa2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5fa2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5fa2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5fa2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d5fa2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5fa2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d5fa2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5fa2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5fa2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5fa2-115">Not supported.</span></span>|
|<span data-ttu-id="d5fa2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5fa2-116">Application</span></span>|<span data-ttu-id="d5fa2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5fa2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5fa2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5fa2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d5fa2-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d5fa2-119">Optional query parameters</span></span>
<span data-ttu-id="d5fa2-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d5fa2-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5fa2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5fa2-121">Request headers</span></span>
|<span data-ttu-id="d5fa2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5fa2-122">Header</span></span>|<span data-ttu-id="d5fa2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d5fa2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5fa2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5fa2-124">Authorization</span></span>|<span data-ttu-id="d5fa2-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5fa2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5fa2-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d5fa2-126">Accept</span></span>|<span data-ttu-id="d5fa2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d5fa2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5fa2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5fa2-128">Request body</span></span>
<span data-ttu-id="d5fa2-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d5fa2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5fa2-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5fa2-130">Response</span></span>
<span data-ttu-id="d5fa2-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d5fa2-131">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5fa2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d5fa2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5fa2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5fa2-133">Request</span></span>
<span data-ttu-id="d5fa2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5fa2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d5fa2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5fa2-135">Response</span></span>
<span data-ttu-id="d5fa2-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5fa2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 519

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
    "id": "c60e7591-7591-c60e-9175-0ec691750ec6",
    "targetedMobileApps": [
      "Targeted Mobile Apps value"
    ],
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7
  }
}
```




