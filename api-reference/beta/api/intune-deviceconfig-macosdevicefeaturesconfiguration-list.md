---
title: Перечисление объектов macOSDeviceFeaturesConfiguration
description: Список свойств и связей объектов macOSDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d30d6b460c3cdc55677dba85737917e4bec697a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891093"
---
# <a name="list-macosdevicefeaturesconfigurations"></a><span data-ttu-id="8b844-103">Перечисление объектов macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b844-103">List macOSDeviceFeaturesConfigurations</span></span>

> <span data-ttu-id="8b844-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8b844-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b844-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b844-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b844-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8b844-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b844-107">Список свойств и связей объектов [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8b844-107">List properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8b844-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8b844-108">Prerequisites</span></span>
<span data-ttu-id="8b844-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b844-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b844-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b844-111">Permission type</span></span>|<span data-ttu-id="8b844-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b844-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b844-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b844-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8b844-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b844-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8b844-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b844-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b844-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b844-116">Not supported.</span></span>|
|<span data-ttu-id="8b844-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b844-117">Application</span></span>|<span data-ttu-id="8b844-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b844-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b844-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b844-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8b844-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b844-120">Request headers</span></span>
|<span data-ttu-id="8b844-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b844-121">Header</span></span>|<span data-ttu-id="8b844-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8b844-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b844-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b844-123">Authorization</span></span>|<span data-ttu-id="8b844-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8b844-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b844-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8b844-125">Accept</span></span>|<span data-ttu-id="8b844-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8b844-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b844-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8b844-127">Request body</span></span>
<span data-ttu-id="8b844-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b844-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b844-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b844-129">Response</span></span>
<span data-ttu-id="8b844-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b844-130">If successful, this method returns a `200 OK` response code and a collection of [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b844-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8b844-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8b844-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b844-132">Request</span></span>
<span data-ttu-id="8b844-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b844-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="8b844-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b844-134">Response</span></span>
<span data-ttu-id="8b844-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8b844-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 785

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
      "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "airPrintDestinations": [
        {
          "@odata.type": "microsoft.graph.airPrintDestination",
          "ipAddress": "Ip Address value",
          "resourcePath": "Resource Path value",
          "port": 4,
          "forceTls": true
        }
      ]
    }
  ]
}
```





