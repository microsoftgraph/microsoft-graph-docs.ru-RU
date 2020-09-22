---
title: Перечисление объектов deviceEnrollmentConfiguration
description: Список свойств и связей объектов deviceEnrollmentConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a869ac8bf8145c663d7283a9c0d61743edc22a6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48068093"
---
# <a name="list-deviceenrollmentconfigurations"></a><span data-ttu-id="dcdde-103">Перечисление объектов deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="dcdde-103">List deviceEnrollmentConfigurations</span></span>

<span data-ttu-id="dcdde-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcdde-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dcdde-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcdde-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcdde-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dcdde-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcdde-107">Список свойств и связей объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dcdde-107">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcdde-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dcdde-108">Prerequisites</span></span>
<span data-ttu-id="dcdde-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcdde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcdde-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dcdde-111">Permission type</span></span>|<span data-ttu-id="dcdde-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dcdde-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcdde-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dcdde-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="dcdde-114">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="dcdde-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="dcdde-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcdde-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="dcdde-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="dcdde-116">&nbsp; &nbsp; **Policy Set**</span></span>| <span data-ttu-id="dcdde-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcdde-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="dcdde-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dcdde-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcdde-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcdde-119">Not supported.</span></span>|
|<span data-ttu-id="dcdde-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dcdde-120">Application</span></span>||
| <span data-ttu-id="dcdde-121">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="dcdde-121">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="dcdde-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcdde-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="dcdde-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="dcdde-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="dcdde-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcdde-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcdde-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dcdde-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dcdde-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dcdde-126">Request headers</span></span>
|<span data-ttu-id="dcdde-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dcdde-127">Header</span></span>|<span data-ttu-id="dcdde-128">Значение</span><span class="sxs-lookup"><span data-stu-id="dcdde-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcdde-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dcdde-129">Authorization</span></span>|<span data-ttu-id="dcdde-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dcdde-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcdde-131">Accept</span><span class="sxs-lookup"><span data-stu-id="dcdde-131">Accept</span></span>|<span data-ttu-id="dcdde-132">application/json</span><span class="sxs-lookup"><span data-stu-id="dcdde-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcdde-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dcdde-133">Request body</span></span>
<span data-ttu-id="dcdde-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dcdde-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcdde-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcdde-135">Response</span></span>
<span data-ttu-id="dcdde-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dcdde-136">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcdde-137">Пример</span><span class="sxs-lookup"><span data-stu-id="dcdde-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcdde-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="dcdde-138">Request</span></span>
<span data-ttu-id="dcdde-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dcdde-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="dcdde-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcdde-140">Response</span></span>
<span data-ttu-id="dcdde-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dcdde-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









