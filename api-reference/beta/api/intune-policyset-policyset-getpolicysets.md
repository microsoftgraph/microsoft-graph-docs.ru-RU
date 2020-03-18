---
title: действие Жетполицисетс
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d2908866f28eceb9e50467566c41fc0b7f65b59e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802127"
---
# <a name="getpolicysets-action"></a><span data-ttu-id="c51d3-103">действие Жетполицисетс</span><span class="sxs-lookup"><span data-stu-id="c51d3-103">getPolicySets action</span></span>

> <span data-ttu-id="c51d3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c51d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c51d3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c51d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c51d3-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c51d3-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c51d3-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c51d3-107">Prerequisites</span></span>
<span data-ttu-id="c51d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c51d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c51d3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c51d3-110">Permission type</span></span>|<span data-ttu-id="c51d3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c51d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c51d3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c51d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c51d3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c51d3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c51d3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c51d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c51d3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c51d3-115">Not supported.</span></span>|
|<span data-ttu-id="c51d3-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c51d3-116">Application</span></span>|<span data-ttu-id="c51d3-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c51d3-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c51d3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c51d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/getPolicySets
```

## <a name="request-headers"></a><span data-ttu-id="c51d3-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c51d3-119">Request headers</span></span>
|<span data-ttu-id="c51d3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c51d3-120">Header</span></span>|<span data-ttu-id="c51d3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c51d3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c51d3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c51d3-122">Authorization</span></span>|<span data-ttu-id="c51d3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c51d3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c51d3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c51d3-124">Accept</span></span>|<span data-ttu-id="c51d3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c51d3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c51d3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c51d3-126">Request body</span></span>
<span data-ttu-id="c51d3-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c51d3-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c51d3-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c51d3-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c51d3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c51d3-129">Property</span></span>|<span data-ttu-id="c51d3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c51d3-130">Type</span></span>|<span data-ttu-id="c51d3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c51d3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c51d3-132">полицисетидс</span><span class="sxs-lookup"><span data-stu-id="c51d3-132">policySetIds</span></span>|<span data-ttu-id="c51d3-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c51d3-133">String collection</span></span>|<span data-ttu-id="c51d3-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c51d3-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c51d3-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="c51d3-135">Response</span></span>
<span data-ttu-id="c51d3-136">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию набора [политик](../resources/intune-policyset-policyset.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c51d3-136">If successful, this action returns a `200 OK` response code and a [policySet](../resources/intune-policyset-policyset.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c51d3-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c51d3-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c51d3-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="c51d3-138">Request</span></span>
<span data-ttu-id="c51d3-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c51d3-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c51d3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c51d3-140">Response</span></span>
<span data-ttu-id="c51d3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c51d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




