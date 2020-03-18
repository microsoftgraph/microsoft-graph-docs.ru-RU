---
title: Список Усерекспериенцеаналитиксбаселинес
description: Список свойств и связей объектов Усерекспериенцеаналитиксбаселине.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 29a3ad020542cba558d50375248da2ea0d1a6fd7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814023"
---
# <a name="list-userexperienceanalyticsbaselines"></a><span data-ttu-id="6ec18-103">Список Усерекспериенцеаналитиксбаселинес</span><span class="sxs-lookup"><span data-stu-id="6ec18-103">List userExperienceAnalyticsBaselines</span></span>

> <span data-ttu-id="6ec18-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ec18-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ec18-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ec18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ec18-106">Список свойств и связей объектов [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) .</span><span class="sxs-lookup"><span data-stu-id="6ec18-106">List properties and relationships of the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ec18-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6ec18-107">Prerequisites</span></span>
<span data-ttu-id="6ec18-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ec18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ec18-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ec18-110">Permission type</span></span>|<span data-ttu-id="6ec18-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ec18-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ec18-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ec18-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6ec18-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ec18-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6ec18-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ec18-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ec18-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ec18-115">Not supported.</span></span>|
|<span data-ttu-id="6ec18-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6ec18-116">Application</span></span>|<span data-ttu-id="6ec18-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ec18-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ec18-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ec18-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsBaselines
```

## <a name="request-headers"></a><span data-ttu-id="6ec18-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6ec18-119">Request headers</span></span>
|<span data-ttu-id="6ec18-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ec18-120">Header</span></span>|<span data-ttu-id="6ec18-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6ec18-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ec18-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ec18-122">Authorization</span></span>|<span data-ttu-id="6ec18-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ec18-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ec18-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6ec18-124">Accept</span></span>|<span data-ttu-id="6ec18-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6ec18-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ec18-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ec18-126">Request body</span></span>
<span data-ttu-id="6ec18-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ec18-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ec18-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ec18-128">Response</span></span>
<span data-ttu-id="6ec18-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6ec18-129">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ec18-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6ec18-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ec18-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ec18-131">Request</span></span>
<span data-ttu-id="6ec18-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ec18-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines
```

### <a name="response"></a><span data-ttu-id="6ec18-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ec18-133">Response</span></span>
<span data-ttu-id="6ec18-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ec18-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 323

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
      "id": "1cce2cab-2cab-1cce-ab2c-ce1cab2cce1c",
      "displayName": "Display Name value",
      "overallScore": 12,
      "isBuiltIn": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00"
    }
  ]
}
```




