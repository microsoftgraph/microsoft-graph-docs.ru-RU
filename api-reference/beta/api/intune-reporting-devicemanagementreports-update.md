---
title: Обновление Девицеманажементрепортс
description: Обновление свойств объекта Девицеманажементрепортс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a56d5495f714c639a699aa1d5ccebb81ea2b7c83
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698136"
---
# <a name="update-devicemanagementreports"></a><span data-ttu-id="621f7-103">Обновление Девицеманажементрепортс</span><span class="sxs-lookup"><span data-stu-id="621f7-103">Update deviceManagementReports</span></span>

<span data-ttu-id="621f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="621f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="621f7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="621f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="621f7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="621f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="621f7-107">Обновление свойств объекта [девицеманажементрепортс](../resources/intune-reporting-devicemanagementreports.md) .</span><span class="sxs-lookup"><span data-stu-id="621f7-107">Update the properties of a [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="621f7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="621f7-108">Prerequisites</span></span>
<span data-ttu-id="621f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="621f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="621f7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="621f7-111">Permission type</span></span>|<span data-ttu-id="621f7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="621f7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="621f7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="621f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="621f7-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="621f7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="621f7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="621f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="621f7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="621f7-116">Not supported.</span></span>|
|<span data-ttu-id="621f7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="621f7-117">Application</span></span>|<span data-ttu-id="621f7-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="621f7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="621f7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="621f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports
```

## <a name="request-headers"></a><span data-ttu-id="621f7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="621f7-120">Request headers</span></span>
|<span data-ttu-id="621f7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="621f7-121">Header</span></span>|<span data-ttu-id="621f7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="621f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="621f7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="621f7-123">Authorization</span></span>|<span data-ttu-id="621f7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="621f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="621f7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="621f7-125">Accept</span></span>|<span data-ttu-id="621f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="621f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="621f7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="621f7-127">Request body</span></span>
<span data-ttu-id="621f7-128">В тексте запроса добавьте представление объекта [девицеманажементрепортс](../resources/intune-reporting-devicemanagementreports.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="621f7-128">In the request body, supply a JSON representation for the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

<span data-ttu-id="621f7-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементрепортс](../resources/intune-reporting-devicemanagementreports.md).</span><span class="sxs-lookup"><span data-stu-id="621f7-129">The following table shows the properties that are required when you create the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md).</span></span>

|<span data-ttu-id="621f7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="621f7-130">Property</span></span>|<span data-ttu-id="621f7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="621f7-131">Type</span></span>|<span data-ttu-id="621f7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="621f7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="621f7-133">id</span><span class="sxs-lookup"><span data-stu-id="621f7-133">id</span></span>|<span data-ttu-id="621f7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="621f7-134">String</span></span>|<span data-ttu-id="621f7-135">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="621f7-135">Unique identifier for this entity</span></span>|



## <a name="response"></a><span data-ttu-id="621f7-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="621f7-136">Response</span></span>
<span data-ttu-id="621f7-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементрепортс](../resources/intune-reporting-devicemanagementreports.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="621f7-137">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="621f7-138">Пример</span><span class="sxs-lookup"><span data-stu-id="621f7-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="621f7-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="621f7-139">Request</span></span>
<span data-ttu-id="621f7-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="621f7-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.deviceManagementReports"
}
```

### <a name="response"></a><span data-ttu-id="621f7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="621f7-141">Response</span></span>
<span data-ttu-id="621f7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="621f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "d6a697d3-97d3-d6a6-d397-a6d6d397a6d6"
}
```





