---
title: Перечисление объектов managedDeviceMobileAppConfiguration
description: Перечисление свойств и связей объектов managedDeviceMobileAppConfiguration.
author: tfitzmac
ms.openlocfilehash: e82c250fb0fb3406d5bb97be4a6cb1711a789adf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358991"
---
# <a name="list-manageddevicemobileappconfigurations"></a><span data-ttu-id="16c05-103">Перечисление объектов managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="16c05-103">List managedDeviceMobileAppConfigurations</span></span>

> <span data-ttu-id="16c05-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="16c05-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16c05-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16c05-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16c05-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="16c05-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16c05-107">Перечисление свойств и связей объектов [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16c05-107">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16c05-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="16c05-108">Prerequisites</span></span>
<span data-ttu-id="16c05-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16c05-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16c05-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16c05-111">Permission type</span></span>|<span data-ttu-id="16c05-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16c05-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16c05-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16c05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16c05-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="16c05-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="16c05-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16c05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16c05-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16c05-116">Not supported.</span></span>|
|<span data-ttu-id="16c05-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16c05-117">Application</span></span>|<span data-ttu-id="16c05-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16c05-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16c05-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16c05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="16c05-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16c05-120">Request headers</span></span>
|<span data-ttu-id="16c05-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16c05-121">Header</span></span>|<span data-ttu-id="16c05-122">Значение</span><span class="sxs-lookup"><span data-stu-id="16c05-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16c05-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16c05-123">Authorization</span></span>|<span data-ttu-id="16c05-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="16c05-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16c05-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16c05-125">Accept</span></span>|<span data-ttu-id="16c05-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16c05-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16c05-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16c05-127">Request body</span></span>
<span data-ttu-id="16c05-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16c05-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16c05-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="16c05-129">Response</span></span>
<span data-ttu-id="16c05-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16c05-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16c05-131">Пример</span><span class="sxs-lookup"><span data-stu-id="16c05-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="16c05-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="16c05-132">Request</span></span>
<span data-ttu-id="16c05-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16c05-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="16c05-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="16c05-134">Response</span></span>
<span data-ttu-id="16c05-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="16c05-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 559

{
  "value": [
    {
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
  ]
}
```





