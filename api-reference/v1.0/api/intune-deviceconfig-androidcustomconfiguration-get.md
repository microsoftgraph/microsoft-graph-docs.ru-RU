---
title: Get androidCustomConfiguration
description: Чтение свойств и связей объекта androidCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 629be2f6358e3bec63230941532d145a45dea9cc
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262526"
---
# <a name="get-androidcustomconfiguration"></a><span data-ttu-id="dc5da-103">Get androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="dc5da-103">Get androidCustomConfiguration</span></span>

> <span data-ttu-id="dc5da-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc5da-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc5da-105">Чтение свойств и связей объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dc5da-105">Read properties and relationships of the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc5da-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="dc5da-106">Prerequisites</span></span>
<span data-ttu-id="dc5da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dc5da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dc5da-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc5da-109">Permission type</span></span>|<span data-ttu-id="dc5da-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc5da-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc5da-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc5da-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dc5da-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc5da-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dc5da-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc5da-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc5da-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc5da-114">Not supported.</span></span>|
|<span data-ttu-id="dc5da-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc5da-115">Application</span></span>|<span data-ttu-id="dc5da-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc5da-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc5da-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc5da-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dc5da-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dc5da-118">Optional query parameters</span></span>
<span data-ttu-id="dc5da-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dc5da-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc5da-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc5da-120">Request headers</span></span>
|<span data-ttu-id="dc5da-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc5da-121">Header</span></span>|<span data-ttu-id="dc5da-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dc5da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc5da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc5da-123">Authorization</span></span>|<span data-ttu-id="dc5da-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dc5da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc5da-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dc5da-125">Accept</span></span>|<span data-ttu-id="dc5da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc5da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc5da-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc5da-127">Request body</span></span>
<span data-ttu-id="dc5da-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dc5da-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc5da-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc5da-129">Response</span></span>
<span data-ttu-id="dc5da-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dc5da-130">If successful, this method returns a `200 OK` response code and [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc5da-131">Пример</span><span class="sxs-lookup"><span data-stu-id="dc5da-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc5da-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc5da-132">Request</span></span>
<span data-ttu-id="dc5da-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc5da-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="dc5da-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc5da-134">Response</span></span>
<span data-ttu-id="dc5da-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dc5da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 625

{
  "value": {
    "@odata.type": "#microsoft.graph.androidCustomConfiguration",
    "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "omaSettings": [
      {
        "@odata.type": "microsoft.graph.omaSettingInteger",
        "displayName": "Display Name value",
        "description": "Description value",
        "omaUri": "Oma Uri value",
        "value": 5
      }
    ]
  }
}
```



