---
title: Список Граупполициконфигуратионс
description: Список свойств и связей объектов Граупполициконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b1c08df7779aa9b44f50634a2576b5b881234839
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087091"
---
# <a name="list-grouppolicyconfigurations"></a><span data-ttu-id="72041-103">Список Граупполициконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="72041-103">List groupPolicyConfigurations</span></span>

> <span data-ttu-id="72041-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72041-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72041-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72041-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72041-106">Список свойств и связей объектов [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="72041-106">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72041-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="72041-107">Prerequisites</span></span>
<span data-ttu-id="72041-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72041-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72041-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72041-110">Permission type</span></span>|<span data-ttu-id="72041-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="72041-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72041-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72041-112">Delegated (work or school account)</span></span>|<span data-ttu-id="72041-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="72041-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="72041-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72041-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72041-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72041-115">Not supported.</span></span>|
|<span data-ttu-id="72041-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72041-116">Application</span></span>|<span data-ttu-id="72041-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="72041-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72041-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72041-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="72041-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="72041-119">Request headers</span></span>
|<span data-ttu-id="72041-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72041-120">Header</span></span>|<span data-ttu-id="72041-121">Значение</span><span class="sxs-lookup"><span data-stu-id="72041-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72041-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72041-122">Authorization</span></span>|<span data-ttu-id="72041-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72041-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72041-124">Accept</span><span class="sxs-lookup"><span data-stu-id="72041-124">Accept</span></span>|<span data-ttu-id="72041-125">application/json</span><span class="sxs-lookup"><span data-stu-id="72041-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72041-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72041-126">Request body</span></span>
<span data-ttu-id="72041-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72041-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72041-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="72041-128">Response</span></span>
<span data-ttu-id="72041-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72041-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72041-130">Пример</span><span class="sxs-lookup"><span data-stu-id="72041-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="72041-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="72041-131">Request</span></span>
<span data-ttu-id="72041-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72041-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations
```

### <a name="response"></a><span data-ttu-id="72041-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="72041-133">Response</span></span>
<span data-ttu-id="72041-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72041-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 448

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "27b935ec-35ec-27b9-ec35-b927ec35b927",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```






