---
title: Получение targetedManagedAppConfiguration
description: Чтение свойств и связей объекта targetedManagedAppConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5210cf43292a70dedd41bb19f048d70454ac996b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800636"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="b0fc2-103">Получение targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b0fc2-103">Get targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="b0fc2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0fc2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0fc2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0fc2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0fc2-106">Чтение свойств и связей объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b0fc2-106">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0fc2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b0fc2-107">Prerequisites</span></span>
<span data-ttu-id="b0fc2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0fc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0fc2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0fc2-110">Permission type</span></span>|<span data-ttu-id="b0fc2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0fc2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0fc2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0fc2-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b0fc2-113">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="b0fc2-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="b0fc2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0fc2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="b0fc2-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="b0fc2-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b0fc2-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0fc2-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b0fc2-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0fc2-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0fc2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0fc2-118">Not supported.</span></span>|
|<span data-ttu-id="b0fc2-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="b0fc2-119">Application</span></span>||
| <span data-ttu-id="b0fc2-120">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="b0fc2-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="b0fc2-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0fc2-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="b0fc2-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="b0fc2-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b0fc2-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0fc2-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0fc2-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0fc2-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0fc2-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b0fc2-125">Optional query parameters</span></span>
<span data-ttu-id="b0fc2-126">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b0fc2-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0fc2-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0fc2-127">Request headers</span></span>
|<span data-ttu-id="b0fc2-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0fc2-128">Header</span></span>|<span data-ttu-id="b0fc2-129">Значение</span><span class="sxs-lookup"><span data-stu-id="b0fc2-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0fc2-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0fc2-130">Authorization</span></span>|<span data-ttu-id="b0fc2-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0fc2-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0fc2-132">Accept</span><span class="sxs-lookup"><span data-stu-id="b0fc2-132">Accept</span></span>|<span data-ttu-id="b0fc2-133">application/json</span><span class="sxs-lookup"><span data-stu-id="b0fc2-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0fc2-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0fc2-134">Request body</span></span>
<span data-ttu-id="b0fc2-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0fc2-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0fc2-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0fc2-136">Response</span></span>
<span data-ttu-id="b0fc2-137">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b0fc2-137">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0fc2-138">Пример</span><span class="sxs-lookup"><span data-stu-id="b0fc2-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0fc2-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0fc2-139">Request</span></span>
<span data-ttu-id="b0fc2-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0fc2-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b0fc2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0fc2-141">Response</span></span>
<span data-ttu-id="b0fc2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0fc2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







