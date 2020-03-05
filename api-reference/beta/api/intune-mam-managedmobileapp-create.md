---
title: Создание объекта managedMobileApp
description: Создание объекта managedMobileApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1594c06e87aa89f8b599c27426769a28740a0300
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463295"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="d083f-103">Создание объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="d083f-103">Create managedMobileApp</span></span>

<span data-ttu-id="d083f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d083f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d083f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d083f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d083f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d083f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d083f-107">Создание объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d083f-107">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d083f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d083f-108">Prerequisites</span></span>
<span data-ttu-id="d083f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d083f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d083f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d083f-111">Permission type</span></span>|<span data-ttu-id="d083f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d083f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d083f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d083f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d083f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d083f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d083f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d083f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d083f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d083f-116">Not supported.</span></span>|
|<span data-ttu-id="d083f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d083f-117">Application</span></span>|<span data-ttu-id="d083f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d083f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d083f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d083f-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d083f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d083f-120">Request headers</span></span>
|<span data-ttu-id="d083f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d083f-121">Header</span></span>|<span data-ttu-id="d083f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d083f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d083f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d083f-123">Authorization</span></span>|<span data-ttu-id="d083f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d083f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d083f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d083f-125">Accept</span></span>|<span data-ttu-id="d083f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d083f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d083f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d083f-127">Request body</span></span>
<span data-ttu-id="d083f-128">В теле запроса добавьте представление объекта managedMobileApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d083f-128">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="d083f-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="d083f-129">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="d083f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d083f-130">Property</span></span>|<span data-ttu-id="d083f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d083f-131">Type</span></span>|<span data-ttu-id="d083f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d083f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d083f-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d083f-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="d083f-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d083f-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="d083f-135">Идентификатор приложения с типом его операционной системы.</span><span class="sxs-lookup"><span data-stu-id="d083f-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="d083f-136">id</span><span class="sxs-lookup"><span data-stu-id="d083f-136">id</span></span>|<span data-ttu-id="d083f-137">String</span><span class="sxs-lookup"><span data-stu-id="d083f-137">String</span></span>|<span data-ttu-id="d083f-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d083f-138">Key of the entity.</span></span>|
|<span data-ttu-id="d083f-139">version</span><span class="sxs-lookup"><span data-stu-id="d083f-139">version</span></span>|<span data-ttu-id="d083f-140">String</span><span class="sxs-lookup"><span data-stu-id="d083f-140">String</span></span>|<span data-ttu-id="d083f-141">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="d083f-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="d083f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d083f-142">Response</span></span>
<span data-ttu-id="d083f-143">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d083f-143">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d083f-144">Пример</span><span class="sxs-lookup"><span data-stu-id="d083f-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="d083f-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="d083f-145">Request</span></span>
<span data-ttu-id="d083f-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d083f-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d083f-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="d083f-147">Response</span></span>
<span data-ttu-id="d083f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d083f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





