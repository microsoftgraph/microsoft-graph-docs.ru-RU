---
title: Обновление объекта managedMobileApp
description: Обновление свойств объекта managedMobileApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9e7d5afbbb290b2a1057a0f6ece52c4912a1bb49
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020635"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="1a16c-103">Обновление объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="1a16c-103">Update managedMobileApp</span></span>

> <span data-ttu-id="1a16c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a16c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a16c-105">Обновление свойств объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a16c-105">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a16c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1a16c-106">Prerequisites</span></span>
<span data-ttu-id="1a16c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a16c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a16c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a16c-109">Permission type</span></span>|<span data-ttu-id="1a16c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a16c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a16c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a16c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1a16c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a16c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1a16c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a16c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a16c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a16c-114">Not supported.</span></span>|
|<span data-ttu-id="1a16c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a16c-115">Application</span></span>|<span data-ttu-id="1a16c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a16c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a16c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a16c-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="1a16c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a16c-118">Request headers</span></span>
|<span data-ttu-id="1a16c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a16c-119">Header</span></span>|<span data-ttu-id="1a16c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1a16c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a16c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a16c-121">Authorization</span></span>|<span data-ttu-id="1a16c-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a16c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a16c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1a16c-123">Accept</span></span>|<span data-ttu-id="1a16c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1a16c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a16c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1a16c-125">Request body</span></span>
<span data-ttu-id="1a16c-126">В теле запроса добавьте представление объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a16c-126">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="1a16c-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a16c-127">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="1a16c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a16c-128">Property</span></span>|<span data-ttu-id="1a16c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1a16c-129">Type</span></span>|<span data-ttu-id="1a16c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1a16c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a16c-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="1a16c-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="1a16c-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="1a16c-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="1a16c-133">Идентификатор приложения с типом его операционной системы.</span><span class="sxs-lookup"><span data-stu-id="1a16c-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="1a16c-134">id</span><span class="sxs-lookup"><span data-stu-id="1a16c-134">id</span></span>|<span data-ttu-id="1a16c-135">String</span><span class="sxs-lookup"><span data-stu-id="1a16c-135">String</span></span>|<span data-ttu-id="1a16c-136">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1a16c-136">Key of the entity.</span></span>|
|<span data-ttu-id="1a16c-137">version</span><span class="sxs-lookup"><span data-stu-id="1a16c-137">version</span></span>|<span data-ttu-id="1a16c-138">String</span><span class="sxs-lookup"><span data-stu-id="1a16c-138">String</span></span>|<span data-ttu-id="1a16c-139">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="1a16c-139">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="1a16c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a16c-140">Response</span></span>
<span data-ttu-id="1a16c-141">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1a16c-141">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a16c-142">Пример</span><span class="sxs-lookup"><span data-stu-id="1a16c-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a16c-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a16c-143">Request</span></span>
<span data-ttu-id="1a16c-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a16c-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
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

### <a name="response"></a><span data-ttu-id="1a16c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a16c-145">Response</span></span>
<span data-ttu-id="1a16c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a16c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



