---
title: Получение объекта managedDeviceMobileAppConfiguration
description: Чтение свойств и связей объекта managedDeviceMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 52ca4d0ba3406545380afe0b03b0750cd7121d64
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699522"
---
# <a name="get-manageddevicemobileappconfiguration"></a><span data-ttu-id="f7ff0-103">Получение объекта managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7ff0-103">Get managedDeviceMobileAppConfiguration</span></span>

<span data-ttu-id="f7ff0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7ff0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7ff0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7ff0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7ff0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7ff0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7ff0-107">Чтение свойств и связей объекта [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7ff0-107">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7ff0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f7ff0-108">Prerequisites</span></span>
<span data-ttu-id="f7ff0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7ff0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7ff0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7ff0-111">Permission type</span></span>|<span data-ttu-id="f7ff0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7ff0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7ff0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7ff0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7ff0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7ff0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f7ff0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7ff0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7ff0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7ff0-116">Not supported.</span></span>|
|<span data-ttu-id="f7ff0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7ff0-117">Application</span></span>|<span data-ttu-id="f7ff0-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7ff0-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7ff0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7ff0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7ff0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f7ff0-120">Optional query parameters</span></span>
<span data-ttu-id="f7ff0-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f7ff0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7ff0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7ff0-122">Request headers</span></span>
|<span data-ttu-id="f7ff0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7ff0-123">Header</span></span>|<span data-ttu-id="f7ff0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f7ff0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7ff0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7ff0-125">Authorization</span></span>|<span data-ttu-id="f7ff0-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7ff0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7ff0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f7ff0-127">Accept</span></span>|<span data-ttu-id="f7ff0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f7ff0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7ff0-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f7ff0-129">Request body</span></span>
<span data-ttu-id="f7ff0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7ff0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7ff0-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7ff0-131">Response</span></span>
<span data-ttu-id="f7ff0-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7ff0-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7ff0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f7ff0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7ff0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7ff0-134">Request</span></span>
<span data-ttu-id="f7ff0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7ff0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f7ff0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7ff0-136">Response</span></span>
<span data-ttu-id="f7ff0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7ff0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





