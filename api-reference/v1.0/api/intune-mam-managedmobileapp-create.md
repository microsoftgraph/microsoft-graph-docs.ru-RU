---
title: Создание объекта managedMobileApp
description: Создание объекта managedMobileApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 17611c7eb3c4052892ec23ab49751db2bfd9b66c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513058"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="5996b-103">Создание объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="5996b-103">Create managedMobileApp</span></span>

<span data-ttu-id="5996b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5996b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5996b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5996b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5996b-106">Создание объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5996b-106">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5996b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5996b-107">Prerequisites</span></span>
<span data-ttu-id="5996b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5996b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5996b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5996b-110">Permission type</span></span>|<span data-ttu-id="5996b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5996b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5996b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5996b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5996b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5996b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5996b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5996b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5996b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5996b-115">Not supported.</span></span>|
|<span data-ttu-id="5996b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5996b-116">Application</span></span>|<span data-ttu-id="5996b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5996b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5996b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5996b-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5996b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5996b-119">Request headers</span></span>
|<span data-ttu-id="5996b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5996b-120">Header</span></span>|<span data-ttu-id="5996b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5996b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5996b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5996b-122">Authorization</span></span>|<span data-ttu-id="5996b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5996b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5996b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5996b-124">Accept</span></span>|<span data-ttu-id="5996b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5996b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5996b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5996b-126">Request body</span></span>
<span data-ttu-id="5996b-127">В теле запроса добавьте представление объекта managedMobileApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5996b-127">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="5996b-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="5996b-128">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="5996b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5996b-129">Property</span></span>|<span data-ttu-id="5996b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5996b-130">Type</span></span>|<span data-ttu-id="5996b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5996b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5996b-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5996b-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="5996b-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5996b-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="5996b-134">Идентификатор приложения с типом его операционной системы.</span><span class="sxs-lookup"><span data-stu-id="5996b-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="5996b-135">id</span><span class="sxs-lookup"><span data-stu-id="5996b-135">id</span></span>|<span data-ttu-id="5996b-136">Строка</span><span class="sxs-lookup"><span data-stu-id="5996b-136">String</span></span>|<span data-ttu-id="5996b-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5996b-137">Key of the entity.</span></span>|
|<span data-ttu-id="5996b-138">version</span><span class="sxs-lookup"><span data-stu-id="5996b-138">version</span></span>|<span data-ttu-id="5996b-139">String</span><span class="sxs-lookup"><span data-stu-id="5996b-139">String</span></span>|<span data-ttu-id="5996b-140">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="5996b-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="5996b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5996b-141">Response</span></span>
<span data-ttu-id="5996b-142">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5996b-142">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5996b-143">Пример</span><span class="sxs-lookup"><span data-stu-id="5996b-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="5996b-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="5996b-144">Request</span></span>
<span data-ttu-id="5996b-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5996b-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
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

### <a name="response"></a><span data-ttu-id="5996b-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="5996b-146">Response</span></span>
<span data-ttu-id="5996b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5996b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




