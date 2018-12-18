---
title: Get macOSGeneralDeviceConfiguration
description: Чтение свойств и связей объекта macOSGeneralDeviceConfiguration.
author: tfitzmac
ms.openlocfilehash: 6ed46c223529d0dde59750db0ed135b71c08482f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359117"
---
# <a name="get-macosgeneraldeviceconfiguration"></a><span data-ttu-id="20b67-103">Get macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="20b67-103">Get macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="20b67-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="20b67-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20b67-105">Чтение свойств и связей объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20b67-105">Read properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20b67-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="20b67-106">Prerequisites</span></span>
<span data-ttu-id="20b67-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20b67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20b67-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20b67-109">Permission type</span></span>|<span data-ttu-id="20b67-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20b67-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20b67-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20b67-111">Delegated (work or school account)</span></span>|<span data-ttu-id="20b67-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="20b67-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="20b67-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20b67-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20b67-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20b67-114">Not supported.</span></span>|
|<span data-ttu-id="20b67-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20b67-115">Application</span></span>|<span data-ttu-id="20b67-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20b67-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20b67-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20b67-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20b67-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="20b67-118">Optional query parameters</span></span>
<span data-ttu-id="20b67-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="20b67-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="20b67-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20b67-120">Request headers</span></span>
|<span data-ttu-id="20b67-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20b67-121">Header</span></span>|<span data-ttu-id="20b67-122">Значение</span><span class="sxs-lookup"><span data-stu-id="20b67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20b67-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20b67-123">Authorization</span></span>|<span data-ttu-id="20b67-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="20b67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20b67-125">Accept</span><span class="sxs-lookup"><span data-stu-id="20b67-125">Accept</span></span>|<span data-ttu-id="20b67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20b67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20b67-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20b67-127">Request body</span></span>
<span data-ttu-id="20b67-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="20b67-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20b67-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="20b67-129">Response</span></span>
<span data-ttu-id="20b67-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="20b67-130">If successful, this method returns a `200 OK` response code and [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20b67-131">Пример</span><span class="sxs-lookup"><span data-stu-id="20b67-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="20b67-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="20b67-132">Request</span></span>
<span data-ttu-id="20b67-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20b67-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="20b67-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="20b67-134">Response</span></span>
<span data-ttu-id="20b67-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="20b67-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



