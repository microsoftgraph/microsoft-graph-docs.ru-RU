---
title: Список Секуритибаселинедевицестатес
description: Список свойств и связей объектов Секуритибаселинедевицестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7bae038d7a2e9d14e60d11d330d29be78a3c19f1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058937"
---
# <a name="list-securitybaselinedevicestates"></a><span data-ttu-id="73957-103">Список Секуритибаселинедевицестатес</span><span class="sxs-lookup"><span data-stu-id="73957-103">List securityBaselineDeviceStates</span></span>

<span data-ttu-id="73957-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73957-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73957-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73957-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73957-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73957-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73957-107">Список свойств и связей объектов [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="73957-107">List properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73957-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="73957-108">Prerequisites</span></span>
<span data-ttu-id="73957-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73957-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73957-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73957-111">Permission type</span></span>|<span data-ttu-id="73957-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73957-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73957-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73957-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73957-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73957-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="73957-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73957-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73957-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73957-116">Not supported.</span></span>|
|<span data-ttu-id="73957-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73957-117">Application</span></span>|<span data-ttu-id="73957-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73957-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73957-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73957-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="73957-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="73957-120">Request headers</span></span>
|<span data-ttu-id="73957-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73957-121">Header</span></span>|<span data-ttu-id="73957-122">Значение</span><span class="sxs-lookup"><span data-stu-id="73957-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73957-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73957-123">Authorization</span></span>|<span data-ttu-id="73957-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73957-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73957-125">Accept</span><span class="sxs-lookup"><span data-stu-id="73957-125">Accept</span></span>|<span data-ttu-id="73957-126">application/json</span><span class="sxs-lookup"><span data-stu-id="73957-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73957-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73957-127">Request body</span></span>
<span data-ttu-id="73957-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73957-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73957-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="73957-129">Response</span></span>
<span data-ttu-id="73957-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73957-130">If successful, this method returns a `200 OK` response code and a collection of [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73957-131">Пример</span><span class="sxs-lookup"><span data-stu-id="73957-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="73957-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="73957-132">Request</span></span>
<span data-ttu-id="73957-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73957-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
```

### <a name="response"></a><span data-ttu-id="73957-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="73957-134">Response</span></span>
<span data-ttu-id="73957-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73957-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 420

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
      "id": "182749bf-49bf-1827-bf49-2718bf492718",
      "managedDeviceId": "Managed Device Id value",
      "deviceDisplayName": "Device Display Name value",
      "userPrincipalName": "User Principal Name value",
      "state": "secure",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
    }
  ]
}
```






