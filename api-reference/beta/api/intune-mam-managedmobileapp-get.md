---
title: Получение объекта managedMobileApp
description: Чтение свойств и связей объекта managedMobileApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e7fd60f64c5ac4385d20105f260342f820b8e478
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37192949"
---
# <a name="get-managedmobileapp"></a><span data-ttu-id="f7bcd-103">Получение объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="f7bcd-103">Get managedMobileApp</span></span>

> <span data-ttu-id="f7bcd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7bcd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7bcd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7bcd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7bcd-106">Чтение свойств и связей объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7bcd-106">Read properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7bcd-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f7bcd-107">Prerequisites</span></span>
<span data-ttu-id="f7bcd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7bcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7bcd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7bcd-110">Permission type</span></span>|<span data-ttu-id="f7bcd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7bcd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7bcd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7bcd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f7bcd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7bcd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f7bcd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7bcd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7bcd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7bcd-115">Not supported.</span></span>|
|<span data-ttu-id="f7bcd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7bcd-116">Application</span></span>|<span data-ttu-id="f7bcd-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7bcd-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7bcd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7bcd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7bcd-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f7bcd-119">Optional query parameters</span></span>
<span data-ttu-id="f7bcd-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f7bcd-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7bcd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7bcd-121">Request headers</span></span>
|<span data-ttu-id="f7bcd-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7bcd-122">Header</span></span>|<span data-ttu-id="f7bcd-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f7bcd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7bcd-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7bcd-124">Authorization</span></span>|<span data-ttu-id="f7bcd-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7bcd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7bcd-126">Accept</span><span class="sxs-lookup"><span data-stu-id="f7bcd-126">Accept</span></span>|<span data-ttu-id="f7bcd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f7bcd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7bcd-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f7bcd-128">Request body</span></span>
<span data-ttu-id="f7bcd-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7bcd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7bcd-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7bcd-130">Response</span></span>
<span data-ttu-id="f7bcd-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f7bcd-131">If successful, this method returns a `200 OK` response code and [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7bcd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f7bcd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7bcd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7bcd-133">Request</span></span>
<span data-ttu-id="f7bcd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7bcd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
```

### <a name="response"></a><span data-ttu-id="f7bcd-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7bcd-135">Response</span></span>
<span data-ttu-id="f7bcd-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7bcd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": {
    "@odata.type": "#microsoft.graph.managedMobileApp",
    "mobileAppIdentifier": {
      "@odata.type": "microsoft.graph.mobileAppIdentifier"
    },
    "id": "0a129715-9715-0a12-1597-120a1597120a",
    "version": "Version value"
  }
}
```




