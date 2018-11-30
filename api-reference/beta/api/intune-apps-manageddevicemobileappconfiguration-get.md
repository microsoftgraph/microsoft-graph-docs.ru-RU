---
title: Получение объекта managedDeviceMobileAppConfiguration
description: Чтение свойств и связей объекта managedDeviceMobileAppConfiguration.
ms.openlocfilehash: 3eea7d30e6a8a1518e5a23f1d1618f6ea377b323
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075619"
---
# <a name="get-manageddevicemobileappconfiguration"></a><span data-ttu-id="fc078-103">Получение объекта managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="fc078-103">Get managedDeviceMobileAppConfiguration</span></span>

> <span data-ttu-id="fc078-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fc078-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc078-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc078-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc078-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fc078-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc078-107">Чтение свойств и связей объекта [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc078-107">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fc078-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fc078-108">Prerequisites</span></span>
<span data-ttu-id="fc078-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc078-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc078-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc078-111">Permission type</span></span>|<span data-ttu-id="fc078-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc078-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc078-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc078-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc078-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc078-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fc078-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc078-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc078-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc078-116">Not supported.</span></span>|
|<span data-ttu-id="fc078-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc078-117">Application</span></span>|<span data-ttu-id="fc078-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc078-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc078-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc078-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc078-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fc078-120">Optional query parameters</span></span>
<span data-ttu-id="fc078-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fc078-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fc078-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc078-122">Request headers</span></span>
|<span data-ttu-id="fc078-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc078-123">Header</span></span>|<span data-ttu-id="fc078-124">Значение</span><span class="sxs-lookup"><span data-stu-id="fc078-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc078-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc078-125">Authorization</span></span>|<span data-ttu-id="fc078-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fc078-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc078-127">Accept</span><span class="sxs-lookup"><span data-stu-id="fc078-127">Accept</span></span>|<span data-ttu-id="fc078-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fc078-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc078-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc078-129">Request body</span></span>
<span data-ttu-id="fc078-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fc078-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc078-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc078-131">Response</span></span>
<span data-ttu-id="fc078-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc078-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc078-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fc078-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="fc078-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc078-134">Request</span></span>
<span data-ttu-id="fc078-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc078-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="fc078-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc078-136">Response</span></span>
<span data-ttu-id="fc078-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="fc078-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 519

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
    "id": "c60e7591-7591-c60e-9175-0ec691750ec6",
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
    "version": 7
  }
}
```





