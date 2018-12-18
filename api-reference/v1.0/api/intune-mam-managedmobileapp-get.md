---
title: Получение объекта managedMobileApp
description: Чтение свойств и связей объекта managedMobileApp.
author: tfitzmac
ms.openlocfilehash: d0e08f0c0381645012883ae18bd54e19bbb45963
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336969"
---
# <a name="get-managedmobileapp"></a><span data-ttu-id="6bff7-103">Получение объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="6bff7-103">Get managedMobileApp</span></span>

> <span data-ttu-id="6bff7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6bff7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bff7-105">Чтение свойств и связей объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6bff7-105">Read properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6bff7-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6bff7-106">Prerequisites</span></span>
<span data-ttu-id="6bff7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bff7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bff7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6bff7-109">Permission type</span></span>|<span data-ttu-id="6bff7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6bff7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bff7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6bff7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6bff7-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bff7-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6bff7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6bff7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bff7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bff7-114">Not supported.</span></span>|
|<span data-ttu-id="6bff7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6bff7-115">Application</span></span>|<span data-ttu-id="6bff7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bff7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bff7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6bff7-117">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="6bff7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6bff7-118">Optional query parameters</span></span>
<span data-ttu-id="6bff7-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6bff7-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6bff7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6bff7-120">Request headers</span></span>
|<span data-ttu-id="6bff7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6bff7-121">Header</span></span>|<span data-ttu-id="6bff7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6bff7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bff7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6bff7-123">Authorization</span></span>|<span data-ttu-id="6bff7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6bff7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bff7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6bff7-125">Accept</span></span>|<span data-ttu-id="6bff7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6bff7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bff7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6bff7-127">Request body</span></span>
<span data-ttu-id="6bff7-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6bff7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bff7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bff7-129">Response</span></span>
<span data-ttu-id="6bff7-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6bff7-130">If successful, this method returns a `200 OK` response code and [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bff7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6bff7-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6bff7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bff7-132">Request</span></span>
<span data-ttu-id="6bff7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6bff7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
```

### <a name="response"></a><span data-ttu-id="6bff7-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="6bff7-134">Response</span></span>
<span data-ttu-id="6bff7-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6bff7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



