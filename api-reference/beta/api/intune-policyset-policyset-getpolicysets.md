---
title: действие getPolicySets
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fbdf718bd9caac3acb4c8b843d93bffc5a40feb1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134601"
---
# <a name="getpolicysets-action"></a><span data-ttu-id="a5d3f-103">действие getPolicySets</span><span class="sxs-lookup"><span data-stu-id="a5d3f-103">getPolicySets action</span></span>

<span data-ttu-id="a5d3f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5d3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5d3f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5d3f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5d3f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5d3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5d3f-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a5d3f-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5d3f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a5d3f-108">Prerequisites</span></span>
<span data-ttu-id="a5d3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5d3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5d3f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5d3f-111">Permission type</span></span>|<span data-ttu-id="a5d3f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5d3f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5d3f-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5d3f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a5d3f-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5d3f-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a5d3f-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5d3f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5d3f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5d3f-116">Not supported.</span></span>|
|<span data-ttu-id="a5d3f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a5d3f-117">Application</span></span>|<span data-ttu-id="a5d3f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5d3f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5d3f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5d3f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/getPolicySets
```

## <a name="request-headers"></a><span data-ttu-id="a5d3f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a5d3f-120">Request headers</span></span>
|<span data-ttu-id="a5d3f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5d3f-121">Header</span></span>|<span data-ttu-id="a5d3f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a5d3f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5d3f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5d3f-123">Authorization</span></span>|<span data-ttu-id="a5d3f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5d3f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5d3f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a5d3f-125">Accept</span></span>|<span data-ttu-id="a5d3f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5d3f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5d3f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5d3f-127">Request body</span></span>
<span data-ttu-id="a5d3f-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5d3f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a5d3f-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a5d3f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a5d3f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5d3f-130">Property</span></span>|<span data-ttu-id="a5d3f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a5d3f-131">Type</span></span>|<span data-ttu-id="a5d3f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a5d3f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5d3f-133">policySetIds</span><span class="sxs-lookup"><span data-stu-id="a5d3f-133">policySetIds</span></span>|<span data-ttu-id="a5d3f-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a5d3f-134">String collection</span></span>|<span data-ttu-id="a5d3f-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a5d3f-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a5d3f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a5d3f-136">Response</span></span>
<span data-ttu-id="a5d3f-137">В случае успеха это действие возвращает код отклика и `200 OK` коллекцию [policySet](../resources/intune-policyset-policyset.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a5d3f-137">If successful, this action returns a `200 OK` response code and a [policySet](../resources/intune-policyset-policyset.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5d3f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a5d3f-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5d3f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5d3f-139">Request</span></span>
<span data-ttu-id="a5d3f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5d3f-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/getPolicySets

Content-type: application/json
Content-length: 58

{
  "policySetIds": [
    "Policy Set Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="a5d3f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5d3f-141">Response</span></span>
<span data-ttu-id="a5d3f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a5d3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 578

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.policySet",
      "id": "653cb373-b373-653c-73b3-3c6573b33c65",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "status": "validating",
      "errorCode": "unauthorized",
      "guidedDeploymentTags": [
        "Guided Deployment Tags value"
      ],
      "roleScopeTags": [
        "Role Scope Tags value"
      ]
    }
  ]
}
```




