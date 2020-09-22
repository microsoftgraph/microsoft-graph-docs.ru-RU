---
title: Функция Compare
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c3d2be68278d41ba842105aa750b0f26cdc8d753
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48047646"
---
# <a name="compare-function"></a><span data-ttu-id="ca03c-103">Функция Compare</span><span class="sxs-lookup"><span data-stu-id="ca03c-103">compare function</span></span>

<span data-ttu-id="ca03c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca03c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca03c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca03c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca03c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca03c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca03c-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ca03c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca03c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ca03c-108">Prerequisites</span></span>
<span data-ttu-id="ca03c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca03c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca03c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca03c-111">Permission type</span></span>|<span data-ttu-id="ca03c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca03c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca03c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca03c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca03c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca03c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ca03c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca03c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca03c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca03c-116">Not supported.</span></span>|
|<span data-ttu-id="ca03c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca03c-117">Application</span></span>|<span data-ttu-id="ca03c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca03c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca03c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca03c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/compare
```

## <a name="request-headers"></a><span data-ttu-id="ca03c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ca03c-120">Request headers</span></span>
|<span data-ttu-id="ca03c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca03c-121">Header</span></span>|<span data-ttu-id="ca03c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ca03c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca03c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca03c-123">Authorization</span></span>|<span data-ttu-id="ca03c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca03c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca03c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ca03c-125">Accept</span></span>|<span data-ttu-id="ca03c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca03c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca03c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ca03c-127">Request body</span></span>
<span data-ttu-id="ca03c-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ca03c-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ca03c-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="ca03c-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ca03c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca03c-130">Property</span></span>|<span data-ttu-id="ca03c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ca03c-131">Type</span></span>|<span data-ttu-id="ca03c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ca03c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca03c-133">templateId</span><span class="sxs-lookup"><span data-stu-id="ca03c-133">templateId</span></span>|<span data-ttu-id="ca03c-134">String</span><span class="sxs-lookup"><span data-stu-id="ca03c-134">String</span></span>|<span data-ttu-id="ca03c-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ca03c-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ca03c-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca03c-136">Response</span></span>
<span data-ttu-id="ca03c-137">В случае успеха эта функция возвращает `200 OK` код отклика и коллекцию [девицеманажементсеттингкомпарисон](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca03c-137">If successful, this function returns a `200 OK` response code and a [deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca03c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="ca03c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca03c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca03c-139">Request</span></span>
<span data-ttu-id="ca03c-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca03c-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/compare(templateId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="ca03c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca03c-141">Response</span></span>
<span data-ttu-id="ca03c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca03c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 364

{
  "value": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingComparison",
      "id": "Id value",
      "displayName": "Display Name value",
      "definitionId": "Definition Id value",
      "currentValueJson": "Current Value Json value",
      "newValueJson": "New Value Json value",
      "comparisonResult": "equal"
    }
  ]
}
```






