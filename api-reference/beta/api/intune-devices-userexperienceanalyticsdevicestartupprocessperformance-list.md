---
title: Список Усерекспериенцеаналитиксдевицестартуппроцессперформанцес
description: Список свойств и связей объектов Усерекспериенцеаналитиксдевицестартуппроцессперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 52d8ea1bb4643aaaea63e45f75af8eb7c4d393c7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49202495"
---
# <a name="list-userexperienceanalyticsdevicestartupprocessperformances"></a><span data-ttu-id="97145-103">Список Усерекспериенцеаналитиксдевицестартуппроцессперформанцес</span><span class="sxs-lookup"><span data-stu-id="97145-103">List userExperienceAnalyticsDeviceStartupProcessPerformances</span></span>

<span data-ttu-id="97145-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97145-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97145-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97145-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97145-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97145-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97145-107">Список свойств и связей объектов [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="97145-107">List properties and relationships of the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97145-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="97145-108">Prerequisites</span></span>
<span data-ttu-id="97145-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97145-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97145-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97145-111">Permission type</span></span>|<span data-ttu-id="97145-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="97145-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97145-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97145-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97145-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="97145-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="97145-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97145-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97145-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97145-116">Not supported.</span></span>|
|<span data-ttu-id="97145-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="97145-117">Application</span></span>|<span data-ttu-id="97145-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="97145-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97145-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97145-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
```

## <a name="request-headers"></a><span data-ttu-id="97145-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="97145-120">Request headers</span></span>
|<span data-ttu-id="97145-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97145-121">Header</span></span>|<span data-ttu-id="97145-122">Значение</span><span class="sxs-lookup"><span data-stu-id="97145-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97145-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97145-123">Authorization</span></span>|<span data-ttu-id="97145-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97145-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97145-125">Accept</span><span class="sxs-lookup"><span data-stu-id="97145-125">Accept</span></span>|<span data-ttu-id="97145-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97145-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97145-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97145-127">Request body</span></span>
<span data-ttu-id="97145-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97145-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97145-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="97145-129">Response</span></span>
<span data-ttu-id="97145-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="97145-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97145-131">Пример</span><span class="sxs-lookup"><span data-stu-id="97145-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="97145-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="97145-132">Request</span></span>
<span data-ttu-id="97145-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97145-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
```

### <a name="response"></a><span data-ttu-id="97145-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="97145-134">Response</span></span>
<span data-ttu-id="97145-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97145-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 399

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
      "id": "86c4355c-355c-86c4-5c35-c4865c35c486",
      "processName": "Process Name value",
      "productName": "Product Name value",
      "publisher": "Publisher value",
      "deviceCount": 11,
      "medianImpactInMs": 0,
      "totalImpactInMs": 15
    }
  ]
}
```




