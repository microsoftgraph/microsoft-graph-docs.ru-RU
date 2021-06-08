---
title: Создание объекта deviceCategory
description: Создание объекта deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9b1bfb046b4a1949ddba846d5a30c34256198049
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759600"
---
# <a name="create-devicecategory"></a><span data-ttu-id="0d5cc-103">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0d5cc-103">Create deviceCategory</span></span>

<span data-ttu-id="0d5cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d5cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d5cc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d5cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d5cc-106">Создание объекта [deviceCategory](../resources/intune-onboarding-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="0d5cc-106">Create a new [deviceCategory](../resources/intune-onboarding-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d5cc-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0d5cc-107">Prerequisites</span></span>
<span data-ttu-id="0d5cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d5cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d5cc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d5cc-110">Permission type</span></span>|<span data-ttu-id="0d5cc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d5cc-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d5cc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d5cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d5cc-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d5cc-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0d5cc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d5cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d5cc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d5cc-115">Not supported.</span></span>|
|<span data-ttu-id="0d5cc-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0d5cc-116">Application</span></span>|<span data-ttu-id="0d5cc-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d5cc-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d5cc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d5cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="0d5cc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0d5cc-119">Request headers</span></span>
|<span data-ttu-id="0d5cc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d5cc-120">Header</span></span>|<span data-ttu-id="0d5cc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0d5cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d5cc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d5cc-122">Authorization</span></span>|<span data-ttu-id="0d5cc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d5cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d5cc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0d5cc-124">Accept</span></span>|<span data-ttu-id="0d5cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0d5cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d5cc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d5cc-126">Request body</span></span>
<span data-ttu-id="0d5cc-127">В теле запроса добавьте представление объекта deviceCategory в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d5cc-127">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="0d5cc-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="0d5cc-128">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="0d5cc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d5cc-129">Property</span></span>|<span data-ttu-id="0d5cc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0d5cc-130">Type</span></span>|<span data-ttu-id="0d5cc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0d5cc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d5cc-132">id</span><span class="sxs-lookup"><span data-stu-id="0d5cc-132">id</span></span>|<span data-ttu-id="0d5cc-133">String</span><span class="sxs-lookup"><span data-stu-id="0d5cc-133">String</span></span>|<span data-ttu-id="0d5cc-134">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="0d5cc-134">Unique identifier for the device category.</span></span> <span data-ttu-id="0d5cc-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d5cc-135">Read-only.</span></span>|
|<span data-ttu-id="0d5cc-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0d5cc-136">displayName</span></span>|<span data-ttu-id="0d5cc-137">String</span><span class="sxs-lookup"><span data-stu-id="0d5cc-137">String</span></span>|<span data-ttu-id="0d5cc-138">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="0d5cc-138">Display name for the device category.</span></span>|
|<span data-ttu-id="0d5cc-139">description</span><span class="sxs-lookup"><span data-stu-id="0d5cc-139">description</span></span>|<span data-ttu-id="0d5cc-140">String</span><span class="sxs-lookup"><span data-stu-id="0d5cc-140">String</span></span>|<span data-ttu-id="0d5cc-141">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="0d5cc-141">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="0d5cc-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d5cc-142">Response</span></span>
<span data-ttu-id="0d5cc-143">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCategory](../resources/intune-onboarding-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0d5cc-143">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-onboarding-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d5cc-144">Пример</span><span class="sxs-lookup"><span data-stu-id="0d5cc-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d5cc-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d5cc-145">Request</span></span>
<span data-ttu-id="0d5cc-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d5cc-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="0d5cc-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d5cc-147">Response</span></span>
<span data-ttu-id="0d5cc-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d5cc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```




