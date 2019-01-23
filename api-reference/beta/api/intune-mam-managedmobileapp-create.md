---
title: Создание объекта managedMobileApp
description: Создание объекта managedMobileApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 546110d3e25c7b5b683f9104997fdbc497e78f9c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404703"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="ff560-103">Создание объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="ff560-103">Create managedMobileApp</span></span>

> <span data-ttu-id="ff560-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ff560-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ff560-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff560-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff560-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff560-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff560-107">Создание объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff560-107">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff560-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ff560-108">Prerequisites</span></span>
<span data-ttu-id="ff560-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ff560-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ff560-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff560-111">Permission type</span></span>|<span data-ttu-id="ff560-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff560-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff560-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff560-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff560-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff560-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ff560-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff560-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff560-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff560-116">Not supported.</span></span>|
|<span data-ttu-id="ff560-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff560-117">Application</span></span>|<span data-ttu-id="ff560-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff560-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff560-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff560-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="ff560-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff560-120">Request headers</span></span>
|<span data-ttu-id="ff560-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff560-121">Header</span></span>|<span data-ttu-id="ff560-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ff560-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff560-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff560-123">Authorization</span></span>|<span data-ttu-id="ff560-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ff560-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff560-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ff560-125">Accept</span></span>|<span data-ttu-id="ff560-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff560-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff560-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ff560-127">Request body</span></span>
<span data-ttu-id="ff560-128">В теле запроса добавьте представление объекта managedMobileApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff560-128">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="ff560-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="ff560-129">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="ff560-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff560-130">Property</span></span>|<span data-ttu-id="ff560-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ff560-131">Type</span></span>|<span data-ttu-id="ff560-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ff560-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff560-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ff560-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="ff560-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ff560-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="ff560-135">Идентификатор приложения с типом его операционной системы.</span><span class="sxs-lookup"><span data-stu-id="ff560-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="ff560-136">id</span><span class="sxs-lookup"><span data-stu-id="ff560-136">id</span></span>|<span data-ttu-id="ff560-137">String</span><span class="sxs-lookup"><span data-stu-id="ff560-137">String</span></span>|<span data-ttu-id="ff560-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ff560-138">Key of the entity.</span></span>|
|<span data-ttu-id="ff560-139">version</span><span class="sxs-lookup"><span data-stu-id="ff560-139">version</span></span>|<span data-ttu-id="ff560-140">String</span><span class="sxs-lookup"><span data-stu-id="ff560-140">String</span></span>|<span data-ttu-id="ff560-141">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="ff560-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="ff560-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff560-142">Response</span></span>
<span data-ttu-id="ff560-143">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ff560-143">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff560-144">Пример</span><span class="sxs-lookup"><span data-stu-id="ff560-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff560-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff560-145">Request</span></span>
<span data-ttu-id="ff560-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff560-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ff560-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff560-147">Response</span></span>
<span data-ttu-id="ff560-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ff560-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




