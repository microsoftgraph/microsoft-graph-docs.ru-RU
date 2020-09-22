---
title: Перечисление объектов macOSGeneralDeviceConfiguration
description: Список свойств и связей объектов macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: afcd5de61dbebf648995499e76f9b5de2d551158
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028912"
---
# <a name="list-macosgeneraldeviceconfigurations"></a><span data-ttu-id="4e89a-103">Перечисление объектов macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="4e89a-103">List macOSGeneralDeviceConfigurations</span></span>

<span data-ttu-id="4e89a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e89a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e89a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e89a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e89a-106">Список свойств и связей объектов [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e89a-106">List properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e89a-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4e89a-107">Prerequisites</span></span>
<span data-ttu-id="4e89a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e89a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e89a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e89a-110">Permission type</span></span>|<span data-ttu-id="4e89a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e89a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e89a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e89a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e89a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e89a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4e89a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e89a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e89a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e89a-115">Not supported.</span></span>|
|<span data-ttu-id="4e89a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e89a-116">Application</span></span>|<span data-ttu-id="4e89a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e89a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e89a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e89a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4e89a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4e89a-119">Request headers</span></span>
|<span data-ttu-id="4e89a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e89a-120">Header</span></span>|<span data-ttu-id="4e89a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4e89a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e89a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e89a-122">Authorization</span></span>|<span data-ttu-id="4e89a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e89a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e89a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4e89a-124">Accept</span></span>|<span data-ttu-id="4e89a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e89a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e89a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e89a-126">Request body</span></span>
<span data-ttu-id="4e89a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e89a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e89a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e89a-128">Response</span></span>
<span data-ttu-id="4e89a-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e89a-129">If successful, this method returns a `200 OK` response code and a collection of [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e89a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4e89a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e89a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e89a-131">Request</span></span>
<span data-ttu-id="4e89a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e89a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="4e89a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e89a-133">Response</span></span>
<span data-ttu-id="4e89a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e89a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1227

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
      "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "compliantAppsList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "compliantAppListType": "appsInListCompliant",
      "emailInDomainSuffixes": [
        "Email In Domain Suffixes value"
      ],
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumCharacterSetCount": 0,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequiredType": "alphanumeric",
      "passwordRequired": true
    }
  ]
}
```









