---
title: действие Хаспайлоадлинкс
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c1b2124c5d2abc85b6ee426ef50e60be367e8f8b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801294"
---
# <a name="haspayloadlinks-action"></a><span data-ttu-id="8712e-103">действие Хаспайлоадлинкс</span><span class="sxs-lookup"><span data-stu-id="8712e-103">hasPayloadLinks action</span></span>

> <span data-ttu-id="8712e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8712e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8712e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8712e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8712e-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8712e-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8712e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8712e-107">Prerequisites</span></span>
<span data-ttu-id="8712e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8712e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8712e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8712e-110">Permission type</span></span>|<span data-ttu-id="8712e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8712e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8712e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8712e-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8712e-113">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="8712e-113">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="8712e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8712e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8712e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8712e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8712e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8712e-116">Not supported.</span></span>|
|<span data-ttu-id="8712e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8712e-117">Application</span></span>||
| <span data-ttu-id="8712e-118">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="8712e-118">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="8712e-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8712e-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8712e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8712e-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/androidManagedAppProtections/hasPayloadLinks
```

## <a name="request-headers"></a><span data-ttu-id="8712e-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8712e-121">Request headers</span></span>
|<span data-ttu-id="8712e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8712e-122">Header</span></span>|<span data-ttu-id="8712e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8712e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8712e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8712e-124">Authorization</span></span>|<span data-ttu-id="8712e-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8712e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8712e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8712e-126">Accept</span></span>|<span data-ttu-id="8712e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8712e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8712e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8712e-128">Request body</span></span>
<span data-ttu-id="8712e-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8712e-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8712e-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="8712e-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8712e-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="8712e-131">Property</span></span>|<span data-ttu-id="8712e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8712e-132">Type</span></span>|<span data-ttu-id="8712e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8712e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8712e-134">пайлоадидс</span><span class="sxs-lookup"><span data-stu-id="8712e-134">payloadIds</span></span>|<span data-ttu-id="8712e-135">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8712e-135">String collection</span></span>|<span data-ttu-id="8712e-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8712e-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8712e-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="8712e-137">Response</span></span>
<span data-ttu-id="8712e-138">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8712e-138">If successful, this action returns a `200 OK` response code and a [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8712e-139">Пример</span><span class="sxs-lookup"><span data-stu-id="8712e-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="8712e-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="8712e-140">Request</span></span>
<span data-ttu-id="8712e-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8712e-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections/hasPayloadLinks

Content-type: application/json
Content-length: 53

{
  "payloadIds": [
    "Payload Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="8712e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8712e-142">Response</span></span>
<span data-ttu-id="8712e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8712e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







