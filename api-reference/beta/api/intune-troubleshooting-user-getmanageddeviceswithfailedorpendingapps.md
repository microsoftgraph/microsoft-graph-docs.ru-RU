---
title: Функция Жетманажеддевицесвисфаиледорпендингаппс
description: Получает список устройств с невыполненными или ожидающими приложениями
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ea4f3746c34f0aeed39892aaf0d1b67a9ee16427
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49223202"
---
# <a name="getmanageddeviceswithfailedorpendingapps-function"></a><span data-ttu-id="34aff-103">Функция Жетманажеддевицесвисфаиледорпендингаппс</span><span class="sxs-lookup"><span data-stu-id="34aff-103">getManagedDevicesWithFailedOrPendingApps function</span></span>

<span data-ttu-id="34aff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34aff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34aff-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34aff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34aff-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34aff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34aff-107">Получает список устройств с невыполненными или ожидающими приложениями</span><span class="sxs-lookup"><span data-stu-id="34aff-107">Retrieves the list of devices with failed or pending apps</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34aff-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="34aff-108">Prerequisites</span></span>
<span data-ttu-id="34aff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34aff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34aff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34aff-111">Permission type</span></span>|<span data-ttu-id="34aff-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="34aff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34aff-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34aff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34aff-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="34aff-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="34aff-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34aff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34aff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34aff-116">Not supported.</span></span>|
|<span data-ttu-id="34aff-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="34aff-117">Application</span></span>|<span data-ttu-id="34aff-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="34aff-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34aff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34aff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithFailedOrPendingApps
```

## <a name="request-headers"></a><span data-ttu-id="34aff-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="34aff-120">Request headers</span></span>
|<span data-ttu-id="34aff-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34aff-121">Header</span></span>|<span data-ttu-id="34aff-122">Значение</span><span class="sxs-lookup"><span data-stu-id="34aff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34aff-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34aff-123">Authorization</span></span>|<span data-ttu-id="34aff-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34aff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34aff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="34aff-125">Accept</span></span>|<span data-ttu-id="34aff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34aff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34aff-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34aff-127">Request body</span></span>
<span data-ttu-id="34aff-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34aff-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34aff-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="34aff-129">Response</span></span>
<span data-ttu-id="34aff-130">В случае успеха эта функция возвращает `200 OK` код отклика и коллекцию [манажеддевицесуммаризедаппстате](../resources/intune-troubleshooting-manageddevicesummarizedappstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34aff-130">If successful, this function returns a `200 OK` response code and a [managedDeviceSummarizedAppState](../resources/intune-troubleshooting-manageddevicesummarizedappstate.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34aff-131">Пример</span><span class="sxs-lookup"><span data-stu-id="34aff-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="34aff-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="34aff-132">Request</span></span>
<span data-ttu-id="34aff-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34aff-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithFailedOrPendingApps
```

### <a name="response"></a><span data-ttu-id="34aff-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="34aff-134">Response</span></span>
<span data-ttu-id="34aff-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34aff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 187

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedDeviceSummarizedAppState",
      "summarizedAppState": "success",
      "deviceId": "Device Id value"
    }
  ]
}
```




