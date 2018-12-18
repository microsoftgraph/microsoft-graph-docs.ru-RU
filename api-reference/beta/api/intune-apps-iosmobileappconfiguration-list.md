---
title: Список iosMobileAppConfigurations
description: Список свойств и связей объектов iosUpdateConfiguration.
author: tfitzmac
ms.openlocfilehash: 3d56946ec2183cd486e9b1ffcebb2979590dfe82
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313988"
---
# <a name="list-iosmobileappconfigurations"></a><span data-ttu-id="e2f11-103">Список iosMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="e2f11-103">List iosMobileAppConfigurations</span></span>

> <span data-ttu-id="e2f11-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e2f11-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2f11-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2f11-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2f11-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e2f11-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2f11-107">Список свойств и связей объектов [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2f11-107">List properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e2f11-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e2f11-108">Prerequisites</span></span>
<span data-ttu-id="e2f11-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2f11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2f11-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2f11-111">Permission type</span></span>|<span data-ttu-id="e2f11-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2f11-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2f11-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2f11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2f11-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2f11-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e2f11-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2f11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2f11-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2f11-116">Not supported.</span></span>|
|<span data-ttu-id="e2f11-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2f11-117">Application</span></span>|<span data-ttu-id="e2f11-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2f11-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2f11-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2f11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e2f11-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2f11-120">Request headers</span></span>
|<span data-ttu-id="e2f11-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2f11-121">Header</span></span>|<span data-ttu-id="e2f11-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e2f11-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2f11-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2f11-123">Authorization</span></span>|<span data-ttu-id="e2f11-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e2f11-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2f11-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e2f11-125">Accept</span></span>|<span data-ttu-id="e2f11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2f11-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2f11-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2f11-127">Request body</span></span>
<span data-ttu-id="e2f11-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2f11-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2f11-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2f11-129">Response</span></span>
<span data-ttu-id="e2f11-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e2f11-130">If successful, this method returns a `200 OK` response code and a collection of [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2f11-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e2f11-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e2f11-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2f11-132">Request</span></span>
<span data-ttu-id="e2f11-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2f11-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="e2f11-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2f11-134">Response</span></span>
<span data-ttu-id="e2f11-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e2f11-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 889

{
  "value": [
    {
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
  ]
}
```





