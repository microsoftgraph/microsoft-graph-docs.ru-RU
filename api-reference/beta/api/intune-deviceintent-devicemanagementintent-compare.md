---
title: сравнение функции
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fe4a73d3f1ea449027a193c8de4e3fc8a3c2ee20
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128952"
---
# <a name="compare-function"></a><span data-ttu-id="8c6af-103">сравнение функции</span><span class="sxs-lookup"><span data-stu-id="8c6af-103">compare function</span></span>

<span data-ttu-id="8c6af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c6af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c6af-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c6af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c6af-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c6af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c6af-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c6af-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c6af-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8c6af-108">Prerequisites</span></span>
<span data-ttu-id="8c6af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c6af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c6af-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c6af-111">Permission type</span></span>|<span data-ttu-id="8c6af-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c6af-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c6af-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c6af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c6af-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c6af-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8c6af-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c6af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c6af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c6af-116">Not supported.</span></span>|
|<span data-ttu-id="8c6af-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8c6af-117">Application</span></span>|<span data-ttu-id="8c6af-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c6af-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c6af-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c6af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/compare
```

## <a name="request-headers"></a><span data-ttu-id="8c6af-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8c6af-120">Request headers</span></span>
|<span data-ttu-id="8c6af-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c6af-121">Header</span></span>|<span data-ttu-id="8c6af-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8c6af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c6af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c6af-123">Authorization</span></span>|<span data-ttu-id="8c6af-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c6af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c6af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8c6af-125">Accept</span></span>|<span data-ttu-id="8c6af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c6af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c6af-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c6af-127">Request body</span></span>
<span data-ttu-id="8c6af-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="8c6af-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="8c6af-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="8c6af-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="8c6af-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c6af-130">Property</span></span>|<span data-ttu-id="8c6af-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8c6af-131">Type</span></span>|<span data-ttu-id="8c6af-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8c6af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c6af-133">templateId</span><span class="sxs-lookup"><span data-stu-id="8c6af-133">templateId</span></span>|<span data-ttu-id="8c6af-134">String</span><span class="sxs-lookup"><span data-stu-id="8c6af-134">String</span></span>|<span data-ttu-id="8c6af-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c6af-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8c6af-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c6af-136">Response</span></span>
<span data-ttu-id="8c6af-137">В случае успешного выполнения эта функция возвращает код отклика и `200 OK` [коллекцию deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8c6af-137">If successful, this function returns a `200 OK` response code and a [deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c6af-138">Пример</span><span class="sxs-lookup"><span data-stu-id="8c6af-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c6af-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c6af-139">Request</span></span>
<span data-ttu-id="8c6af-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c6af-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/compare(templateId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="8c6af-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c6af-141">Response</span></span>
<span data-ttu-id="8c6af-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c6af-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




