---
title: действие importOffice365DeviceConfigurationPolicies
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 76da266c9bf4d1646634fe7dc5363d2ed5d77e40
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48043509"
---
# <a name="importoffice365deviceconfigurationpolicies-action"></a><span data-ttu-id="0265d-103">действие importOffice365DeviceConfigurationPolicies</span><span class="sxs-lookup"><span data-stu-id="0265d-103">importOffice365DeviceConfigurationPolicies action</span></span>

<span data-ttu-id="0265d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0265d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0265d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0265d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0265d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0265d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0265d-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0265d-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0265d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0265d-108">Prerequisites</span></span>
<span data-ttu-id="0265d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0265d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0265d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0265d-111">Permission type</span></span>|<span data-ttu-id="0265d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0265d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0265d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0265d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0265d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0265d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0265d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0265d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0265d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0265d-116">Not supported.</span></span>|
|<span data-ttu-id="0265d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0265d-117">Application</span></span>|<span data-ttu-id="0265d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0265d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0265d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0265d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/importOffice365DeviceConfigurationPolicies
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/importOffice365DeviceConfigurationPolicies
```

## <a name="request-headers"></a><span data-ttu-id="0265d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0265d-120">Request headers</span></span>
|<span data-ttu-id="0265d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0265d-121">Header</span></span>|<span data-ttu-id="0265d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0265d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0265d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0265d-123">Authorization</span></span>|<span data-ttu-id="0265d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0265d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0265d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0265d-125">Accept</span></span>|<span data-ttu-id="0265d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0265d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0265d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0265d-127">Request body</span></span>
<span data-ttu-id="0265d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0265d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0265d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0265d-129">Response</span></span>
<span data-ttu-id="0265d-130">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0265d-130">If successful, this action returns a `200 OK` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0265d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0265d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0265d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0265d-132">Request</span></span>
<span data-ttu-id="0265d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0265d-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/importOffice365DeviceConfigurationPolicies
```

### <a name="response"></a><span data-ttu-id="0265d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0265d-134">Response</span></span>
<span data-ttu-id="0265d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0265d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 452

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntent",
      "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
      "displayName": "Display Name value",
      "description": "Description value",
      "isAssigned": true,
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "templateId": "Template Id value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```






