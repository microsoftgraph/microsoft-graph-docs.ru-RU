---
title: Перечисление объектов macOSGeneralDeviceConfiguration
description: Список свойств и связей объектов macOSGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 014732195966dd44adea6e28b0d6e945b18cc0d8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971614"
---
# <a name="list-macosgeneraldeviceconfigurations"></a><span data-ttu-id="c120c-103">Перечисление объектов macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c120c-103">List macOSGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="c120c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c120c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c120c-105">Список свойств и связей объектов [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c120c-105">List properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c120c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c120c-106">Prerequisites</span></span>
<span data-ttu-id="c120c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c120c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c120c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c120c-109">Permission type</span></span>|<span data-ttu-id="c120c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c120c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c120c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c120c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c120c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c120c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c120c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c120c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c120c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c120c-114">Not supported.</span></span>|
|<span data-ttu-id="c120c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c120c-115">Application</span></span>|<span data-ttu-id="c120c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c120c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c120c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c120c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c120c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c120c-118">Request headers</span></span>
|<span data-ttu-id="c120c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c120c-119">Header</span></span>|<span data-ttu-id="c120c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c120c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c120c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c120c-121">Authorization</span></span>|<span data-ttu-id="c120c-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c120c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c120c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c120c-123">Accept</span></span>|<span data-ttu-id="c120c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c120c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c120c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c120c-125">Request body</span></span>
<span data-ttu-id="c120c-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c120c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c120c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c120c-127">Response</span></span>
<span data-ttu-id="c120c-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c120c-128">If successful, this method returns a `200 OK` response code and a collection of [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c120c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c120c-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c120c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c120c-130">Request</span></span>
<span data-ttu-id="c120c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c120c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="c120c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c120c-132">Response</span></span>
<span data-ttu-id="c120c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c120c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



