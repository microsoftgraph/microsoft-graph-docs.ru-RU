---
title: Получение targetedManagedAppConfiguration
description: Чтение свойств и связей объекта targetedManagedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 27d275f1cb310d4ab6a82ce394bbd13389ea7917
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939545"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="4ca33-103">Получение targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ca33-103">Get targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="4ca33-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ca33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ca33-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ca33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ca33-106">Чтение свойств и связей объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ca33-106">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ca33-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4ca33-107">Prerequisites</span></span>
<span data-ttu-id="4ca33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ca33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ca33-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ca33-110">Permission type</span></span>|<span data-ttu-id="4ca33-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ca33-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ca33-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ca33-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4ca33-113">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="4ca33-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="4ca33-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ca33-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="4ca33-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="4ca33-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="4ca33-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ca33-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4ca33-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ca33-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ca33-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ca33-118">Not supported.</span></span>|
|<span data-ttu-id="4ca33-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ca33-119">Application</span></span>||
| <span data-ttu-id="4ca33-120">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="4ca33-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="4ca33-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ca33-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="4ca33-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="4ca33-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="4ca33-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ca33-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ca33-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ca33-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ca33-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4ca33-125">Optional query parameters</span></span>
<span data-ttu-id="4ca33-126">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4ca33-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ca33-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ca33-127">Request headers</span></span>
|<span data-ttu-id="4ca33-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ca33-128">Header</span></span>|<span data-ttu-id="4ca33-129">Значение</span><span class="sxs-lookup"><span data-stu-id="4ca33-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ca33-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ca33-130">Authorization</span></span>|<span data-ttu-id="4ca33-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ca33-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ca33-132">Accept</span><span class="sxs-lookup"><span data-stu-id="4ca33-132">Accept</span></span>|<span data-ttu-id="4ca33-133">application/json</span><span class="sxs-lookup"><span data-stu-id="4ca33-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ca33-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4ca33-134">Request body</span></span>
<span data-ttu-id="4ca33-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ca33-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ca33-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ca33-136">Response</span></span>
<span data-ttu-id="4ca33-137">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4ca33-137">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ca33-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4ca33-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ca33-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ca33-139">Request</span></span>
<span data-ttu-id="4ca33-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ca33-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="4ca33-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ca33-141">Response</span></span>
<span data-ttu-id="4ca33-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ca33-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 679

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "2444e029-e029-2444-29e0-442429e04424",
    "version": "Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "deployedAppCount": 0,
    "isAssigned": true
  }
}
```








