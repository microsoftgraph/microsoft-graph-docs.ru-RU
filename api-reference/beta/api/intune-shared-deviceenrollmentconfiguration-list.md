---
title: Перечисление объектов deviceEnrollmentConfiguration
description: Список свойств и связей объектов deviceEnrollmentConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3323599ba9731a109b3dd6841fbc90179b5cf48a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940021"
---
# <a name="list-deviceenrollmentconfigurations"></a><span data-ttu-id="44366-103">Перечисление объектов deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="44366-103">List deviceEnrollmentConfigurations</span></span>

> <span data-ttu-id="44366-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44366-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44366-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44366-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44366-106">Список свойств и связей объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44366-106">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44366-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="44366-107">Prerequisites</span></span>
<span data-ttu-id="44366-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44366-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44366-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44366-110">Permission type</span></span>|<span data-ttu-id="44366-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44366-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44366-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44366-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="44366-113">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="44366-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="44366-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="44366-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="44366-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="44366-115">&nbsp; &nbsp; **Policy Set**</span></span>| <span data-ttu-id="44366-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="44366-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="44366-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44366-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44366-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44366-118">Not supported.</span></span>|
|<span data-ttu-id="44366-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44366-119">Application</span></span>||
| <span data-ttu-id="44366-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="44366-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="44366-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="44366-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="44366-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="44366-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="44366-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="44366-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44366-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44366-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="44366-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="44366-125">Request headers</span></span>
|<span data-ttu-id="44366-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44366-126">Header</span></span>|<span data-ttu-id="44366-127">Значение</span><span class="sxs-lookup"><span data-stu-id="44366-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44366-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44366-128">Authorization</span></span>|<span data-ttu-id="44366-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44366-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44366-130">Accept</span><span class="sxs-lookup"><span data-stu-id="44366-130">Accept</span></span>|<span data-ttu-id="44366-131">application/json</span><span class="sxs-lookup"><span data-stu-id="44366-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44366-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44366-132">Request body</span></span>
<span data-ttu-id="44366-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44366-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44366-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="44366-134">Response</span></span>
<span data-ttu-id="44366-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="44366-135">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44366-136">Пример</span><span class="sxs-lookup"><span data-stu-id="44366-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="44366-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="44366-137">Request</span></span>
<span data-ttu-id="44366-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44366-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="44366-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="44366-139">Response</span></span>
<span data-ttu-id="44366-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44366-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








