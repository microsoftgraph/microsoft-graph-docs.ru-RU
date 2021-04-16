---
title: Перечисление объектов targetedManagedAppConfiguration
description: Список свойств и связей объектов targetedManagedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 56aa751eafe45534055bc661640d1781818f95c4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864573"
---
# <a name="list-targetedmanagedappconfigurations"></a><span data-ttu-id="1e838-103">Перечисление объектов targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1e838-103">List targetedManagedAppConfigurations</span></span>

<span data-ttu-id="1e838-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e838-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e838-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e838-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e838-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1e838-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e838-107">Список свойств и связей объектов [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e838-107">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e838-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1e838-108">Prerequisites</span></span>
<span data-ttu-id="1e838-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e838-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e838-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e838-111">Permission type</span></span>|<span data-ttu-id="1e838-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e838-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e838-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e838-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1e838-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="1e838-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="1e838-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e838-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="1e838-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="1e838-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="1e838-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e838-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1e838-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e838-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e838-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e838-119">Not supported.</span></span>|
|<span data-ttu-id="1e838-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="1e838-120">Application</span></span>||
| <span data-ttu-id="1e838-121">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="1e838-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="1e838-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e838-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="1e838-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="1e838-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="1e838-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e838-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e838-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e838-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1e838-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1e838-126">Request headers</span></span>
|<span data-ttu-id="1e838-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1e838-127">Header</span></span>|<span data-ttu-id="1e838-128">Значение</span><span class="sxs-lookup"><span data-stu-id="1e838-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e838-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1e838-129">Authorization</span></span>|<span data-ttu-id="1e838-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e838-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e838-131">Accept</span><span class="sxs-lookup"><span data-stu-id="1e838-131">Accept</span></span>|<span data-ttu-id="1e838-132">application/json</span><span class="sxs-lookup"><span data-stu-id="1e838-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e838-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e838-133">Request body</span></span>
<span data-ttu-id="1e838-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1e838-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e838-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e838-135">Response</span></span>
<span data-ttu-id="1e838-136">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1e838-136">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e838-137">Пример</span><span class="sxs-lookup"><span data-stu-id="1e838-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e838-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e838-138">Request</span></span>
<span data-ttu-id="1e838-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e838-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
```

### <a name="response"></a><span data-ttu-id="1e838-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e838-140">Response</span></span>
<span data-ttu-id="1e838-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1e838-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







