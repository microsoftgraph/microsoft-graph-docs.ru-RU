---
title: Функция Compare
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6afc3a4de32c9cb1d594e1354a7087c042ca7905
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37189055"
---
# <a name="compare-function"></a><span data-ttu-id="e7ed3-103">Функция Compare</span><span class="sxs-lookup"><span data-stu-id="e7ed3-103">compare function</span></span>

> <span data-ttu-id="e7ed3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7ed3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7ed3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7ed3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7ed3-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e7ed3-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7ed3-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e7ed3-107">Prerequisites</span></span>
<span data-ttu-id="e7ed3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7ed3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7ed3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7ed3-110">Permission type</span></span>|<span data-ttu-id="e7ed3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7ed3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7ed3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7ed3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7ed3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7ed3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e7ed3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7ed3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7ed3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7ed3-115">Not supported.</span></span>|
|<span data-ttu-id="e7ed3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7ed3-116">Application</span></span>|<span data-ttu-id="e7ed3-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7ed3-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7ed3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7ed3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/compare
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}/compare
```

## <a name="request-headers"></a><span data-ttu-id="e7ed3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7ed3-119">Request headers</span></span>
|<span data-ttu-id="e7ed3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7ed3-120">Header</span></span>|<span data-ttu-id="e7ed3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e7ed3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7ed3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e7ed3-122">Authorization</span></span>|<span data-ttu-id="e7ed3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7ed3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7ed3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e7ed3-124">Accept</span></span>|<span data-ttu-id="e7ed3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7ed3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7ed3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e7ed3-126">Request body</span></span>
<span data-ttu-id="e7ed3-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="e7ed3-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e7ed3-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="e7ed3-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e7ed3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7ed3-129">Property</span></span>|<span data-ttu-id="e7ed3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e7ed3-130">Type</span></span>|<span data-ttu-id="e7ed3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e7ed3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7ed3-132">templateId</span><span class="sxs-lookup"><span data-stu-id="e7ed3-132">templateId</span></span>|<span data-ttu-id="e7ed3-133">String</span><span class="sxs-lookup"><span data-stu-id="e7ed3-133">String</span></span>|<span data-ttu-id="e7ed3-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e7ed3-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e7ed3-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7ed3-135">Response</span></span>
<span data-ttu-id="e7ed3-136">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [девицеманажементсеттингкомпарисон](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e7ed3-136">If successful, this function returns a `200 OK` response code and a [deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7ed3-137">Пример</span><span class="sxs-lookup"><span data-stu-id="e7ed3-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7ed3-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7ed3-138">Request</span></span>
<span data-ttu-id="e7ed3-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7ed3-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/compare(templateId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e7ed3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7ed3-140">Response</span></span>
<span data-ttu-id="e7ed3-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e7ed3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




