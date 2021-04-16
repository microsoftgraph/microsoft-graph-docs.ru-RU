---
title: Перечисление объектов deviceCompliancePolicy
description: Список свойств и связей объектов deviceCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 41a38f453d524e73dc1d0a3b79718ca559deee02
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863375"
---
# <a name="list-devicecompliancepolicies"></a><span data-ttu-id="d946a-103">Перечисление объектов deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d946a-103">List deviceCompliancePolicies</span></span>

<span data-ttu-id="d946a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d946a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d946a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d946a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d946a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d946a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d946a-107">Список свойств и связей объектов [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d946a-107">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d946a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d946a-108">Prerequisites</span></span>
<span data-ttu-id="d946a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d946a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d946a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d946a-111">Permission type</span></span>|<span data-ttu-id="d946a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d946a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d946a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d946a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d946a-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="d946a-114">&nbsp; &nbsp; **Device configuration**</span></span>  | <span data-ttu-id="d946a-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d946a-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="d946a-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d946a-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d946a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d946a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d946a-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d946a-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d946a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d946a-119">Not supported.</span></span>|
|<span data-ttu-id="d946a-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d946a-120">Application</span></span>||
| <span data-ttu-id="d946a-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="d946a-121">&nbsp; &nbsp; **Device configuration**</span></span>  | <span data-ttu-id="d946a-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d946a-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="d946a-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d946a-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d946a-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d946a-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d946a-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d946a-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="d946a-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d946a-126">Request headers</span></span>
|<span data-ttu-id="d946a-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d946a-127">Header</span></span>|<span data-ttu-id="d946a-128">Значение</span><span class="sxs-lookup"><span data-stu-id="d946a-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d946a-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d946a-129">Authorization</span></span>|<span data-ttu-id="d946a-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d946a-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d946a-131">Accept</span><span class="sxs-lookup"><span data-stu-id="d946a-131">Accept</span></span>|<span data-ttu-id="d946a-132">application/json</span><span class="sxs-lookup"><span data-stu-id="d946a-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d946a-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d946a-133">Request body</span></span>
<span data-ttu-id="d946a-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d946a-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d946a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d946a-135">Response</span></span>
<span data-ttu-id="d946a-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d946a-136">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d946a-137">Пример</span><span class="sxs-lookup"><span data-stu-id="d946a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="d946a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="d946a-138">Request</span></span>
<span data-ttu-id="d946a-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d946a-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="d946a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d946a-140">Response</span></span>
<span data-ttu-id="d946a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d946a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 467

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "4214b716-b716-4214-16b7-144216b71442",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```







