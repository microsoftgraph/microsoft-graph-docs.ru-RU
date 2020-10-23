---
title: действие Хаспайлоадлинкс
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c79a406823d2c225092d5509c90dcc1b486cab56
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729919"
---
# <a name="haspayloadlinks-action"></a><span data-ttu-id="45ff5-103">действие Хаспайлоадлинкс</span><span class="sxs-lookup"><span data-stu-id="45ff5-103">hasPayloadLinks action</span></span>

<span data-ttu-id="45ff5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45ff5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45ff5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45ff5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45ff5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45ff5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45ff5-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="45ff5-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45ff5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="45ff5-108">Prerequisites</span></span>
<span data-ttu-id="45ff5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45ff5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45ff5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45ff5-111">Permission type</span></span>|<span data-ttu-id="45ff5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45ff5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45ff5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45ff5-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="45ff5-114">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="45ff5-114">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="45ff5-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="45ff5-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="45ff5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45ff5-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45ff5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45ff5-117">Not supported.</span></span>|
|<span data-ttu-id="45ff5-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45ff5-118">Application</span></span>||
| <span data-ttu-id="45ff5-119">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="45ff5-119">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="45ff5-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="45ff5-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45ff5-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45ff5-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/hasPayloadLinks
```

## <a name="request-headers"></a><span data-ttu-id="45ff5-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="45ff5-122">Request headers</span></span>
|<span data-ttu-id="45ff5-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45ff5-123">Header</span></span>|<span data-ttu-id="45ff5-124">Значение</span><span class="sxs-lookup"><span data-stu-id="45ff5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45ff5-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45ff5-125">Authorization</span></span>|<span data-ttu-id="45ff5-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45ff5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45ff5-127">Accept</span><span class="sxs-lookup"><span data-stu-id="45ff5-127">Accept</span></span>|<span data-ttu-id="45ff5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="45ff5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45ff5-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45ff5-129">Request body</span></span>
<span data-ttu-id="45ff5-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45ff5-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="45ff5-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="45ff5-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="45ff5-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="45ff5-132">Property</span></span>|<span data-ttu-id="45ff5-133">Тип</span><span class="sxs-lookup"><span data-stu-id="45ff5-133">Type</span></span>|<span data-ttu-id="45ff5-134">Описание</span><span class="sxs-lookup"><span data-stu-id="45ff5-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45ff5-135">пайлоадидс</span><span class="sxs-lookup"><span data-stu-id="45ff5-135">payloadIds</span></span>|<span data-ttu-id="45ff5-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="45ff5-136">String collection</span></span>|<span data-ttu-id="45ff5-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="45ff5-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="45ff5-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="45ff5-138">Response</span></span>
<span data-ttu-id="45ff5-139">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45ff5-139">If successful, this action returns a `200 OK` response code and a [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45ff5-140">Пример</span><span class="sxs-lookup"><span data-stu-id="45ff5-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="45ff5-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="45ff5-141">Request</span></span>
<span data-ttu-id="45ff5-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45ff5-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/hasPayloadLinks

Content-type: application/json
Content-length: 53

{
  "payloadIds": [
    "Payload Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="45ff5-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="45ff5-143">Response</span></span>
<span data-ttu-id="45ff5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45ff5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








