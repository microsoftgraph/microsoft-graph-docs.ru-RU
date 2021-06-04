---
title: Функция verifyWindowsEnrollmentAutoDiscovery
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d53af260054dad19f07aa80c0b062bd5da9061c9
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732718"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="41370-103">Функция verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="41370-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

<span data-ttu-id="41370-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41370-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41370-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="41370-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41370-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="41370-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41370-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="41370-107">Prerequisites</span></span>
<span data-ttu-id="41370-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41370-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41370-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41370-110">Permission type</span></span>|<span data-ttu-id="41370-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="41370-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41370-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41370-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="41370-113">&nbsp;&nbsp;Onboarding</span><span class="sxs-lookup"><span data-stu-id="41370-113">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="41370-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41370-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="41370-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41370-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41370-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41370-116">Not supported.</span></span>|
|<span data-ttu-id="41370-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41370-117">Application</span></span>|<span data-ttu-id="41370-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41370-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41370-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41370-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="41370-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="41370-120">Request headers</span></span>
|<span data-ttu-id="41370-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41370-121">Header</span></span>|<span data-ttu-id="41370-122">Значение</span><span class="sxs-lookup"><span data-stu-id="41370-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41370-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="41370-123">Authorization</span></span>|<span data-ttu-id="41370-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41370-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41370-125">Accept</span><span class="sxs-lookup"><span data-stu-id="41370-125">Accept</span></span>|<span data-ttu-id="41370-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41370-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41370-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41370-127">Request body</span></span>
<span data-ttu-id="41370-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="41370-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="41370-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="41370-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="41370-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="41370-130">Property</span></span>|<span data-ttu-id="41370-131">Тип</span><span class="sxs-lookup"><span data-stu-id="41370-131">Type</span></span>|<span data-ttu-id="41370-132">Описание</span><span class="sxs-lookup"><span data-stu-id="41370-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41370-133">domainName</span><span class="sxs-lookup"><span data-stu-id="41370-133">domainName</span></span>|<span data-ttu-id="41370-134">String</span><span class="sxs-lookup"><span data-stu-id="41370-134">String</span></span>|<span data-ttu-id="41370-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="41370-135">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="41370-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="41370-136">Response</span></span>
<span data-ttu-id="41370-137">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="41370-137">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41370-138">Пример</span><span class="sxs-lookup"><span data-stu-id="41370-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="41370-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="41370-139">Request</span></span>
<span data-ttu-id="41370-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41370-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="41370-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="41370-141">Response</span></span>
<span data-ttu-id="41370-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="41370-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```









