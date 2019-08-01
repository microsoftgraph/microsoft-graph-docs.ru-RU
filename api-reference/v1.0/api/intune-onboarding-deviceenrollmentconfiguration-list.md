---
title: Перечисление объектов deviceEnrollmentConfiguration
description: Список свойств и связей объектов deviceEnrollmentConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 871032421bd18eab0a622df0449804fa1da82e3f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018066"
---
# <a name="list-deviceenrollmentconfigurations"></a><span data-ttu-id="fa930-103">Перечисление объектов deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="fa930-103">List deviceEnrollmentConfigurations</span></span>

> <span data-ttu-id="fa930-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa930-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa930-105">Список свойств и связей объектов [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa930-105">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa930-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fa930-106">Prerequisites</span></span>
<span data-ttu-id="fa930-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa930-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa930-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa930-109">Permission type</span></span>|<span data-ttu-id="fa930-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa930-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa930-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa930-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa930-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa930-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fa930-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa930-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa930-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa930-114">Not supported.</span></span>|
|<span data-ttu-id="fa930-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa930-115">Application</span></span>|<span data-ttu-id="fa930-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa930-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa930-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa930-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fa930-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa930-118">Request headers</span></span>
|<span data-ttu-id="fa930-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa930-119">Header</span></span>|<span data-ttu-id="fa930-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fa930-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa930-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa930-121">Authorization</span></span>|<span data-ttu-id="fa930-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa930-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa930-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fa930-123">Accept</span></span>|<span data-ttu-id="fa930-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fa930-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa930-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fa930-125">Request body</span></span>
<span data-ttu-id="fa930-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa930-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa930-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa930-127">Response</span></span>
<span data-ttu-id="fa930-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fa930-128">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa930-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fa930-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa930-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa930-130">Request</span></span>
<span data-ttu-id="fa930-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa930-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="fa930-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa930-132">Response</span></span>
<span data-ttu-id="fa930-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa930-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7
    }
  ]
}
```



