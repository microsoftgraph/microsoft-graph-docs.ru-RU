---
title: Функция Жеткоманажеддевицессуммари
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 44dd46dc5fd48127ed380a50a9d43f98bb2364bb
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792494"
---
# <a name="getcomanageddevicessummary-function"></a><span data-ttu-id="b4477-103">Функция Жеткоманажеддевицессуммари</span><span class="sxs-lookup"><span data-stu-id="b4477-103">getComanagedDevicesSummary function</span></span>

<span data-ttu-id="b4477-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4477-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4477-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4477-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4477-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4477-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4477-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b4477-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4477-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b4477-108">Prerequisites</span></span>
<span data-ttu-id="b4477-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4477-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4477-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4477-111">Permission type</span></span>|<span data-ttu-id="b4477-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4477-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4477-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4477-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4477-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4477-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b4477-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4477-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4477-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4477-116">Not supported.</span></span>|
|<span data-ttu-id="b4477-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b4477-117">Application</span></span>|<span data-ttu-id="b4477-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4477-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4477-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4477-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getComanagedDevicesSummary
```

## <a name="request-headers"></a><span data-ttu-id="b4477-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b4477-120">Request headers</span></span>
|<span data-ttu-id="b4477-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4477-121">Header</span></span>|<span data-ttu-id="b4477-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b4477-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4477-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4477-123">Authorization</span></span>|<span data-ttu-id="b4477-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4477-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4477-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b4477-125">Accept</span></span>|<span data-ttu-id="b4477-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4477-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4477-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4477-127">Request body</span></span>
<span data-ttu-id="b4477-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4477-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4477-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4477-129">Response</span></span>
<span data-ttu-id="b4477-130">В случае успеха эта функция возвращает `200 OK` код отклика и объект [команажеддевицессуммари](../resources/intune-devices-comanageddevicessummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4477-130">If successful, this function returns a `200 OK` response code and a [comanagedDevicesSummary](../resources/intune-devices-comanageddevicessummary.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4477-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b4477-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4477-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4477-132">Request</span></span>
<span data-ttu-id="b4477-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4477-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getComanagedDevicesSummary
```

### <a name="response"></a><span data-ttu-id="b4477-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4477-134">Response</span></span>
<span data-ttu-id="b4477-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4477-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 379

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
    "officeAppsCount": 15,
    "totalComanagedCount": 3
  }
}
```



