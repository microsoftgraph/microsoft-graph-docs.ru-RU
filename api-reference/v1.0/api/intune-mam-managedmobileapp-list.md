---
title: Перечисление объектов managedMobileApp
description: Список свойств и связей объектов managedMobileApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ccca3430d678e0c5263d4f76cc1dcf05900a1c2b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259173"
---
# <a name="list-managedmobileapps"></a><span data-ttu-id="bfe74-103">Перечисление объектов managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="bfe74-103">List managedMobileApps</span></span>

> <span data-ttu-id="bfe74-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bfe74-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfe74-105">Список свойств и связей объектов [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfe74-105">List properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bfe74-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bfe74-106">Prerequisites</span></span>
<span data-ttu-id="bfe74-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bfe74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bfe74-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfe74-109">Permission type</span></span>|<span data-ttu-id="bfe74-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfe74-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfe74-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfe74-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bfe74-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bfe74-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bfe74-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfe74-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfe74-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfe74-114">Not supported.</span></span>|
|<span data-ttu-id="bfe74-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bfe74-115">Application</span></span>|<span data-ttu-id="bfe74-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfe74-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfe74-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfe74-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="bfe74-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bfe74-118">Request headers</span></span>
|<span data-ttu-id="bfe74-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bfe74-119">Header</span></span>|<span data-ttu-id="bfe74-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bfe74-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfe74-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfe74-121">Authorization</span></span>|<span data-ttu-id="bfe74-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bfe74-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfe74-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bfe74-123">Accept</span></span>|<span data-ttu-id="bfe74-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bfe74-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfe74-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bfe74-125">Request body</span></span>
<span data-ttu-id="bfe74-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bfe74-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfe74-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfe74-127">Response</span></span>
<span data-ttu-id="bfe74-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bfe74-128">If successful, this method returns a `200 OK` response code and a collection of [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfe74-129">Пример</span><span class="sxs-lookup"><span data-stu-id="bfe74-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="bfe74-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfe74-130">Request</span></span>
<span data-ttu-id="bfe74-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfe74-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
```

### <a name="response"></a><span data-ttu-id="bfe74-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="bfe74-132">Response</span></span>
<span data-ttu-id="bfe74-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bfe74-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



