---
title: Список Виндовсинформатионпротектиондевицерегистратионс
description: Список свойств и связей объектов Виндовсинформатионпротектиондевицерегистратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1732249e765b308fdbbcba2e2f3c1353c58a60f4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167286"
---
# <a name="list-windowsinformationprotectiondeviceregistrations"></a><span data-ttu-id="e72f4-103">Список Виндовсинформатионпротектиондевицерегистратионс</span><span class="sxs-lookup"><span data-stu-id="e72f4-103">List windowsInformationProtectionDeviceRegistrations</span></span>

> <span data-ttu-id="e72f4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e72f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e72f4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e72f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e72f4-106">Список свойств и связей объектов [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .</span><span class="sxs-lookup"><span data-stu-id="e72f4-106">List properties and relationships of the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e72f4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e72f4-107">Prerequisites</span></span>
<span data-ttu-id="e72f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e72f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e72f4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e72f4-110">Permission type</span></span>|<span data-ttu-id="e72f4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e72f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e72f4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e72f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e72f4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e72f4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e72f4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e72f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e72f4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e72f4-115">Not supported.</span></span>|
|<span data-ttu-id="e72f4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e72f4-116">Application</span></span>|<span data-ttu-id="e72f4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e72f4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e72f4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e72f4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="e72f4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e72f4-119">Request headers</span></span>
|<span data-ttu-id="e72f4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e72f4-120">Header</span></span>|<span data-ttu-id="e72f4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e72f4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e72f4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e72f4-122">Authorization</span></span>|<span data-ttu-id="e72f4-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e72f4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e72f4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e72f4-124">Accept</span></span>|<span data-ttu-id="e72f4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e72f4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e72f4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e72f4-126">Request body</span></span>
<span data-ttu-id="e72f4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e72f4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e72f4-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="e72f4-128">Response</span></span>
<span data-ttu-id="e72f4-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e72f4-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e72f4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e72f4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e72f4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e72f4-131">Request</span></span>
<span data-ttu-id="e72f4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e72f4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

### <a name="response"></a><span data-ttu-id="e72f4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e72f4-133">Response</span></span>
<span data-ttu-id="e72f4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e72f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 480

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
      "id": "dd72e2c8-e2c8-dd72-c8e2-72ddc8e272dd",
      "userId": "User Id value",
      "deviceRegistrationId": "Device Registration Id value",
      "deviceName": "Device Name value",
      "deviceType": "Device Type value",
      "deviceMacAddress": "Device Mac Address value",
      "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
    }
  ]
}
```




