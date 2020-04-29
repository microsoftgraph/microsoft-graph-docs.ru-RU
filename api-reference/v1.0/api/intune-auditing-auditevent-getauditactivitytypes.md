---
title: Функция getAuditActivityTypes
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 57f3af7dc556f05eeecd7dbb395152f923b41e11
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464389"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="d5878-103">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="d5878-103">getAuditActivityTypes function</span></span>

<span data-ttu-id="d5878-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5878-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5878-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5878-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5878-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d5878-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5878-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d5878-107">Prerequisites</span></span>
<span data-ttu-id="d5878-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5878-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5878-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5878-110">Permission type</span></span>|<span data-ttu-id="d5878-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5878-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5878-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5878-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d5878-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5878-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d5878-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5878-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5878-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5878-115">Not supported.</span></span>|
|<span data-ttu-id="d5878-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5878-116">Application</span></span>|<span data-ttu-id="d5878-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5878-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5878-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5878-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="d5878-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d5878-119">Request headers</span></span>
|<span data-ttu-id="d5878-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5878-120">Header</span></span>|<span data-ttu-id="d5878-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d5878-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5878-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5878-122">Authorization</span></span>|<span data-ttu-id="d5878-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5878-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5878-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d5878-124">Accept</span></span>|<span data-ttu-id="d5878-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d5878-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5878-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d5878-126">Request body</span></span>
<span data-ttu-id="d5878-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="d5878-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d5878-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="d5878-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d5878-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5878-129">Property</span></span>|<span data-ttu-id="d5878-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d5878-130">Type</span></span>|<span data-ttu-id="d5878-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d5878-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5878-132">category</span><span class="sxs-lookup"><span data-stu-id="d5878-132">category</span></span>|<span data-ttu-id="d5878-133">String</span><span class="sxs-lookup"><span data-stu-id="d5878-133">String</span></span>|<span data-ttu-id="d5878-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d5878-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d5878-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="d5878-135">Response</span></span>
<span data-ttu-id="d5878-136">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d5878-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5878-137">Пример</span><span class="sxs-lookup"><span data-stu-id="d5878-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5878-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5878-138">Request</span></span>
<span data-ttu-id="d5878-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5878-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="d5878-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5878-140">Response</span></span>
<span data-ttu-id="d5878-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5878-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 61

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```






