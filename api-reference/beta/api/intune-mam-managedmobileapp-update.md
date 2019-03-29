---
title: Обновление объекта managedMobileApp
description: Обновление свойств объекта managedMobileApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 378c28bfee54090fd0802ff4c5ae61b262adf41f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972328"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="084cb-103">Обновление объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="084cb-103">Update managedMobileApp</span></span>

> <span data-ttu-id="084cb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="084cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="084cb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="084cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="084cb-106">Обновление свойств объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="084cb-106">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="084cb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="084cb-107">Prerequisites</span></span>
<span data-ttu-id="084cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="084cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="084cb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="084cb-110">Permission type</span></span>|<span data-ttu-id="084cb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="084cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="084cb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="084cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="084cb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="084cb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="084cb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="084cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="084cb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="084cb-115">Not supported.</span></span>|
|<span data-ttu-id="084cb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="084cb-116">Application</span></span>|<span data-ttu-id="084cb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="084cb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="084cb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="084cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="084cb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="084cb-119">Request headers</span></span>
|<span data-ttu-id="084cb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="084cb-120">Header</span></span>|<span data-ttu-id="084cb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="084cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="084cb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="084cb-122">Authorization</span></span>|<span data-ttu-id="084cb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="084cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="084cb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="084cb-124">Accept</span></span>|<span data-ttu-id="084cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="084cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="084cb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="084cb-126">Request body</span></span>
<span data-ttu-id="084cb-127">В теле запроса добавьте представление объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="084cb-127">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="084cb-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="084cb-128">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="084cb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="084cb-129">Property</span></span>|<span data-ttu-id="084cb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="084cb-130">Type</span></span>|<span data-ttu-id="084cb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="084cb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="084cb-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="084cb-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="084cb-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="084cb-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="084cb-134">Идентификатор приложения с типом его операционной системы.</span><span class="sxs-lookup"><span data-stu-id="084cb-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="084cb-135">id</span><span class="sxs-lookup"><span data-stu-id="084cb-135">id</span></span>|<span data-ttu-id="084cb-136">String</span><span class="sxs-lookup"><span data-stu-id="084cb-136">String</span></span>|<span data-ttu-id="084cb-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="084cb-137">Key of the entity.</span></span>|
|<span data-ttu-id="084cb-138">version</span><span class="sxs-lookup"><span data-stu-id="084cb-138">version</span></span>|<span data-ttu-id="084cb-139">String</span><span class="sxs-lookup"><span data-stu-id="084cb-139">String</span></span>|<span data-ttu-id="084cb-140">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="084cb-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="084cb-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="084cb-141">Response</span></span>
<span data-ttu-id="084cb-142">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="084cb-142">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="084cb-143">Пример</span><span class="sxs-lookup"><span data-stu-id="084cb-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="084cb-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="084cb-144">Request</span></span>
<span data-ttu-id="084cb-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="084cb-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
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

### <a name="response"></a><span data-ttu-id="084cb-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="084cb-146">Response</span></span>
<span data-ttu-id="084cb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="084cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




