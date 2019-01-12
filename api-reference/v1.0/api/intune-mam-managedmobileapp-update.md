---
title: Обновление объекта managedMobileApp
description: Обновление свойств объекта managedMobileApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: efa34a090a52c54034e132e92e6ab853802bece3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941865"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="09aca-103">Обновление объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="09aca-103">Update managedMobileApp</span></span>

> <span data-ttu-id="09aca-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="09aca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09aca-105">Обновление свойств объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="09aca-105">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="09aca-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="09aca-106">Prerequisites</span></span>
<span data-ttu-id="09aca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09aca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09aca-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09aca-109">Permission type</span></span>|<span data-ttu-id="09aca-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="09aca-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09aca-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09aca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="09aca-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09aca-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="09aca-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09aca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09aca-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09aca-114">Not supported.</span></span>|
|<span data-ttu-id="09aca-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09aca-115">Application</span></span>|<span data-ttu-id="09aca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09aca-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09aca-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09aca-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="09aca-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09aca-118">Request headers</span></span>
|<span data-ttu-id="09aca-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09aca-119">Header</span></span>|<span data-ttu-id="09aca-120">Значение</span><span class="sxs-lookup"><span data-stu-id="09aca-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09aca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="09aca-121">Authorization</span></span>|<span data-ttu-id="09aca-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="09aca-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09aca-123">Accept</span><span class="sxs-lookup"><span data-stu-id="09aca-123">Accept</span></span>|<span data-ttu-id="09aca-124">application/json</span><span class="sxs-lookup"><span data-stu-id="09aca-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09aca-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="09aca-125">Request body</span></span>
<span data-ttu-id="09aca-126">В теле запроса добавьте представление объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09aca-126">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="09aca-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="09aca-127">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="09aca-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="09aca-128">Property</span></span>|<span data-ttu-id="09aca-129">Тип</span><span class="sxs-lookup"><span data-stu-id="09aca-129">Type</span></span>|<span data-ttu-id="09aca-130">Описание</span><span class="sxs-lookup"><span data-stu-id="09aca-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09aca-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="09aca-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="09aca-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="09aca-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="09aca-133">Идентификатор приложения с типом его операционной системы.</span><span class="sxs-lookup"><span data-stu-id="09aca-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="09aca-134">id</span><span class="sxs-lookup"><span data-stu-id="09aca-134">id</span></span>|<span data-ttu-id="09aca-135">Строка</span><span class="sxs-lookup"><span data-stu-id="09aca-135">String</span></span>|<span data-ttu-id="09aca-136">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="09aca-136">Key of the entity.</span></span>|
|<span data-ttu-id="09aca-137">version</span><span class="sxs-lookup"><span data-stu-id="09aca-137">version</span></span>|<span data-ttu-id="09aca-138">Строка</span><span class="sxs-lookup"><span data-stu-id="09aca-138">String</span></span>|<span data-ttu-id="09aca-139">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="09aca-139">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="09aca-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="09aca-140">Response</span></span>
<span data-ttu-id="09aca-141">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="09aca-141">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09aca-142">Пример</span><span class="sxs-lookup"><span data-stu-id="09aca-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="09aca-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="09aca-143">Request</span></span>
<span data-ttu-id="09aca-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09aca-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="09aca-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="09aca-145">Response</span></span>
<span data-ttu-id="09aca-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="09aca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



