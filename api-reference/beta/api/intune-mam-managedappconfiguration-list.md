---
title: Перечисление объектов managedAppConfiguration
description: Список свойств и связей объектов managedAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0357ddb9f47aa98f49347a9ec00170883817276a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078698"
---
# <a name="list-managedappconfigurations"></a><span data-ttu-id="79422-103">Перечисление объектов managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="79422-103">List managedAppConfigurations</span></span>

<span data-ttu-id="79422-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79422-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79422-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79422-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79422-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79422-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79422-107">Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79422-107">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79422-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="79422-108">Prerequisites</span></span>
<span data-ttu-id="79422-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79422-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79422-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79422-111">Permission type</span></span>|<span data-ttu-id="79422-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79422-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79422-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79422-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79422-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="79422-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="79422-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79422-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79422-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79422-116">Not supported.</span></span>|
|<span data-ttu-id="79422-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79422-117">Application</span></span>|<span data-ttu-id="79422-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="79422-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79422-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79422-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="79422-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="79422-120">Request headers</span></span>
|<span data-ttu-id="79422-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79422-121">Header</span></span>|<span data-ttu-id="79422-122">Значение</span><span class="sxs-lookup"><span data-stu-id="79422-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79422-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79422-123">Authorization</span></span>|<span data-ttu-id="79422-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79422-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79422-125">Accept</span><span class="sxs-lookup"><span data-stu-id="79422-125">Accept</span></span>|<span data-ttu-id="79422-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79422-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79422-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79422-127">Request body</span></span>
<span data-ttu-id="79422-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79422-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79422-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="79422-129">Response</span></span>
<span data-ttu-id="79422-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="79422-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79422-131">Пример</span><span class="sxs-lookup"><span data-stu-id="79422-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="79422-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="79422-132">Request</span></span>
<span data-ttu-id="79422-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79422-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="79422-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="79422-134">Response</span></span>
<span data-ttu-id="79422-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79422-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 666

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppConfiguration",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "2ed27cb5-7cb5-2ed2-b57c-d22eb57cd22e",
      "version": "Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```






