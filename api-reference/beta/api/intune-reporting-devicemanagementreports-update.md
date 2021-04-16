---
title: Обновление deviceManagementReports
description: Обновление свойств объекта deviceManagementReports.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 88569f50004cbf5ec79fa6fa81457990b0356bb1
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866008"
---
# <a name="update-devicemanagementreports"></a><span data-ttu-id="735c2-103">Обновление deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="735c2-103">Update deviceManagementReports</span></span>

<span data-ttu-id="735c2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="735c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="735c2-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="735c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="735c2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="735c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="735c2-107">Обновление свойств объекта [deviceManagementReports.](../resources/intune-reporting-devicemanagementreports.md)</span><span class="sxs-lookup"><span data-stu-id="735c2-107">Update the properties of a [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="735c2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="735c2-108">Prerequisites</span></span>
<span data-ttu-id="735c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="735c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="735c2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="735c2-111">Permission type</span></span>|<span data-ttu-id="735c2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="735c2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="735c2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="735c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="735c2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="735c2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="735c2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="735c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="735c2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="735c2-116">Not supported.</span></span>|
|<span data-ttu-id="735c2-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="735c2-117">Application</span></span>|<span data-ttu-id="735c2-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="735c2-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="735c2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="735c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports
```

## <a name="request-headers"></a><span data-ttu-id="735c2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="735c2-120">Request headers</span></span>
|<span data-ttu-id="735c2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="735c2-121">Header</span></span>|<span data-ttu-id="735c2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="735c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="735c2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="735c2-123">Authorization</span></span>|<span data-ttu-id="735c2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="735c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="735c2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="735c2-125">Accept</span></span>|<span data-ttu-id="735c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="735c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="735c2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="735c2-127">Request body</span></span>
<span data-ttu-id="735c2-128">В теле запроса поставляем представление JSON для [объекта deviceManagementReports.](../resources/intune-reporting-devicemanagementreports.md)</span><span class="sxs-lookup"><span data-stu-id="735c2-128">In the request body, supply a JSON representation for the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

<span data-ttu-id="735c2-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementReports.](../resources/intune-reporting-devicemanagementreports.md)</span><span class="sxs-lookup"><span data-stu-id="735c2-129">The following table shows the properties that are required when you create the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md).</span></span>

|<span data-ttu-id="735c2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="735c2-130">Property</span></span>|<span data-ttu-id="735c2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="735c2-131">Type</span></span>|<span data-ttu-id="735c2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="735c2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="735c2-133">id</span><span class="sxs-lookup"><span data-stu-id="735c2-133">id</span></span>|<span data-ttu-id="735c2-134">String</span><span class="sxs-lookup"><span data-stu-id="735c2-134">String</span></span>|<span data-ttu-id="735c2-135">Уникальный идентификатор для этого объекта</span><span class="sxs-lookup"><span data-stu-id="735c2-135">Unique identifier for this entity</span></span>|



## <a name="response"></a><span data-ttu-id="735c2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="735c2-136">Response</span></span>
<span data-ttu-id="735c2-137">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="735c2-137">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="735c2-138">Пример</span><span class="sxs-lookup"><span data-stu-id="735c2-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="735c2-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="735c2-139">Request</span></span>
<span data-ttu-id="735c2-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="735c2-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.deviceManagementReports"
}
```

### <a name="response"></a><span data-ttu-id="735c2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="735c2-141">Response</span></span>
<span data-ttu-id="735c2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="735c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "d6a697d3-97d3-d6a6-d397-a6d6d397a6d6"
}
```




