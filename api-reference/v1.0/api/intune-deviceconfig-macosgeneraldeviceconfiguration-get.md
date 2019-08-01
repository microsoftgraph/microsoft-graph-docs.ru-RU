---
title: Get macOSGeneralDeviceConfiguration
description: Чтение свойств и связей объекта macOSGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f3dc909b3e4f2138d42d159d6ff8f2bb864c3799
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997416"
---
# <a name="get-macosgeneraldeviceconfiguration"></a><span data-ttu-id="3e1fa-103">Get macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e1fa-103">Get macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="3e1fa-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e1fa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e1fa-105">Чтение свойств и связей объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e1fa-105">Read properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e1fa-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3e1fa-106">Prerequisites</span></span>
<span data-ttu-id="3e1fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e1fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e1fa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e1fa-109">Permission type</span></span>|<span data-ttu-id="3e1fa-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e1fa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e1fa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e1fa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3e1fa-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e1fa-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3e1fa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e1fa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e1fa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e1fa-114">Not supported.</span></span>|
|<span data-ttu-id="3e1fa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e1fa-115">Application</span></span>|<span data-ttu-id="3e1fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e1fa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e1fa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e1fa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e1fa-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3e1fa-118">Optional query parameters</span></span>
<span data-ttu-id="3e1fa-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3e1fa-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e1fa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e1fa-120">Request headers</span></span>
|<span data-ttu-id="3e1fa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e1fa-121">Header</span></span>|<span data-ttu-id="3e1fa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3e1fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e1fa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e1fa-123">Authorization</span></span>|<span data-ttu-id="3e1fa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e1fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e1fa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3e1fa-125">Accept</span></span>|<span data-ttu-id="3e1fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e1fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e1fa-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3e1fa-127">Request body</span></span>
<span data-ttu-id="3e1fa-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3e1fa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e1fa-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e1fa-129">Response</span></span>
<span data-ttu-id="3e1fa-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3e1fa-130">If successful, this method returns a `200 OK` response code and [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e1fa-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3e1fa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e1fa-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e1fa-132">Request</span></span>
<span data-ttu-id="3e1fa-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e1fa-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="3e1fa-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e1fa-134">Response</span></span>
<span data-ttu-id="3e1fa-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e1fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1155

{
  "value": {
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
}
```



