---
title: Функция Жеткоманажеддевицессуммари
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10bc2573d2bec17f0faf8532237e7a3ebda03cce
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792382"
---
# <a name="getcomanageddevicessummary-function"></a><span data-ttu-id="40922-103">Функция Жеткоманажеддевицессуммари</span><span class="sxs-lookup"><span data-stu-id="40922-103">getComanagedDevicesSummary function</span></span>

<span data-ttu-id="40922-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40922-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40922-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40922-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40922-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40922-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40922-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="40922-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40922-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="40922-108">Prerequisites</span></span>
<span data-ttu-id="40922-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40922-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40922-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40922-111">Permission type</span></span>|<span data-ttu-id="40922-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40922-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40922-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40922-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40922-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="40922-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="40922-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40922-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40922-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40922-116">Not supported.</span></span>|
|<span data-ttu-id="40922-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40922-117">Application</span></span>|<span data-ttu-id="40922-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="40922-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40922-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40922-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getComanagedDevicesSummary
```

## <a name="request-headers"></a><span data-ttu-id="40922-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="40922-120">Request headers</span></span>
|<span data-ttu-id="40922-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40922-121">Header</span></span>|<span data-ttu-id="40922-122">Значение</span><span class="sxs-lookup"><span data-stu-id="40922-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40922-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40922-123">Authorization</span></span>|<span data-ttu-id="40922-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40922-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40922-125">Accept</span><span class="sxs-lookup"><span data-stu-id="40922-125">Accept</span></span>|<span data-ttu-id="40922-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40922-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40922-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="40922-127">Request body</span></span>
<span data-ttu-id="40922-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40922-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40922-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="40922-129">Response</span></span>
<span data-ttu-id="40922-130">В случае успеха эта функция возвращает `200 OK` код отклика и объект [команажеддевицессуммари](../resources/intune-devices-comanageddevicessummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40922-130">If successful, this function returns a `200 OK` response code and a [comanagedDevicesSummary](../resources/intune-devices-comanageddevicessummary.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40922-131">Пример</span><span class="sxs-lookup"><span data-stu-id="40922-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="40922-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="40922-132">Request</span></span>
<span data-ttu-id="40922-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40922-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getComanagedDevicesSummary
```

### <a name="response"></a><span data-ttu-id="40922-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="40922-134">Response</span></span>
<span data-ttu-id="40922-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40922-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 348

{
  "value": {
    "@odata.type": "microsoft.graph.comanagedDevicesSummary",
    "inventoryCount": 14,
    "compliancePolicyCount": 5,
    "resourceAccessCount": 3,
    "configurationSettingsCount": 10,
    "windowsUpdateForBusinessCount": 13,
    "endpointProtectionCount": 7,
    "modernAppsCount": 15,
    "officeAppsCount": 15
  }
}
```



