---
title: Получить iosMobileAppConfiguration
description: Считывание свойств и связей объекта iosMobileAppConfiguration.
author: tfitzmac
ms.openlocfilehash: 4784930ca0d61d898af0801be2661148958c1bc7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313001"
---
# <a name="get-iosmobileappconfiguration"></a><span data-ttu-id="9f825-103">Получить iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9f825-103">Get iosMobileAppConfiguration</span></span>

> <span data-ttu-id="9f825-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9f825-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f825-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f825-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f825-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9f825-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f825-107">Чтение списка свойств и связей объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f825-107">Read properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f825-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="9f825-108">Prerequisites</span></span>
<span data-ttu-id="9f825-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f825-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f825-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f825-111">Permission type</span></span>|<span data-ttu-id="9f825-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f825-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f825-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f825-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f825-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f825-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9f825-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f825-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f825-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f825-116">Not supported.</span></span>|
|<span data-ttu-id="9f825-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f825-117">Application</span></span>|<span data-ttu-id="9f825-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f825-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f825-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f825-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f825-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9f825-120">Optional query parameters</span></span>
<span data-ttu-id="9f825-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9f825-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9f825-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f825-122">Request headers</span></span>
|<span data-ttu-id="9f825-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f825-123">Header</span></span>|<span data-ttu-id="9f825-124">Значение</span><span class="sxs-lookup"><span data-stu-id="9f825-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f825-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f825-125">Authorization</span></span>|<span data-ttu-id="9f825-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9f825-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f825-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9f825-127">Accept</span></span>|<span data-ttu-id="9f825-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9f825-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f825-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f825-129">Request body</span></span>
<span data-ttu-id="9f825-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f825-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f825-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f825-131">Response</span></span>
<span data-ttu-id="9f825-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f825-132">If successful, this method returns a `200 OK` response code and [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f825-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9f825-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f825-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f825-134">Request</span></span>
<span data-ttu-id="9f825-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f825-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9f825-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f825-136">Response</span></span>
<span data-ttu-id="9f825-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9f825-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 831

{
  "value": {
    "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
    "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
    "targetedMobileApps": [
      "Targeted Mobile Apps value"
    ],
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
    "settings": [
      {
        "@odata.type": "microsoft.graph.appConfigurationSettingItem",
        "appConfigKey": "App Config Key value",
        "appConfigKeyType": "integerType",
        "appConfigKeyValue": "App Config Key Value value"
      }
    ]
  }
}
```





