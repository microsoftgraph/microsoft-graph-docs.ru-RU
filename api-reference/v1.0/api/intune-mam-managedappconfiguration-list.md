---
title: Перечисление объектов managedAppConfiguration
description: Список свойств и связей объектов managedAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4928bba9def12a2b63e8a729c4cf2f794732736b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43369552"
---
# <a name="list-managedappconfigurations"></a><span data-ttu-id="8fea7-103">Перечисление объектов managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8fea7-103">List managedAppConfigurations</span></span>

<span data-ttu-id="8fea7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fea7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8fea7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8fea7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fea7-106">Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8fea7-106">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fea7-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8fea7-107">Prerequisites</span></span>
<span data-ttu-id="8fea7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fea7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fea7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fea7-110">Permission type</span></span>|<span data-ttu-id="8fea7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fea7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fea7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fea7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8fea7-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8fea7-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8fea7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fea7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fea7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fea7-115">Not supported.</span></span>|
|<span data-ttu-id="8fea7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8fea7-116">Application</span></span>|<span data-ttu-id="8fea7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fea7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fea7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fea7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="8fea7-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8fea7-119">Request headers</span></span>
|<span data-ttu-id="8fea7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8fea7-120">Header</span></span>|<span data-ttu-id="8fea7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8fea7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fea7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fea7-122">Authorization</span></span>|<span data-ttu-id="8fea7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fea7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fea7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8fea7-124">Accept</span></span>|<span data-ttu-id="8fea7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8fea7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fea7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8fea7-126">Request body</span></span>
<span data-ttu-id="8fea7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8fea7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fea7-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="8fea7-128">Response</span></span>
<span data-ttu-id="8fea7-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8fea7-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fea7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8fea7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fea7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fea7-131">Request</span></span>
<span data-ttu-id="8fea7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8fea7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="8fea7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fea7-133">Response</span></span>
<span data-ttu-id="8fea7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8fea7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 592

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppConfiguration",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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






