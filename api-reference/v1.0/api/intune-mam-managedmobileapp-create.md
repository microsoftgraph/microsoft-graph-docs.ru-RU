---
title: Создание объекта managedMobileApp
description: Создание объекта managedMobileApp.
ms.openlocfilehash: 56eabc98d51e2717406b2aa4993e21b26aecd47d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025728"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="93e81-103">Создание объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="93e81-103">Create managedMobileApp</span></span>

> <span data-ttu-id="93e81-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="93e81-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93e81-105">Создание объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93e81-105">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="93e81-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="93e81-106">Prerequisites</span></span>
<span data-ttu-id="93e81-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93e81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93e81-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93e81-109">Permission type</span></span>|<span data-ttu-id="93e81-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="93e81-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93e81-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93e81-111">Delegated (work or school account)</span></span>|<span data-ttu-id="93e81-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93e81-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="93e81-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93e81-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93e81-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93e81-114">Not supported.</span></span>|
|<span data-ttu-id="93e81-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93e81-115">Application</span></span>|<span data-ttu-id="93e81-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93e81-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93e81-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93e81-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="93e81-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93e81-118">Request headers</span></span>
|<span data-ttu-id="93e81-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93e81-119">Header</span></span>|<span data-ttu-id="93e81-120">Значение</span><span class="sxs-lookup"><span data-stu-id="93e81-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93e81-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="93e81-121">Authorization</span></span>|<span data-ttu-id="93e81-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="93e81-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93e81-123">Accept</span><span class="sxs-lookup"><span data-stu-id="93e81-123">Accept</span></span>|<span data-ttu-id="93e81-124">application/json</span><span class="sxs-lookup"><span data-stu-id="93e81-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93e81-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="93e81-125">Request body</span></span>
<span data-ttu-id="93e81-126">В теле запроса добавьте представление объекта managedMobileApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93e81-126">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="93e81-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="93e81-127">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="93e81-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="93e81-128">Property</span></span>|<span data-ttu-id="93e81-129">Тип</span><span class="sxs-lookup"><span data-stu-id="93e81-129">Type</span></span>|<span data-ttu-id="93e81-130">Описание</span><span class="sxs-lookup"><span data-stu-id="93e81-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93e81-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="93e81-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="93e81-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="93e81-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="93e81-133">Идентификатор приложения с типом его операционной системы.</span><span class="sxs-lookup"><span data-stu-id="93e81-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="93e81-134">id</span><span class="sxs-lookup"><span data-stu-id="93e81-134">id</span></span>|<span data-ttu-id="93e81-135">String</span><span class="sxs-lookup"><span data-stu-id="93e81-135">String</span></span>|<span data-ttu-id="93e81-136">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="93e81-136">Key of the entity.</span></span>|
|<span data-ttu-id="93e81-137">version</span><span class="sxs-lookup"><span data-stu-id="93e81-137">version</span></span>|<span data-ttu-id="93e81-138">String</span><span class="sxs-lookup"><span data-stu-id="93e81-138">String</span></span>|<span data-ttu-id="93e81-139">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="93e81-139">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="93e81-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="93e81-140">Response</span></span>
<span data-ttu-id="93e81-141">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="93e81-141">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93e81-142">Пример</span><span class="sxs-lookup"><span data-stu-id="93e81-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="93e81-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="93e81-143">Request</span></span>
<span data-ttu-id="93e81-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93e81-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="93e81-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="93e81-145">Response</span></span>
<span data-ttu-id="93e81-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="93e81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



