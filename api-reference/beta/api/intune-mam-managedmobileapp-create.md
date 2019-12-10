---
title: Создание объекта managedMobileApp
description: Создание объекта managedMobileApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 07259080e3d72f32b0cbc2e2659bf1646317f7ad
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39942284"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="08416-103">Создание объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="08416-103">Create managedMobileApp</span></span>

> <span data-ttu-id="08416-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08416-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08416-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08416-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08416-106">Создание объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="08416-106">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08416-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="08416-107">Prerequisites</span></span>
<span data-ttu-id="08416-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08416-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08416-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08416-110">Permission type</span></span>|<span data-ttu-id="08416-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08416-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08416-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08416-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08416-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08416-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="08416-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08416-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08416-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08416-115">Not supported.</span></span>|
|<span data-ttu-id="08416-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08416-116">Application</span></span>|<span data-ttu-id="08416-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08416-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08416-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08416-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="08416-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="08416-119">Request headers</span></span>
|<span data-ttu-id="08416-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08416-120">Header</span></span>|<span data-ttu-id="08416-121">Значение</span><span class="sxs-lookup"><span data-stu-id="08416-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08416-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08416-122">Authorization</span></span>|<span data-ttu-id="08416-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08416-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08416-124">Accept</span><span class="sxs-lookup"><span data-stu-id="08416-124">Accept</span></span>|<span data-ttu-id="08416-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08416-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08416-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="08416-126">Request body</span></span>
<span data-ttu-id="08416-127">В теле запроса добавьте представление объекта managedMobileApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08416-127">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="08416-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="08416-128">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="08416-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="08416-129">Property</span></span>|<span data-ttu-id="08416-130">Тип</span><span class="sxs-lookup"><span data-stu-id="08416-130">Type</span></span>|<span data-ttu-id="08416-131">Описание</span><span class="sxs-lookup"><span data-stu-id="08416-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08416-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="08416-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="08416-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="08416-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="08416-134">Идентификатор приложения с типом его операционной системы.</span><span class="sxs-lookup"><span data-stu-id="08416-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="08416-135">id</span><span class="sxs-lookup"><span data-stu-id="08416-135">id</span></span>|<span data-ttu-id="08416-136">Строка</span><span class="sxs-lookup"><span data-stu-id="08416-136">String</span></span>|<span data-ttu-id="08416-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="08416-137">Key of the entity.</span></span>|
|<span data-ttu-id="08416-138">version</span><span class="sxs-lookup"><span data-stu-id="08416-138">version</span></span>|<span data-ttu-id="08416-139">String</span><span class="sxs-lookup"><span data-stu-id="08416-139">String</span></span>|<span data-ttu-id="08416-140">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="08416-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="08416-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="08416-141">Response</span></span>
<span data-ttu-id="08416-142">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="08416-142">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08416-143">Пример</span><span class="sxs-lookup"><span data-stu-id="08416-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="08416-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="08416-144">Request</span></span>
<span data-ttu-id="08416-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08416-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="08416-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="08416-146">Response</span></span>
<span data-ttu-id="08416-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08416-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





