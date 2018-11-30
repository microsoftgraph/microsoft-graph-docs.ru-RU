---
title: Перечисление объектов managedMobileApp
description: Список свойств и связей объектов managedMobileApp.
ms.openlocfilehash: 7f0c9fce4ee4feeab3a78615c9f87db5b4d5775e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025836"
---
# <a name="list-managedmobileapps"></a><span data-ttu-id="947ef-103">Перечисление объектов managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="947ef-103">List managedMobileApps</span></span>

> <span data-ttu-id="947ef-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="947ef-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="947ef-105">Список свойств и связей объектов [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="947ef-105">List properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="947ef-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="947ef-106">Prerequisites</span></span>
<span data-ttu-id="947ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="947ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="947ef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="947ef-109">Permission type</span></span>|<span data-ttu-id="947ef-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="947ef-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="947ef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="947ef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="947ef-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="947ef-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="947ef-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="947ef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="947ef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="947ef-114">Not supported.</span></span>|
|<span data-ttu-id="947ef-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="947ef-115">Application</span></span>|<span data-ttu-id="947ef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="947ef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="947ef-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="947ef-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps
```

## <a name="request-headers"></a><span data-ttu-id="947ef-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="947ef-118">Request headers</span></span>
|<span data-ttu-id="947ef-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="947ef-119">Header</span></span>|<span data-ttu-id="947ef-120">Значение</span><span class="sxs-lookup"><span data-stu-id="947ef-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="947ef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="947ef-121">Authorization</span></span>|<span data-ttu-id="947ef-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="947ef-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="947ef-123">Accept</span><span class="sxs-lookup"><span data-stu-id="947ef-123">Accept</span></span>|<span data-ttu-id="947ef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="947ef-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="947ef-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="947ef-125">Request body</span></span>
<span data-ttu-id="947ef-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="947ef-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="947ef-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="947ef-127">Response</span></span>
<span data-ttu-id="947ef-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="947ef-128">If successful, this method returns a `200 OK` response code and a collection of [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="947ef-129">Пример</span><span class="sxs-lookup"><span data-stu-id="947ef-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="947ef-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="947ef-130">Request</span></span>
<span data-ttu-id="947ef-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="947ef-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
```

### <a name="response"></a><span data-ttu-id="947ef-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="947ef-132">Response</span></span>
<span data-ttu-id="947ef-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="947ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```



