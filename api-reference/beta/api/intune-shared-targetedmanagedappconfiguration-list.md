---
title: Перечисление объектов targetedManagedAppConfiguration
description: Список свойств и связей объектов targetedManagedAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 66962de7861d717ee73ba73c32acafa74fcfb753
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465310"
---
# <a name="list-targetedmanagedappconfigurations"></a><span data-ttu-id="b8d5e-103">Перечисление объектов targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b8d5e-103">List targetedManagedAppConfigurations</span></span>

<span data-ttu-id="b8d5e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8d5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8d5e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8d5e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8d5e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8d5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8d5e-107">Список свойств и связей объектов [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8d5e-107">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8d5e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b8d5e-108">Prerequisites</span></span>
<span data-ttu-id="b8d5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8d5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8d5e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8d5e-111">Permission type</span></span>|<span data-ttu-id="b8d5e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8d5e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8d5e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8d5e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b8d5e-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="b8d5e-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="b8d5e-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8d5e-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="b8d5e-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="b8d5e-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b8d5e-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8d5e-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b8d5e-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8d5e-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8d5e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8d5e-119">Not supported.</span></span>|
|<span data-ttu-id="b8d5e-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8d5e-120">Application</span></span>||
| <span data-ttu-id="b8d5e-121">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="b8d5e-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="b8d5e-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8d5e-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="b8d5e-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="b8d5e-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b8d5e-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8d5e-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8d5e-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8d5e-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b8d5e-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b8d5e-126">Request headers</span></span>
|<span data-ttu-id="b8d5e-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8d5e-127">Header</span></span>|<span data-ttu-id="b8d5e-128">Значение</span><span class="sxs-lookup"><span data-stu-id="b8d5e-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8d5e-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8d5e-129">Authorization</span></span>|<span data-ttu-id="b8d5e-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8d5e-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8d5e-131">Accept</span><span class="sxs-lookup"><span data-stu-id="b8d5e-131">Accept</span></span>|<span data-ttu-id="b8d5e-132">application/json</span><span class="sxs-lookup"><span data-stu-id="b8d5e-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8d5e-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b8d5e-133">Request body</span></span>
<span data-ttu-id="b8d5e-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b8d5e-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8d5e-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b8d5e-135">Response</span></span>
<span data-ttu-id="b8d5e-136">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b8d5e-136">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8d5e-137">Пример</span><span class="sxs-lookup"><span data-stu-id="b8d5e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8d5e-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8d5e-138">Request</span></span>
<span data-ttu-id="b8d5e-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8d5e-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
```

### <a name="response"></a><span data-ttu-id="b8d5e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8d5e-140">Response</span></span>
<span data-ttu-id="b8d5e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8d5e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 731

{
  "value": [
    {
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
  ]
}
```






