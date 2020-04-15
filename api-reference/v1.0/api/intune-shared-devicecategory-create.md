---
title: Создание объекта deviceCategory
description: Создание объекта deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: da7ecf3988c83aa7ef7f2fc16ac98271518e3c6b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465811"
---
# <a name="create-devicecategory"></a><span data-ttu-id="c5a9d-103">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="c5a9d-103">Create deviceCategory</span></span>

<span data-ttu-id="c5a9d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5a9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5a9d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5a9d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5a9d-106">Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="c5a9d-106">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5a9d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c5a9d-107">Prerequisites</span></span>
<span data-ttu-id="c5a9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5a9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5a9d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5a9d-110">Permission type</span></span>|<span data-ttu-id="c5a9d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5a9d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5a9d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5a9d-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c5a9d-113">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c5a9d-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c5a9d-114">Девицеманажементманажед Devices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c5a9d-114">DeviceManagementManaged Devices.ReadWrite.All</span></span>|
|<span data-ttu-id="c5a9d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5a9d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5a9d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5a9d-116">Not supported.</span></span>|
|<span data-ttu-id="c5a9d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5a9d-117">Application</span></span>|<span data-ttu-id="c5a9d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5a9d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5a9d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5a9d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="c5a9d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c5a9d-120">Request headers</span></span>
|<span data-ttu-id="c5a9d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5a9d-121">Header</span></span>|<span data-ttu-id="c5a9d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c5a9d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5a9d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5a9d-123">Authorization</span></span>|<span data-ttu-id="c5a9d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5a9d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5a9d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5a9d-125">Accept</span></span>|<span data-ttu-id="c5a9d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5a9d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5a9d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c5a9d-127">Request body</span></span>
<span data-ttu-id="c5a9d-128">В теле запроса добавьте представление объекта deviceCategory в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5a9d-128">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="c5a9d-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="c5a9d-129">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="c5a9d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5a9d-130">Property</span></span>|<span data-ttu-id="c5a9d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c5a9d-131">Type</span></span>|<span data-ttu-id="c5a9d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c5a9d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5a9d-133">id</span><span class="sxs-lookup"><span data-stu-id="c5a9d-133">id</span></span>|<span data-ttu-id="c5a9d-134">String</span><span class="sxs-lookup"><span data-stu-id="c5a9d-134">String</span></span>|<span data-ttu-id="c5a9d-135">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="c5a9d-135">Unique identifier for the device category.</span></span> <span data-ttu-id="c5a9d-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c5a9d-136">Read-only.</span></span>|
|<span data-ttu-id="c5a9d-137">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c5a9d-137">**Onboarding**</span></span>|
|<span data-ttu-id="c5a9d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="c5a9d-138">displayName</span></span>|<span data-ttu-id="c5a9d-139">Строка</span><span class="sxs-lookup"><span data-stu-id="c5a9d-139">String</span></span>|<span data-ttu-id="c5a9d-140">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="c5a9d-140">Display name for the device category.</span></span>|
|<span data-ttu-id="c5a9d-141">description</span><span class="sxs-lookup"><span data-stu-id="c5a9d-141">description</span></span>|<span data-ttu-id="c5a9d-142">String</span><span class="sxs-lookup"><span data-stu-id="c5a9d-142">String</span></span>|<span data-ttu-id="c5a9d-143">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="c5a9d-143">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="c5a9d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5a9d-144">Response</span></span>
<span data-ttu-id="c5a9d-145">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c5a9d-145">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5a9d-146">Пример</span><span class="sxs-lookup"><span data-stu-id="c5a9d-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="c5a9d-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5a9d-147">Request</span></span>
<span data-ttu-id="c5a9d-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5a9d-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c5a9d-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5a9d-149">Response</span></span>
<span data-ttu-id="c5a9d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5a9d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






