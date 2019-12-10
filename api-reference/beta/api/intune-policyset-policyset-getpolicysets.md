---
title: действие Жетполицисетс
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ad53b5938ec6cd7c2a40dbe8e790579da668d2b9
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940961"
---
# <a name="getpolicysets-action"></a><span data-ttu-id="78c2e-103">действие Жетполицисетс</span><span class="sxs-lookup"><span data-stu-id="78c2e-103">getPolicySets action</span></span>

> <span data-ttu-id="78c2e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78c2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78c2e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="78c2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78c2e-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="78c2e-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78c2e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="78c2e-107">Prerequisites</span></span>
<span data-ttu-id="78c2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78c2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78c2e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78c2e-110">Permission type</span></span>|<span data-ttu-id="78c2e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="78c2e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78c2e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78c2e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="78c2e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="78c2e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="78c2e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78c2e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78c2e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78c2e-115">Not supported.</span></span>|
|<span data-ttu-id="78c2e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78c2e-116">Application</span></span>|<span data-ttu-id="78c2e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="78c2e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78c2e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78c2e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/getPolicySets
```

## <a name="request-headers"></a><span data-ttu-id="78c2e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="78c2e-119">Request headers</span></span>
|<span data-ttu-id="78c2e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="78c2e-120">Header</span></span>|<span data-ttu-id="78c2e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="78c2e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78c2e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="78c2e-122">Authorization</span></span>|<span data-ttu-id="78c2e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78c2e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78c2e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="78c2e-124">Accept</span></span>|<span data-ttu-id="78c2e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="78c2e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78c2e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="78c2e-126">Request body</span></span>
<span data-ttu-id="78c2e-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78c2e-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="78c2e-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="78c2e-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="78c2e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="78c2e-129">Property</span></span>|<span data-ttu-id="78c2e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="78c2e-130">Type</span></span>|<span data-ttu-id="78c2e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="78c2e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78c2e-132">полицисетидс</span><span class="sxs-lookup"><span data-stu-id="78c2e-132">policySetIds</span></span>|<span data-ttu-id="78c2e-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="78c2e-133">String collection</span></span>|<span data-ttu-id="78c2e-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="78c2e-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="78c2e-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="78c2e-135">Response</span></span>
<span data-ttu-id="78c2e-136">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию набора [политик](../resources/intune-policyset-policyset.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="78c2e-136">If successful, this action returns a `200 OK` response code and a [policySet](../resources/intune-policyset-policyset.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78c2e-137">Пример</span><span class="sxs-lookup"><span data-stu-id="78c2e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="78c2e-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="78c2e-138">Request</span></span>
<span data-ttu-id="78c2e-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78c2e-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="78c2e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="78c2e-140">Response</span></span>
<span data-ttu-id="78c2e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="78c2e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





