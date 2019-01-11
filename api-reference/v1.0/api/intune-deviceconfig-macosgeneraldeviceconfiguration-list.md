---
title: Перечисление объектов macOSGeneralDeviceConfiguration
description: Список свойств и связей объектов macOSGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6c11cc0f1fef43297fd585dc5c9e30ecd361d04e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855218"
---
# <a name="list-macosgeneraldeviceconfigurations"></a><span data-ttu-id="d78f7-103">Перечисление объектов macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d78f7-103">List macOSGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="d78f7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d78f7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d78f7-105">Список свойств и связей объектов [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d78f7-105">List properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d78f7-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d78f7-106">Prerequisites</span></span>
<span data-ttu-id="d78f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d78f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d78f7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d78f7-109">Permission type</span></span>|<span data-ttu-id="d78f7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d78f7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d78f7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d78f7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d78f7-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d78f7-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d78f7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d78f7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d78f7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d78f7-114">Not supported.</span></span>|
|<span data-ttu-id="d78f7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d78f7-115">Application</span></span>|<span data-ttu-id="d78f7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d78f7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d78f7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d78f7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d78f7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d78f7-118">Request headers</span></span>
|<span data-ttu-id="d78f7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d78f7-119">Header</span></span>|<span data-ttu-id="d78f7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d78f7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d78f7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d78f7-121">Authorization</span></span>|<span data-ttu-id="d78f7-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d78f7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d78f7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d78f7-123">Accept</span></span>|<span data-ttu-id="d78f7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d78f7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d78f7-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d78f7-125">Request body</span></span>
<span data-ttu-id="d78f7-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d78f7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d78f7-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d78f7-127">Response</span></span>
<span data-ttu-id="d78f7-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d78f7-128">If successful, this method returns a `200 OK` response code and a collection of [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d78f7-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d78f7-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d78f7-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d78f7-130">Request</span></span>
<span data-ttu-id="d78f7-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d78f7-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="d78f7-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="d78f7-132">Response</span></span>
<span data-ttu-id="d78f7-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d78f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



