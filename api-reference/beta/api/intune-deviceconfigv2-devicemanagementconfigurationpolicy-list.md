---
title: Список ДевицеманажементконфигуратионполиЦиес
description: Список свойств и связей объектов Девицеманажементконфигуратионполици.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 84aabc5b0fd2a10dfc8eb7e24ee3cf5818e7fa1e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242307"
---
# <a name="list-devicemanagementconfigurationpolicies"></a><span data-ttu-id="6c4f5-103">Список ДевицеманажементконфигуратионполиЦиес</span><span class="sxs-lookup"><span data-stu-id="6c4f5-103">List deviceManagementConfigurationPolicies</span></span>

<span data-ttu-id="6c4f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c4f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c4f5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c4f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c4f5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c4f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c4f5-107">Список свойств и связей объектов [девицеманажементконфигуратионполици](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="6c4f5-107">List properties and relationships of the [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c4f5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6c4f5-108">Prerequisites</span></span>
<span data-ttu-id="6c4f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c4f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c4f5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c4f5-111">Permission type</span></span>|<span data-ttu-id="6c4f5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c4f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c4f5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c4f5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c4f5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c4f5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6c4f5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c4f5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c4f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c4f5-116">Not supported.</span></span>|
|<span data-ttu-id="6c4f5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6c4f5-117">Application</span></span>|<span data-ttu-id="6c4f5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c4f5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c4f5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c4f5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationPolicies
```

## <a name="request-headers"></a><span data-ttu-id="6c4f5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6c4f5-120">Request headers</span></span>
|<span data-ttu-id="6c4f5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c4f5-121">Header</span></span>|<span data-ttu-id="6c4f5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6c4f5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c4f5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c4f5-123">Authorization</span></span>|<span data-ttu-id="6c4f5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c4f5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c4f5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6c4f5-125">Accept</span></span>|<span data-ttu-id="6c4f5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c4f5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c4f5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c4f5-127">Request body</span></span>
<span data-ttu-id="6c4f5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c4f5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c4f5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c4f5-129">Response</span></span>
<span data-ttu-id="6c4f5-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементконфигуратионполици](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c4f5-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c4f5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6c4f5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c4f5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c4f5-132">Request</span></span>
<span data-ttu-id="6c4f5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c4f5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationPolicies
```

### <a name="response"></a><span data-ttu-id="6c4f5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c4f5-134">Response</span></span>
<span data-ttu-id="6c4f5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c4f5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 607

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
      "id": "3ffd7cd0-7cd0-3ffd-d07c-fd3fd07cfd3f",
      "name": "Name value",
      "description": "Description value",
      "platforms": "macOS",
      "technologies": "mdm",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "settingCount": 12,
      "creationSource": "Creation Source value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "isAssigned": true
    }
  ]
}
```




