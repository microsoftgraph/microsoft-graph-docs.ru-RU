---
title: Функция Compare
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 86607a33e92aac13c93941eb4290399011e8aa94
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49213190"
---
# <a name="compare-function"></a><span data-ttu-id="4e1dd-103">Функция Compare</span><span class="sxs-lookup"><span data-stu-id="4e1dd-103">compare function</span></span>

<span data-ttu-id="4e1dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e1dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e1dd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e1dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e1dd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e1dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e1dd-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4e1dd-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e1dd-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4e1dd-108">Prerequisites</span></span>
<span data-ttu-id="4e1dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e1dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e1dd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e1dd-111">Permission type</span></span>|<span data-ttu-id="4e1dd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e1dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e1dd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e1dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e1dd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e1dd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4e1dd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e1dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e1dd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e1dd-116">Not supported.</span></span>|
|<span data-ttu-id="4e1dd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4e1dd-117">Application</span></span>|<span data-ttu-id="4e1dd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e1dd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e1dd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e1dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/compare
```

## <a name="request-headers"></a><span data-ttu-id="4e1dd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4e1dd-120">Request headers</span></span>
|<span data-ttu-id="4e1dd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e1dd-121">Header</span></span>|<span data-ttu-id="4e1dd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4e1dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e1dd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e1dd-123">Authorization</span></span>|<span data-ttu-id="4e1dd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e1dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e1dd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e1dd-125">Accept</span></span>|<span data-ttu-id="4e1dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e1dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e1dd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e1dd-127">Request body</span></span>
<span data-ttu-id="4e1dd-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="4e1dd-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="4e1dd-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="4e1dd-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4e1dd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e1dd-130">Property</span></span>|<span data-ttu-id="4e1dd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4e1dd-131">Type</span></span>|<span data-ttu-id="4e1dd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4e1dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e1dd-133">templateId</span><span class="sxs-lookup"><span data-stu-id="4e1dd-133">templateId</span></span>|<span data-ttu-id="4e1dd-134">String</span><span class="sxs-lookup"><span data-stu-id="4e1dd-134">String</span></span>|<span data-ttu-id="4e1dd-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4e1dd-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4e1dd-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e1dd-136">Response</span></span>
<span data-ttu-id="4e1dd-137">В случае успеха эта функция возвращает `200 OK` код отклика и коллекцию [девицеманажементсеттингкомпарисон](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e1dd-137">If successful, this function returns a `200 OK` response code and a [deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e1dd-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4e1dd-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e1dd-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e1dd-139">Request</span></span>
<span data-ttu-id="4e1dd-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e1dd-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/compare(templateId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="4e1dd-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e1dd-141">Response</span></span>
<span data-ttu-id="4e1dd-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e1dd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




