---
title: Функция Compare
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 624857073e52c15323ff11336fcbfc6aa265b80b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381495"
---
# <a name="compare-function"></a><span data-ttu-id="4b31e-103">Функция Compare</span><span class="sxs-lookup"><span data-stu-id="4b31e-103">compare function</span></span>

<span data-ttu-id="4b31e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b31e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b31e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b31e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b31e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b31e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b31e-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4b31e-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b31e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4b31e-108">Prerequisites</span></span>
<span data-ttu-id="4b31e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b31e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b31e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b31e-111">Permission type</span></span>|<span data-ttu-id="4b31e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b31e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b31e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b31e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b31e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b31e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4b31e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b31e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b31e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b31e-116">Not supported.</span></span>|
|<span data-ttu-id="4b31e-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="4b31e-117">Application</span></span>|<span data-ttu-id="4b31e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b31e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b31e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b31e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/compare
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}/compare
```

## <a name="request-headers"></a><span data-ttu-id="4b31e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4b31e-120">Request headers</span></span>
|<span data-ttu-id="4b31e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b31e-121">Header</span></span>|<span data-ttu-id="4b31e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4b31e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b31e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b31e-123">Authorization</span></span>|<span data-ttu-id="4b31e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b31e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b31e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4b31e-125">Accept</span></span>|<span data-ttu-id="4b31e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b31e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b31e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b31e-127">Request body</span></span>
<span data-ttu-id="4b31e-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="4b31e-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="4b31e-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="4b31e-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4b31e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b31e-130">Property</span></span>|<span data-ttu-id="4b31e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4b31e-131">Type</span></span>|<span data-ttu-id="4b31e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4b31e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b31e-133">templateId</span><span class="sxs-lookup"><span data-stu-id="4b31e-133">templateId</span></span>|<span data-ttu-id="4b31e-134">String</span><span class="sxs-lookup"><span data-stu-id="4b31e-134">String</span></span>|<span data-ttu-id="4b31e-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4b31e-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4b31e-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b31e-136">Response</span></span>
<span data-ttu-id="4b31e-137">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [девицеманажементсеттингкомпарисон](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b31e-137">If successful, this function returns a `200 OK` response code and a [deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b31e-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4b31e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b31e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b31e-139">Request</span></span>
<span data-ttu-id="4b31e-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b31e-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/compare(templateId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="4b31e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b31e-141">Response</span></span>
<span data-ttu-id="4b31e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b31e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



