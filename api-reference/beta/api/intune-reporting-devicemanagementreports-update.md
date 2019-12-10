---
title: Обновление Девицеманажементрепортс
description: Обновление свойств объекта Девицеманажементрепортс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 41649751eb195aff05adcd1867ede27b3b47e7b8
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940273"
---
# <a name="update-devicemanagementreports"></a><span data-ttu-id="5a929-103">Обновление Девицеманажементрепортс</span><span class="sxs-lookup"><span data-stu-id="5a929-103">Update deviceManagementReports</span></span>

> <span data-ttu-id="5a929-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a929-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a929-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a929-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a929-106">Обновление свойств объекта [девицеманажементрепортс](../resources/intune-reporting-devicemanagementreports.md) .</span><span class="sxs-lookup"><span data-stu-id="5a929-106">Update the properties of a [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a929-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5a929-107">Prerequisites</span></span>
<span data-ttu-id="5a929-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a929-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a929-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a929-110">Permission type</span></span>|<span data-ttu-id="5a929-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a929-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a929-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a929-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a929-113">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5a929-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5a929-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a929-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a929-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a929-115">Not supported.</span></span>|
|<span data-ttu-id="5a929-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a929-116">Application</span></span>|<span data-ttu-id="5a929-117">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5a929-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a929-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a929-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports
```

## <a name="request-headers"></a><span data-ttu-id="5a929-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5a929-119">Request headers</span></span>
|<span data-ttu-id="5a929-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a929-120">Header</span></span>|<span data-ttu-id="5a929-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5a929-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a929-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a929-122">Authorization</span></span>|<span data-ttu-id="5a929-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a929-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a929-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5a929-124">Accept</span></span>|<span data-ttu-id="5a929-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5a929-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a929-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5a929-126">Request body</span></span>
<span data-ttu-id="5a929-127">В тексте запроса добавьте представление объекта [девицеманажементрепортс](../resources/intune-reporting-devicemanagementreports.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a929-127">In the request body, supply a JSON representation for the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

<span data-ttu-id="5a929-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементрепортс](../resources/intune-reporting-devicemanagementreports.md).</span><span class="sxs-lookup"><span data-stu-id="5a929-128">The following table shows the properties that are required when you create the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md).</span></span>

|<span data-ttu-id="5a929-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a929-129">Property</span></span>|<span data-ttu-id="5a929-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5a929-130">Type</span></span>|<span data-ttu-id="5a929-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5a929-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a929-132">id</span><span class="sxs-lookup"><span data-stu-id="5a929-132">id</span></span>|<span data-ttu-id="5a929-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5a929-133">String</span></span>|<span data-ttu-id="5a929-134">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="5a929-134">Unique identifier for this entity</span></span>|



## <a name="response"></a><span data-ttu-id="5a929-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a929-135">Response</span></span>
<span data-ttu-id="5a929-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементрепортс](../resources/intune-reporting-devicemanagementreports.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a929-136">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a929-137">Пример</span><span class="sxs-lookup"><span data-stu-id="5a929-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a929-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a929-138">Request</span></span>
<span data-ttu-id="5a929-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a929-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.deviceManagementReports"
}
```

### <a name="response"></a><span data-ttu-id="5a929-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a929-140">Response</span></span>
<span data-ttu-id="5a929-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a929-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "d6a697d3-97d3-d6a6-d397-a6d6d397a6d6"
}
```





