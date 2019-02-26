---
title: Перечисление объектов managedDeviceMobileAppConfiguration
description: Перечисление свойств и связей объектов managedDeviceMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1f9a8a1cde5912635ee3dcd2ec9b2dd78605767
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259803"
---
# <a name="list-manageddevicemobileappconfigurations"></a><span data-ttu-id="acf06-103">Перечисление объектов managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="acf06-103">List managedDeviceMobileAppConfigurations</span></span>

> <span data-ttu-id="acf06-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="acf06-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acf06-105">Перечисление свойств и связей объектов [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="acf06-105">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="acf06-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="acf06-106">Prerequisites</span></span>
<span data-ttu-id="acf06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="acf06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="acf06-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="acf06-109">Permission type</span></span>|<span data-ttu-id="acf06-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="acf06-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acf06-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="acf06-111">Delegated (work or school account)</span></span>|<span data-ttu-id="acf06-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="acf06-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="acf06-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="acf06-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acf06-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acf06-114">Not supported.</span></span>|
|<span data-ttu-id="acf06-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="acf06-115">Application</span></span>|<span data-ttu-id="acf06-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acf06-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acf06-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="acf06-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="acf06-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="acf06-118">Request headers</span></span>
|<span data-ttu-id="acf06-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="acf06-119">Header</span></span>|<span data-ttu-id="acf06-120">Значение</span><span class="sxs-lookup"><span data-stu-id="acf06-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acf06-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="acf06-121">Authorization</span></span>|<span data-ttu-id="acf06-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="acf06-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acf06-123">Accept</span><span class="sxs-lookup"><span data-stu-id="acf06-123">Accept</span></span>|<span data-ttu-id="acf06-124">application/json</span><span class="sxs-lookup"><span data-stu-id="acf06-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acf06-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="acf06-125">Request body</span></span>
<span data-ttu-id="acf06-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="acf06-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acf06-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="acf06-127">Response</span></span>
<span data-ttu-id="acf06-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="acf06-128">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acf06-129">Пример</span><span class="sxs-lookup"><span data-stu-id="acf06-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="acf06-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="acf06-130">Request</span></span>
<span data-ttu-id="acf06-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="acf06-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="acf06-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="acf06-132">Response</span></span>
<span data-ttu-id="acf06-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="acf06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 485

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
      "id": "c60e7591-7591-c60e-9175-0ec691750ec6",
      "targetedMobileApps": [
        "Targeted Mobile Apps value"
      ],
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```



