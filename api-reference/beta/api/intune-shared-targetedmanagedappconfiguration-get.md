---
title: Получение targetedManagedAppConfiguration
description: Чтение свойств и связей объекта targetedManagedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4394f541d46195a4c3987a4cdeec667eb0316a95
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865651"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="51edd-103">Получение targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="51edd-103">Get targetedManagedAppConfiguration</span></span>

<span data-ttu-id="51edd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51edd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51edd-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51edd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51edd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51edd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51edd-107">Чтение свойств и связей объекта [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51edd-107">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51edd-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="51edd-108">Prerequisites</span></span>
<span data-ttu-id="51edd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51edd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51edd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51edd-111">Permission type</span></span>|<span data-ttu-id="51edd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51edd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51edd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51edd-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="51edd-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="51edd-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="51edd-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="51edd-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="51edd-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="51edd-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="51edd-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="51edd-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="51edd-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51edd-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51edd-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51edd-119">Not supported.</span></span>|
|<span data-ttu-id="51edd-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="51edd-120">Application</span></span>||
| <span data-ttu-id="51edd-121">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="51edd-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="51edd-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="51edd-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="51edd-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="51edd-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="51edd-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="51edd-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51edd-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51edd-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51edd-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51edd-126">Optional query parameters</span></span>
<span data-ttu-id="51edd-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="51edd-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51edd-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51edd-128">Request headers</span></span>
|<span data-ttu-id="51edd-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51edd-129">Header</span></span>|<span data-ttu-id="51edd-130">Значение</span><span class="sxs-lookup"><span data-stu-id="51edd-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51edd-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51edd-131">Authorization</span></span>|<span data-ttu-id="51edd-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51edd-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51edd-133">Accept</span><span class="sxs-lookup"><span data-stu-id="51edd-133">Accept</span></span>|<span data-ttu-id="51edd-134">application/json</span><span class="sxs-lookup"><span data-stu-id="51edd-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51edd-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51edd-135">Request body</span></span>
<span data-ttu-id="51edd-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51edd-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51edd-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="51edd-137">Response</span></span>
<span data-ttu-id="51edd-138">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="51edd-138">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51edd-139">Пример</span><span class="sxs-lookup"><span data-stu-id="51edd-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="51edd-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="51edd-140">Request</span></span>
<span data-ttu-id="51edd-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51edd-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="51edd-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="51edd-142">Response</span></span>
<span data-ttu-id="51edd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51edd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







