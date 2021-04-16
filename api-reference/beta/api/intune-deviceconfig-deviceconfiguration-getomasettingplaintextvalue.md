---
title: функция getOmaSettingPlainTextValue
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7cd6e09c56d96c344ba8ba2fc4c29202dea63cd3
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868821"
---
# <a name="getomasettingplaintextvalue-function"></a><span data-ttu-id="dc02b-103">функция getOmaSettingPlainTextValue</span><span class="sxs-lookup"><span data-stu-id="dc02b-103">getOmaSettingPlainTextValue function</span></span>

<span data-ttu-id="dc02b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc02b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc02b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc02b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc02b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc02b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc02b-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dc02b-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc02b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dc02b-108">Prerequisites</span></span>
<span data-ttu-id="dc02b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc02b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc02b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc02b-111">Permission type</span></span>|<span data-ttu-id="dc02b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc02b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc02b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc02b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc02b-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc02b-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dc02b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc02b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc02b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc02b-116">Not supported.</span></span>|
|<span data-ttu-id="dc02b-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="dc02b-117">Application</span></span>|<span data-ttu-id="dc02b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc02b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc02b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc02b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/getOmaSettingPlainTextValue
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/getOmaSettingPlainTextValue
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/getOmaSettingPlainTextValue
```

## <a name="request-headers"></a><span data-ttu-id="dc02b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dc02b-120">Request headers</span></span>
|<span data-ttu-id="dc02b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc02b-121">Header</span></span>|<span data-ttu-id="dc02b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dc02b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc02b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc02b-123">Authorization</span></span>|<span data-ttu-id="dc02b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc02b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc02b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dc02b-125">Accept</span></span>|<span data-ttu-id="dc02b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc02b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc02b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc02b-127">Request body</span></span>
<span data-ttu-id="dc02b-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="dc02b-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="dc02b-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="dc02b-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="dc02b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc02b-130">Property</span></span>|<span data-ttu-id="dc02b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dc02b-131">Type</span></span>|<span data-ttu-id="dc02b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dc02b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc02b-133">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="dc02b-133">secretReferenceValueId</span></span>|<span data-ttu-id="dc02b-134">String</span><span class="sxs-lookup"><span data-stu-id="dc02b-134">String</span></span>|<span data-ttu-id="dc02b-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dc02b-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dc02b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc02b-136">Response</span></span>
<span data-ttu-id="dc02b-137">В случае успешной работы эта функция возвращает код отклика и `200 OK` строку в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dc02b-137">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc02b-138">Пример</span><span class="sxs-lookup"><span data-stu-id="dc02b-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc02b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc02b-139">Request</span></span>
<span data-ttu-id="dc02b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc02b-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/getOmaSettingPlainTextValue(secretReferenceValueId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="dc02b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc02b-141">Response</span></span>
<span data-ttu-id="dc02b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc02b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 57

{
  "value": "Get Oma Setting Plain Text Value value"
}
```




