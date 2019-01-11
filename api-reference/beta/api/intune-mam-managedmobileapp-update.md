---
title: Обновление объекта managedMobileApp
description: Обновление свойств объекта managedMobileApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cf1a5d756f46e3986b8131b7726860edb6931ed1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859516"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="fd64c-103">Обновление объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="fd64c-103">Update managedMobileApp</span></span>

> <span data-ttu-id="fd64c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fd64c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd64c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd64c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd64c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fd64c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd64c-107">Обновление свойств объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fd64c-107">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd64c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fd64c-108">Prerequisites</span></span>
<span data-ttu-id="fd64c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd64c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd64c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd64c-111">Permission type</span></span>|<span data-ttu-id="fd64c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd64c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd64c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd64c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fd64c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd64c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fd64c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd64c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd64c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd64c-116">Not supported.</span></span>|
|<span data-ttu-id="fd64c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd64c-117">Application</span></span>|<span data-ttu-id="fd64c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd64c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd64c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd64c-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="fd64c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd64c-120">Request headers</span></span>
|<span data-ttu-id="fd64c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd64c-121">Header</span></span>|<span data-ttu-id="fd64c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fd64c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd64c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd64c-123">Authorization</span></span>|<span data-ttu-id="fd64c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fd64c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd64c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fd64c-125">Accept</span></span>|<span data-ttu-id="fd64c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fd64c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd64c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fd64c-127">Request body</span></span>
<span data-ttu-id="fd64c-128">В теле запроса добавьте представление объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd64c-128">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="fd64c-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fd64c-129">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="fd64c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd64c-130">Property</span></span>|<span data-ttu-id="fd64c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fd64c-131">Type</span></span>|<span data-ttu-id="fd64c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fd64c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd64c-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fd64c-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="fd64c-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fd64c-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="fd64c-135">Идентификатор приложения с типом его операционной системы.</span><span class="sxs-lookup"><span data-stu-id="fd64c-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="fd64c-136">id</span><span class="sxs-lookup"><span data-stu-id="fd64c-136">id</span></span>|<span data-ttu-id="fd64c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="fd64c-137">String</span></span>|<span data-ttu-id="fd64c-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fd64c-138">Key of the entity.</span></span>|
|<span data-ttu-id="fd64c-139">version</span><span class="sxs-lookup"><span data-stu-id="fd64c-139">version</span></span>|<span data-ttu-id="fd64c-140">Строка</span><span class="sxs-lookup"><span data-stu-id="fd64c-140">String</span></span>|<span data-ttu-id="fd64c-141">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="fd64c-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="fd64c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd64c-142">Response</span></span>
<span data-ttu-id="fd64c-143">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fd64c-143">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd64c-144">Пример</span><span class="sxs-lookup"><span data-stu-id="fd64c-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd64c-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd64c-145">Request</span></span>
<span data-ttu-id="fd64c-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd64c-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 126

{
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="fd64c-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd64c-147">Response</span></span>
<span data-ttu-id="fd64c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fd64c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





