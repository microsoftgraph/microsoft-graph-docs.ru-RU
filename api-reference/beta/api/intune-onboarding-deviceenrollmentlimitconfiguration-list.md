---
title: Перечисление объектов deviceEnrollmentLimitConfiguration
description: Список свойств и связей объектов deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b89e3b6fc65794d6a45fbafc410b4537ef16156
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179434"
---
# <a name="list-deviceenrollmentlimitconfigurations"></a><span data-ttu-id="971bc-103">Перечисление объектов deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="971bc-103">List deviceEnrollmentLimitConfigurations</span></span>

<span data-ttu-id="971bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="971bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="971bc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="971bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="971bc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="971bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="971bc-107">Список свойств и связей объектов [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="971bc-107">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="971bc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="971bc-108">Prerequisites</span></span>
<span data-ttu-id="971bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="971bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="971bc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="971bc-111">Permission type</span></span>|<span data-ttu-id="971bc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="971bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="971bc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="971bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="971bc-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="971bc-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="971bc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="971bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="971bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="971bc-116">Not supported.</span></span>|
|<span data-ttu-id="971bc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="971bc-117">Application</span></span>|<span data-ttu-id="971bc-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="971bc-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="971bc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="971bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="971bc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="971bc-120">Request headers</span></span>
|<span data-ttu-id="971bc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="971bc-121">Header</span></span>|<span data-ttu-id="971bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="971bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="971bc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="971bc-123">Authorization</span></span>|<span data-ttu-id="971bc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="971bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="971bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="971bc-125">Accept</span></span>|<span data-ttu-id="971bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="971bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="971bc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="971bc-127">Request body</span></span>
<span data-ttu-id="971bc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="971bc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="971bc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="971bc-129">Response</span></span>
<span data-ttu-id="971bc-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="971bc-130">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="971bc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="971bc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="971bc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="971bc-132">Request</span></span>
<span data-ttu-id="971bc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="971bc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="971bc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="971bc-134">Response</span></span>
<span data-ttu-id="971bc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="971bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 520

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
      "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "limit": 5
    }
  ]
}
```



