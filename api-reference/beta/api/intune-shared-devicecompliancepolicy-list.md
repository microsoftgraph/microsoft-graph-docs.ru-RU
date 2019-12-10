---
title: Перечисление объектов deviceCompliancePolicy
description: Список свойств и связей объектов deviceCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eb2aae4079bc98ad017c315b23c929057f085093
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940112"
---
# <a name="list-devicecompliancepolicies"></a><span data-ttu-id="5e4e0-103">Перечисление объектов deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5e4e0-103">List deviceCompliancePolicies</span></span>

> <span data-ttu-id="5e4e0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e4e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e4e0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e4e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e4e0-106">Список свойств и связей объектов [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5e4e0-106">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e4e0-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5e4e0-107">Prerequisites</span></span>
<span data-ttu-id="5e4e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e4e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e4e0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e4e0-110">Permission type</span></span>|<span data-ttu-id="5e4e0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e4e0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e4e0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e4e0-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5e4e0-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="5e4e0-113">&nbsp; &nbsp; **Device configuration**</span></span>  | <span data-ttu-id="5e4e0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e4e0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="5e4e0-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="5e4e0-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="5e4e0-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e4e0-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5e4e0-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e4e0-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e4e0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e4e0-118">Not supported.</span></span>|
|<span data-ttu-id="5e4e0-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e4e0-119">Application</span></span>||
| <span data-ttu-id="5e4e0-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="5e4e0-120">&nbsp; &nbsp; **Device configuration**</span></span>  | <span data-ttu-id="5e4e0-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e4e0-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="5e4e0-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="5e4e0-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="5e4e0-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e4e0-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e4e0-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e4e0-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="5e4e0-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5e4e0-125">Request headers</span></span>
|<span data-ttu-id="5e4e0-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e4e0-126">Header</span></span>|<span data-ttu-id="5e4e0-127">Значение</span><span class="sxs-lookup"><span data-stu-id="5e4e0-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e4e0-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e4e0-128">Authorization</span></span>|<span data-ttu-id="5e4e0-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e4e0-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e4e0-130">Accept</span><span class="sxs-lookup"><span data-stu-id="5e4e0-130">Accept</span></span>|<span data-ttu-id="5e4e0-131">application/json</span><span class="sxs-lookup"><span data-stu-id="5e4e0-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e4e0-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5e4e0-132">Request body</span></span>
<span data-ttu-id="5e4e0-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5e4e0-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e4e0-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e4e0-134">Response</span></span>
<span data-ttu-id="5e4e0-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e4e0-135">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e4e0-136">Пример</span><span class="sxs-lookup"><span data-stu-id="5e4e0-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e4e0-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e4e0-137">Request</span></span>
<span data-ttu-id="5e4e0-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e4e0-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="5e4e0-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e4e0-139">Response</span></span>
<span data-ttu-id="5e4e0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e4e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 467

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "4214b716-b716-4214-16b7-144216b71442",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```








