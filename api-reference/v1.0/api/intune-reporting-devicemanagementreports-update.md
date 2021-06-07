---
title: Обновление deviceManagementReports
description: Обновление свойств объекта deviceManagementReports.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d462f754c18c319fb0ca731b8dd51830e2d8dbc
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52749010"
---
# <a name="update-devicemanagementreports"></a><span data-ttu-id="a1d17-103">Обновление deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="a1d17-103">Update deviceManagementReports</span></span>

<span data-ttu-id="a1d17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1d17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1d17-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1d17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1d17-106">Обновление свойств объекта [deviceManagementReports.](../resources/intune-reporting-devicemanagementreports.md)</span><span class="sxs-lookup"><span data-stu-id="a1d17-106">Update the properties of a [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1d17-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a1d17-107">Prerequisites</span></span>
<span data-ttu-id="a1d17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1d17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1d17-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1d17-110">Permission type</span></span>|<span data-ttu-id="a1d17-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1d17-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1d17-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1d17-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1d17-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1d17-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a1d17-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1d17-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1d17-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1d17-115">Not supported.</span></span>|
|<span data-ttu-id="a1d17-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a1d17-116">Application</span></span>|<span data-ttu-id="a1d17-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1d17-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1d17-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1d17-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports
```

## <a name="request-headers"></a><span data-ttu-id="a1d17-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a1d17-119">Request headers</span></span>
|<span data-ttu-id="a1d17-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1d17-120">Header</span></span>|<span data-ttu-id="a1d17-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a1d17-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1d17-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1d17-122">Authorization</span></span>|<span data-ttu-id="a1d17-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1d17-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1d17-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a1d17-124">Accept</span></span>|<span data-ttu-id="a1d17-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1d17-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1d17-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1d17-126">Request body</span></span>
<span data-ttu-id="a1d17-127">В теле запроса поставляем представление JSON для [объекта deviceManagementReports.](../resources/intune-reporting-devicemanagementreports.md)</span><span class="sxs-lookup"><span data-stu-id="a1d17-127">In the request body, supply a JSON representation for the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

<span data-ttu-id="a1d17-128">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementReports.](../resources/intune-reporting-devicemanagementreports.md)</span><span class="sxs-lookup"><span data-stu-id="a1d17-128">The following table shows the properties that are required when you create the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md).</span></span>

|<span data-ttu-id="a1d17-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1d17-129">Property</span></span>|<span data-ttu-id="a1d17-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a1d17-130">Type</span></span>|<span data-ttu-id="a1d17-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a1d17-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1d17-132">id</span><span class="sxs-lookup"><span data-stu-id="a1d17-132">id</span></span>|<span data-ttu-id="a1d17-133">String</span><span class="sxs-lookup"><span data-stu-id="a1d17-133">String</span></span>|<span data-ttu-id="a1d17-134">Уникальный идентификатор для этого объекта</span><span class="sxs-lookup"><span data-stu-id="a1d17-134">Unique identifier for this entity</span></span>|



## <a name="response"></a><span data-ttu-id="a1d17-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1d17-135">Response</span></span>
<span data-ttu-id="a1d17-136">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a1d17-136">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1d17-137">Пример</span><span class="sxs-lookup"><span data-stu-id="a1d17-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1d17-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1d17-138">Request</span></span>
<span data-ttu-id="a1d17-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1d17-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/reports
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.deviceManagementReports"
}
```

### <a name="response"></a><span data-ttu-id="a1d17-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1d17-140">Response</span></span>
<span data-ttu-id="a1d17-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1d17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "d6a697d3-97d3-d6a6-d397-a6d6d397a6d6"
}
```




