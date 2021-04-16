---
title: действие hasPayloadLinks
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: da945082218aead0c8aabd694ede6b6cdead6409
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866379"
---
# <a name="haspayloadlinks-action"></a><span data-ttu-id="ce384-103">действие hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="ce384-103">hasPayloadLinks action</span></span>

<span data-ttu-id="ce384-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce384-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce384-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce384-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce384-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce384-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce384-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ce384-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce384-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ce384-108">Prerequisites</span></span>
<span data-ttu-id="ce384-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce384-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce384-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce384-111">Permission type</span></span>|<span data-ttu-id="ce384-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce384-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce384-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce384-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ce384-114">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="ce384-114">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ce384-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce384-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ce384-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce384-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce384-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce384-117">Not supported.</span></span>|
|<span data-ttu-id="ce384-118">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ce384-118">Application</span></span>||
| <span data-ttu-id="ce384-119">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="ce384-119">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ce384-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce384-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce384-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce384-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles/hasPayloadLinks
```

## <a name="request-headers"></a><span data-ttu-id="ce384-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ce384-122">Request headers</span></span>
|<span data-ttu-id="ce384-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce384-123">Header</span></span>|<span data-ttu-id="ce384-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ce384-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce384-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce384-125">Authorization</span></span>|<span data-ttu-id="ce384-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce384-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce384-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ce384-127">Accept</span></span>|<span data-ttu-id="ce384-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ce384-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce384-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce384-129">Request body</span></span>
<span data-ttu-id="ce384-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce384-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ce384-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="ce384-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ce384-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce384-132">Property</span></span>|<span data-ttu-id="ce384-133">Тип</span><span class="sxs-lookup"><span data-stu-id="ce384-133">Type</span></span>|<span data-ttu-id="ce384-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ce384-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce384-135">payloadIds</span><span class="sxs-lookup"><span data-stu-id="ce384-135">payloadIds</span></span>|<span data-ttu-id="ce384-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ce384-136">String collection</span></span>|<span data-ttu-id="ce384-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ce384-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ce384-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="ce384-138">Response</span></span>
<span data-ttu-id="ce384-139">В случае успешного действия возвращается код ответа и `200 OK` [коллекция hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ce384-139">If successful, this action returns a `200 OK` response code and a [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce384-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ce384-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce384-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce384-141">Request</span></span>
<span data-ttu-id="ce384-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce384-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/hasPayloadLinks

Content-type: application/json
Content-length: 53

{
  "payloadIds": [
    "Payload Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="ce384-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce384-143">Response</span></span>
<span data-ttu-id="ce384-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce384-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.hasPayloadLinkResultItem",
      "payloadId": "Payload Id value",
      "hasLink": true,
      "error": "Error value",
      "sources": [
        "policySets"
      ]
    }
  ]
}
```







