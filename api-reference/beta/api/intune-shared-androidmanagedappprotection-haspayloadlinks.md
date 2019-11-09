---
title: действие Хаспайлоадлинкс
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 254313e5594a06bec117189432fdb6ac6d198913
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086286"
---
# <a name="haspayloadlinks-action"></a><span data-ttu-id="56ca1-103">действие Хаспайлоадлинкс</span><span class="sxs-lookup"><span data-stu-id="56ca1-103">hasPayloadLinks action</span></span>

> <span data-ttu-id="56ca1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56ca1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56ca1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="56ca1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56ca1-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="56ca1-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56ca1-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="56ca1-107">Prerequisites</span></span>
<span data-ttu-id="56ca1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56ca1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56ca1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56ca1-110">Permission type</span></span>|<span data-ttu-id="56ca1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="56ca1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56ca1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56ca1-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="56ca1-113">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="56ca1-113">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="56ca1-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="56ca1-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="56ca1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56ca1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56ca1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56ca1-116">Not supported.</span></span>|
|<span data-ttu-id="56ca1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56ca1-117">Application</span></span>||
| <span data-ttu-id="56ca1-118">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="56ca1-118">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="56ca1-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="56ca1-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56ca1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56ca1-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/androidManagedAppProtections/hasPayloadLinks
```

## <a name="request-headers"></a><span data-ttu-id="56ca1-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="56ca1-121">Request headers</span></span>
|<span data-ttu-id="56ca1-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="56ca1-122">Header</span></span>|<span data-ttu-id="56ca1-123">Значение</span><span class="sxs-lookup"><span data-stu-id="56ca1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56ca1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56ca1-124">Authorization</span></span>|<span data-ttu-id="56ca1-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56ca1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56ca1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="56ca1-126">Accept</span></span>|<span data-ttu-id="56ca1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="56ca1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56ca1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56ca1-128">Request body</span></span>
<span data-ttu-id="56ca1-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56ca1-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="56ca1-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="56ca1-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="56ca1-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="56ca1-131">Property</span></span>|<span data-ttu-id="56ca1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="56ca1-132">Type</span></span>|<span data-ttu-id="56ca1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="56ca1-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56ca1-134">пайлоадидс</span><span class="sxs-lookup"><span data-stu-id="56ca1-134">payloadIds</span></span>|<span data-ttu-id="56ca1-135">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="56ca1-135">String collection</span></span>|<span data-ttu-id="56ca1-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="56ca1-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="56ca1-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="56ca1-137">Response</span></span>
<span data-ttu-id="56ca1-138">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="56ca1-138">If successful, this action returns a `200 OK` response code and a [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56ca1-139">Пример</span><span class="sxs-lookup"><span data-stu-id="56ca1-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="56ca1-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="56ca1-140">Request</span></span>
<span data-ttu-id="56ca1-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56ca1-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="56ca1-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="56ca1-142">Response</span></span>
<span data-ttu-id="56ca1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="56ca1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









