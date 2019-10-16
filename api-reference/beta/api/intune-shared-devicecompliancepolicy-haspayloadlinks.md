---
title: действие Хаспайлоадлинкс
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 56dcbe4c2235f85967c627547cd6c9b9e6439b3f
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536191"
---
# <a name="haspayloadlinks-action"></a><span data-ttu-id="34793-103">действие Хаспайлоадлинкс</span><span class="sxs-lookup"><span data-stu-id="34793-103">hasPayloadLinks action</span></span>

> <span data-ttu-id="34793-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34793-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34793-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34793-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34793-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="34793-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34793-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="34793-107">Prerequisites</span></span>
<span data-ttu-id="34793-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34793-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34793-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34793-110">Permission type</span></span>|<span data-ttu-id="34793-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="34793-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34793-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34793-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="34793-113">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="34793-113">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="34793-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="34793-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="34793-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34793-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34793-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34793-116">Not supported.</span></span>|
|<span data-ttu-id="34793-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="34793-117">Application</span></span>||
| <span data-ttu-id="34793-118">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="34793-118">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="34793-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="34793-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34793-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34793-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/hasPayloadLinks
```

## <a name="request-headers"></a><span data-ttu-id="34793-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34793-121">Request headers</span></span>
|<span data-ttu-id="34793-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34793-122">Header</span></span>|<span data-ttu-id="34793-123">Значение</span><span class="sxs-lookup"><span data-stu-id="34793-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34793-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34793-124">Authorization</span></span>|<span data-ttu-id="34793-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34793-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34793-126">Accept</span><span class="sxs-lookup"><span data-stu-id="34793-126">Accept</span></span>|<span data-ttu-id="34793-127">application/json</span><span class="sxs-lookup"><span data-stu-id="34793-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34793-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34793-128">Request body</span></span>
<span data-ttu-id="34793-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34793-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="34793-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="34793-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="34793-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="34793-131">Property</span></span>|<span data-ttu-id="34793-132">Тип</span><span class="sxs-lookup"><span data-stu-id="34793-132">Type</span></span>|<span data-ttu-id="34793-133">Описание</span><span class="sxs-lookup"><span data-stu-id="34793-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34793-134">пайлоадидс</span><span class="sxs-lookup"><span data-stu-id="34793-134">payloadIds</span></span>|<span data-ttu-id="34793-135">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="34793-135">String collection</span></span>|<span data-ttu-id="34793-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="34793-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="34793-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="34793-137">Response</span></span>
<span data-ttu-id="34793-138">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34793-138">If successful, this action returns a `200 OK` response code and a [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34793-139">Пример</span><span class="sxs-lookup"><span data-stu-id="34793-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="34793-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="34793-140">Request</span></span>
<span data-ttu-id="34793-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34793-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/hasPayloadLinks

Content-type: application/json
Content-length: 53

{
  "payloadIds": [
    "Payload Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="34793-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="34793-142">Response</span></span>
<span data-ttu-id="34793-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34793-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






