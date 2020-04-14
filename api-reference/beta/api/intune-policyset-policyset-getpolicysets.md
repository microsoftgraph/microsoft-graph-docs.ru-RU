---
title: действие Жетполицисетс
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d63abb1649308f726e7dfc7e5225b50a977cef79
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457743"
---
# <a name="getpolicysets-action"></a><span data-ttu-id="6f84a-103">действие Жетполицисетс</span><span class="sxs-lookup"><span data-stu-id="6f84a-103">getPolicySets action</span></span>

<span data-ttu-id="6f84a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f84a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f84a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f84a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f84a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f84a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f84a-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6f84a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f84a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6f84a-108">Prerequisites</span></span>
<span data-ttu-id="6f84a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f84a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f84a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f84a-111">Permission type</span></span>|<span data-ttu-id="6f84a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f84a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f84a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f84a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f84a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f84a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6f84a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f84a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f84a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f84a-116">Not supported.</span></span>|
|<span data-ttu-id="6f84a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f84a-117">Application</span></span>|<span data-ttu-id="6f84a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f84a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f84a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f84a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/getPolicySets
```

## <a name="request-headers"></a><span data-ttu-id="6f84a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6f84a-120">Request headers</span></span>
|<span data-ttu-id="6f84a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f84a-121">Header</span></span>|<span data-ttu-id="6f84a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6f84a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f84a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f84a-123">Authorization</span></span>|<span data-ttu-id="6f84a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f84a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f84a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6f84a-125">Accept</span></span>|<span data-ttu-id="6f84a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f84a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f84a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f84a-127">Request body</span></span>
<span data-ttu-id="6f84a-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f84a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6f84a-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="6f84a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6f84a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f84a-130">Property</span></span>|<span data-ttu-id="6f84a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6f84a-131">Type</span></span>|<span data-ttu-id="6f84a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6f84a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f84a-133">полицисетидс</span><span class="sxs-lookup"><span data-stu-id="6f84a-133">policySetIds</span></span>|<span data-ttu-id="6f84a-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6f84a-134">String collection</span></span>|<span data-ttu-id="6f84a-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6f84a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6f84a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f84a-136">Response</span></span>
<span data-ttu-id="6f84a-137">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию набора [политик](../resources/intune-policyset-policyset.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6f84a-137">If successful, this action returns a `200 OK` response code and a [policySet](../resources/intune-policyset-policyset.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f84a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="6f84a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f84a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f84a-139">Request</span></span>
<span data-ttu-id="6f84a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f84a-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6f84a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f84a-141">Response</span></span>
<span data-ttu-id="6f84a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f84a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



