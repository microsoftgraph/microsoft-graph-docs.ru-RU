---
title: действие Креатекопи
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e25371a5efb1a9cc342bb6122b464d304848b4ba
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177249"
---
# <a name="createcopy-action"></a><span data-ttu-id="a70ff-103">действие Креатекопи</span><span class="sxs-lookup"><span data-stu-id="a70ff-103">createCopy action</span></span>

<span data-ttu-id="a70ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a70ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a70ff-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a70ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a70ff-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a70ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a70ff-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a70ff-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a70ff-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a70ff-108">Prerequisites</span></span>
<span data-ttu-id="a70ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a70ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a70ff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a70ff-111">Permission type</span></span>|<span data-ttu-id="a70ff-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a70ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a70ff-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a70ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a70ff-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a70ff-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a70ff-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a70ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a70ff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a70ff-116">Not supported.</span></span>|
|<span data-ttu-id="a70ff-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a70ff-117">Application</span></span>|<span data-ttu-id="a70ff-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a70ff-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a70ff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a70ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/createCopy
```

## <a name="request-headers"></a><span data-ttu-id="a70ff-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a70ff-120">Request headers</span></span>
|<span data-ttu-id="a70ff-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a70ff-121">Header</span></span>|<span data-ttu-id="a70ff-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a70ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a70ff-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a70ff-123">Authorization</span></span>|<span data-ttu-id="a70ff-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a70ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a70ff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a70ff-125">Accept</span></span>|<span data-ttu-id="a70ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a70ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a70ff-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a70ff-127">Request body</span></span>
<span data-ttu-id="a70ff-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a70ff-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a70ff-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a70ff-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a70ff-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a70ff-130">Property</span></span>|<span data-ttu-id="a70ff-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a70ff-131">Type</span></span>|<span data-ttu-id="a70ff-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a70ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a70ff-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a70ff-133">displayName</span></span>|<span data-ttu-id="a70ff-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a70ff-134">String</span></span>|<span data-ttu-id="a70ff-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a70ff-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a70ff-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a70ff-136">Response</span></span>
<span data-ttu-id="a70ff-137">При успешном выполнении это действие возвращает `200 OK` код отклика и объект [девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a70ff-137">If successful, this action returns a `200 OK` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a70ff-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a70ff-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a70ff-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a70ff-139">Request</span></span>
<span data-ttu-id="a70ff-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a70ff-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/createCopy

Content-type: application/json
Content-length: 43

{
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="a70ff-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a70ff-141">Response</span></span>
<span data-ttu-id="a70ff-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a70ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 418

{
  "value": {
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
}
```



