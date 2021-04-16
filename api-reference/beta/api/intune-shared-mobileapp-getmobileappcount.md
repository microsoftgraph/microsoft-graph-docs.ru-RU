---
title: функция getMobileAppCount
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e6b975137bff474366f083bb880e7ebaca33c2f8
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863838"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="bd946-103">функция getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="bd946-103">getMobileAppCount function</span></span>

<span data-ttu-id="bd946-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd946-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd946-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd946-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd946-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd946-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd946-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="bd946-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd946-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bd946-108">Prerequisites</span></span>
<span data-ttu-id="bd946-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd946-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd946-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd946-111">Permission type</span></span>|<span data-ttu-id="bd946-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd946-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd946-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd946-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bd946-114">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="bd946-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="bd946-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd946-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bd946-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd946-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd946-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd946-117">Not supported.</span></span>|
|<span data-ttu-id="bd946-118">Для приложения</span><span class="sxs-lookup"><span data-stu-id="bd946-118">Application</span></span>||
| <span data-ttu-id="bd946-119">&nbsp; &nbsp; **Приложения**</span><span class="sxs-lookup"><span data-stu-id="bd946-119">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="bd946-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd946-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd946-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd946-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="bd946-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bd946-122">Request headers</span></span>
|<span data-ttu-id="bd946-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd946-123">Header</span></span>|<span data-ttu-id="bd946-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bd946-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd946-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd946-125">Authorization</span></span>|<span data-ttu-id="bd946-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd946-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd946-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bd946-127">Accept</span></span>|<span data-ttu-id="bd946-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bd946-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd946-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd946-129">Request body</span></span>
<span data-ttu-id="bd946-130">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="bd946-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="bd946-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="bd946-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="bd946-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd946-132">Property</span></span>|<span data-ttu-id="bd946-133">Тип</span><span class="sxs-lookup"><span data-stu-id="bd946-133">Type</span></span>|<span data-ttu-id="bd946-134">Описание</span><span class="sxs-lookup"><span data-stu-id="bd946-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd946-135">status</span><span class="sxs-lookup"><span data-stu-id="bd946-135">status</span></span>|<span data-ttu-id="bd946-136">String</span><span class="sxs-lookup"><span data-stu-id="bd946-136">String</span></span>|<span data-ttu-id="bd946-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="bd946-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bd946-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="bd946-138">Response</span></span>
<span data-ttu-id="bd946-139">В случае успешной работы эта функция возвращает код `200 OK` отклика и int64 в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bd946-139">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd946-140">Пример</span><span class="sxs-lookup"><span data-stu-id="bd946-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd946-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd946-141">Request</span></span>
<span data-ttu-id="bd946-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd946-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="bd946-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd946-143">Response</span></span>
<span data-ttu-id="bd946-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd946-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```







