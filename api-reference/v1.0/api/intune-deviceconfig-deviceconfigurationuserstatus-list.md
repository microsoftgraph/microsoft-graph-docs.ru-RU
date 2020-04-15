---
title: Перечисление объектов deviceConfigurationUserStatus
description: Список свойств и связей объектов deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c2378d6cce7cb4319b6c56805e7838dfdbe19586
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450586"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="44746-103">Перечисление объектов deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="44746-103">List deviceConfigurationUserStatuses</span></span>

<span data-ttu-id="44746-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44746-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44746-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44746-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44746-106">Список свойств и связей объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="44746-106">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44746-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="44746-107">Prerequisites</span></span>
<span data-ttu-id="44746-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44746-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44746-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44746-110">Permission type</span></span>|<span data-ttu-id="44746-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44746-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44746-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44746-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44746-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="44746-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="44746-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44746-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44746-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44746-115">Not supported.</span></span>|
|<span data-ttu-id="44746-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44746-116">Application</span></span>|<span data-ttu-id="44746-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44746-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44746-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44746-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="44746-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="44746-119">Request headers</span></span>
|<span data-ttu-id="44746-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44746-120">Header</span></span>|<span data-ttu-id="44746-121">Значение</span><span class="sxs-lookup"><span data-stu-id="44746-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44746-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="44746-122">Authorization</span></span>|<span data-ttu-id="44746-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44746-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44746-124">Accept</span><span class="sxs-lookup"><span data-stu-id="44746-124">Accept</span></span>|<span data-ttu-id="44746-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44746-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44746-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44746-126">Request body</span></span>
<span data-ttu-id="44746-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44746-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44746-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="44746-128">Response</span></span>
<span data-ttu-id="44746-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44746-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44746-130">Пример</span><span class="sxs-lookup"><span data-stu-id="44746-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="44746-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="44746-131">Request</span></span>
<span data-ttu-id="44746-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44746-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="44746-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="44746-133">Response</span></span>
<span data-ttu-id="44746-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44746-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
      "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```






