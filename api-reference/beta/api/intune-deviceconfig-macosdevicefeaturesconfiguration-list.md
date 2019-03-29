---
title: Перечисление объектов macOSDeviceFeaturesConfiguration
description: Список свойств и связей объектов macOSDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60effb48c82efd7fb37237550a350c9a3c8587bd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957502"
---
# <a name="list-macosdevicefeaturesconfigurations"></a><span data-ttu-id="43286-103">Перечисление объектов macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="43286-103">List macOSDeviceFeaturesConfigurations</span></span>

> <span data-ttu-id="43286-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43286-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43286-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43286-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43286-106">Список свойств и связей объектов [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="43286-106">List properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43286-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="43286-107">Prerequisites</span></span>
<span data-ttu-id="43286-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43286-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43286-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43286-110">Permission type</span></span>|<span data-ttu-id="43286-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43286-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43286-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43286-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43286-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="43286-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="43286-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43286-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43286-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43286-115">Not supported.</span></span>|
|<span data-ttu-id="43286-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43286-116">Application</span></span>|<span data-ttu-id="43286-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43286-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43286-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43286-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="43286-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43286-119">Request headers</span></span>
|<span data-ttu-id="43286-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43286-120">Header</span></span>|<span data-ttu-id="43286-121">Значение</span><span class="sxs-lookup"><span data-stu-id="43286-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43286-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43286-122">Authorization</span></span>|<span data-ttu-id="43286-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43286-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43286-124">Accept</span><span class="sxs-lookup"><span data-stu-id="43286-124">Accept</span></span>|<span data-ttu-id="43286-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43286-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43286-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43286-126">Request body</span></span>
<span data-ttu-id="43286-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43286-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43286-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="43286-128">Response</span></span>
<span data-ttu-id="43286-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="43286-129">If successful, this method returns a `200 OK` response code and a collection of [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43286-130">Пример</span><span class="sxs-lookup"><span data-stu-id="43286-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="43286-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="43286-131">Request</span></span>
<span data-ttu-id="43286-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43286-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="43286-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="43286-133">Response</span></span>
<span data-ttu-id="43286-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43286-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




