---
title: Создание объекта managedMobileApp
description: Создание объекта managedMobileApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f6363932442346dbbcfb7350a7ba020de384df53
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803472"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="856dd-103">Создание объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="856dd-103">Create managedMobileApp</span></span>

> <span data-ttu-id="856dd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="856dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="856dd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="856dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="856dd-106">Создание объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="856dd-106">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="856dd-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="856dd-107">Prerequisites</span></span>
<span data-ttu-id="856dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="856dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="856dd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="856dd-110">Permission type</span></span>|<span data-ttu-id="856dd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="856dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="856dd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="856dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="856dd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="856dd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="856dd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="856dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="856dd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="856dd-115">Not supported.</span></span>|
|<span data-ttu-id="856dd-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="856dd-116">Application</span></span>|<span data-ttu-id="856dd-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="856dd-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="856dd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="856dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
POST /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps
POST /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps
```

## <a name="request-headers"></a><span data-ttu-id="856dd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="856dd-119">Request headers</span></span>
|<span data-ttu-id="856dd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="856dd-120">Header</span></span>|<span data-ttu-id="856dd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="856dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="856dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="856dd-122">Authorization</span></span>|<span data-ttu-id="856dd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="856dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="856dd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="856dd-124">Accept</span></span>|<span data-ttu-id="856dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="856dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="856dd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="856dd-126">Request body</span></span>
<span data-ttu-id="856dd-127">В теле запроса добавьте представление объекта managedMobileApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="856dd-127">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="856dd-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="856dd-128">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="856dd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="856dd-129">Property</span></span>|<span data-ttu-id="856dd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="856dd-130">Type</span></span>|<span data-ttu-id="856dd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="856dd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="856dd-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="856dd-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="856dd-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="856dd-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="856dd-134">Идентификатор приложения с типом его операционной системы.</span><span class="sxs-lookup"><span data-stu-id="856dd-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="856dd-135">id</span><span class="sxs-lookup"><span data-stu-id="856dd-135">id</span></span>|<span data-ttu-id="856dd-136">String</span><span class="sxs-lookup"><span data-stu-id="856dd-136">String</span></span>|<span data-ttu-id="856dd-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="856dd-137">Key of the entity.</span></span>|
|<span data-ttu-id="856dd-138">version</span><span class="sxs-lookup"><span data-stu-id="856dd-138">version</span></span>|<span data-ttu-id="856dd-139">String</span><span class="sxs-lookup"><span data-stu-id="856dd-139">String</span></span>|<span data-ttu-id="856dd-140">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="856dd-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="856dd-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="856dd-141">Response</span></span>
<span data-ttu-id="856dd-142">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="856dd-142">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="856dd-143">Пример</span><span class="sxs-lookup"><span data-stu-id="856dd-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="856dd-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="856dd-144">Request</span></span>
<span data-ttu-id="856dd-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="856dd-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="856dd-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="856dd-146">Response</span></span>
<span data-ttu-id="856dd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="856dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 230

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```




