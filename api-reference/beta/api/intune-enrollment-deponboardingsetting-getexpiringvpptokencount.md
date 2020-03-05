---
title: Функция Жетекспирингвпптокенкаунт
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2fcf2cd678818d9770f833e3ad7e4a14b0100a5d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467160"
---
# <a name="getexpiringvpptokencount-function"></a><span data-ttu-id="db34c-103">Функция Жетекспирингвпптокенкаунт</span><span class="sxs-lookup"><span data-stu-id="db34c-103">getExpiringVppTokenCount function</span></span>

<span data-ttu-id="db34c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="db34c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db34c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db34c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db34c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db34c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db34c-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="db34c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db34c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="db34c-108">Prerequisites</span></span>
<span data-ttu-id="db34c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db34c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db34c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db34c-111">Permission type</span></span>|<span data-ttu-id="db34c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="db34c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db34c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db34c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db34c-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="db34c-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="db34c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db34c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db34c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db34c-116">Not supported.</span></span>|
|<span data-ttu-id="db34c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db34c-117">Application</span></span>|<span data-ttu-id="db34c-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="db34c-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db34c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db34c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/getExpiringVppTokenCount
```

## <a name="request-headers"></a><span data-ttu-id="db34c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="db34c-120">Request headers</span></span>
|<span data-ttu-id="db34c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="db34c-121">Header</span></span>|<span data-ttu-id="db34c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="db34c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db34c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db34c-123">Authorization</span></span>|<span data-ttu-id="db34c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db34c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db34c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="db34c-125">Accept</span></span>|<span data-ttu-id="db34c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db34c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db34c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db34c-127">Request body</span></span>
<span data-ttu-id="db34c-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="db34c-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="db34c-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="db34c-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="db34c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="db34c-130">Property</span></span>|<span data-ttu-id="db34c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="db34c-131">Type</span></span>|<span data-ttu-id="db34c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="db34c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db34c-133">експирингбефоредатетиме</span><span class="sxs-lookup"><span data-stu-id="db34c-133">expiringBeforeDateTime</span></span>|<span data-ttu-id="db34c-134">String</span><span class="sxs-lookup"><span data-stu-id="db34c-134">String</span></span>|<span data-ttu-id="db34c-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="db34c-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="db34c-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="db34c-136">Response</span></span>
<span data-ttu-id="db34c-137">В случае успеха эта функция возвращает код `200 OK` отклика и значение Int32 в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="db34c-137">If successful, this function returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db34c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="db34c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="db34c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="db34c-139">Request</span></span>
<span data-ttu-id="db34c-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db34c-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/getExpiringVppTokenCount(expiringBeforeDateTime='parameterValue')
```

### <a name="response"></a><span data-ttu-id="db34c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="db34c-141">Response</span></span>
<span data-ttu-id="db34c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db34c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 8
}
```





