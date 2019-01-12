---
title: Получение объекта managedMobileApp
description: Чтение свойств и связей объекта managedMobileApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 102f282f1fdc61ea1640356fb41a5a7c45ace625
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985993"
---
# <a name="get-managedmobileapp"></a><span data-ttu-id="5099c-103">Получение объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="5099c-103">Get managedMobileApp</span></span>

> <span data-ttu-id="5099c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5099c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5099c-105">Чтение свойств и связей объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5099c-105">Read properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5099c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5099c-106">Prerequisites</span></span>
<span data-ttu-id="5099c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5099c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5099c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5099c-109">Permission type</span></span>|<span data-ttu-id="5099c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5099c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5099c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5099c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5099c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5099c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5099c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5099c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5099c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5099c-114">Not supported.</span></span>|
|<span data-ttu-id="5099c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5099c-115">Application</span></span>|<span data-ttu-id="5099c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5099c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5099c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5099c-117">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="5099c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5099c-118">Optional query parameters</span></span>
<span data-ttu-id="5099c-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5099c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5099c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5099c-120">Request headers</span></span>
|<span data-ttu-id="5099c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5099c-121">Header</span></span>|<span data-ttu-id="5099c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5099c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5099c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5099c-123">Authorization</span></span>|<span data-ttu-id="5099c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5099c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5099c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5099c-125">Accept</span></span>|<span data-ttu-id="5099c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5099c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5099c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5099c-127">Request body</span></span>
<span data-ttu-id="5099c-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5099c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5099c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5099c-129">Response</span></span>
<span data-ttu-id="5099c-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5099c-130">If successful, this method returns a `200 OK` response code and [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5099c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5099c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="5099c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5099c-132">Request</span></span>
<span data-ttu-id="5099c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5099c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
```

### <a name="response"></a><span data-ttu-id="5099c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5099c-134">Response</span></span>
<span data-ttu-id="5099c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5099c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



