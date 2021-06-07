---
title: Получение windowsPhone81CustomConfiguration
description: Считывание свойств и связей объекта windowsPhone81CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6101cad3f6ba4ae68c667c1b44b9100e4e627d4e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756192"
---
# <a name="get-windowsphone81customconfiguration"></a><span data-ttu-id="7eed3-103">Получение windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="7eed3-103">Get windowsPhone81CustomConfiguration</span></span>

<span data-ttu-id="7eed3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7eed3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7eed3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7eed3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7eed3-106">Считывание свойств и связей объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7eed3-106">Read properties and relationships of the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7eed3-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7eed3-107">Prerequisites</span></span>
<span data-ttu-id="7eed3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7eed3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7eed3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7eed3-110">Permission type</span></span>|<span data-ttu-id="7eed3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7eed3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7eed3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7eed3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7eed3-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7eed3-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7eed3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7eed3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7eed3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7eed3-115">Not supported.</span></span>|
|<span data-ttu-id="7eed3-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7eed3-116">Application</span></span>|<span data-ttu-id="7eed3-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7eed3-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7eed3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7eed3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7eed3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7eed3-119">Optional query parameters</span></span>
<span data-ttu-id="7eed3-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7eed3-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7eed3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7eed3-121">Request headers</span></span>
|<span data-ttu-id="7eed3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7eed3-122">Header</span></span>|<span data-ttu-id="7eed3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7eed3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7eed3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7eed3-124">Authorization</span></span>|<span data-ttu-id="7eed3-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7eed3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7eed3-126">Accept</span><span class="sxs-lookup"><span data-stu-id="7eed3-126">Accept</span></span>|<span data-ttu-id="7eed3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7eed3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7eed3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7eed3-128">Request body</span></span>
<span data-ttu-id="7eed3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7eed3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7eed3-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7eed3-130">Response</span></span>
<span data-ttu-id="7eed3-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7eed3-131">If successful, this method returns a `200 OK` response code and [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7eed3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7eed3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7eed3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7eed3-133">Request</span></span>
<span data-ttu-id="7eed3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7eed3-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="7eed3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7eed3-135">Response</span></span>
<span data-ttu-id="7eed3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7eed3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 604

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
    "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "omaSettings": [
      {
        "@odata.type": "microsoft.graph.omaSetting",
        "displayName": "Display Name value",
        "description": "Description value",
        "omaUri": "Oma Uri value"
      }
    ]
  }
}
```




