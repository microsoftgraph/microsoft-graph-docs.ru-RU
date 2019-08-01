---
title: Функция getAuditActivityTypes
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 45ba5a7cf0280e5f54fbbfa00166521ff50e9354
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015909"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="7ba13-103">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="7ba13-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="7ba13-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ba13-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ba13-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7ba13-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ba13-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7ba13-106">Prerequisites</span></span>
<span data-ttu-id="7ba13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ba13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ba13-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ba13-109">Permission type</span></span>|<span data-ttu-id="7ba13-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ba13-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ba13-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ba13-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7ba13-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ba13-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7ba13-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ba13-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ba13-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ba13-114">Not supported.</span></span>|
|<span data-ttu-id="7ba13-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ba13-115">Application</span></span>|<span data-ttu-id="7ba13-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ba13-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ba13-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ba13-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="7ba13-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ba13-118">Request headers</span></span>
|<span data-ttu-id="7ba13-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ba13-119">Header</span></span>|<span data-ttu-id="7ba13-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7ba13-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ba13-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ba13-121">Authorization</span></span>|<span data-ttu-id="7ba13-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ba13-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ba13-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7ba13-123">Accept</span></span>|<span data-ttu-id="7ba13-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7ba13-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ba13-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7ba13-125">Request body</span></span>
<span data-ttu-id="7ba13-126">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="7ba13-126">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7ba13-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="7ba13-127">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7ba13-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ba13-128">Property</span></span>|<span data-ttu-id="7ba13-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7ba13-129">Type</span></span>|<span data-ttu-id="7ba13-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7ba13-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ba13-131">category</span><span class="sxs-lookup"><span data-stu-id="7ba13-131">category</span></span>|<span data-ttu-id="7ba13-132">String</span><span class="sxs-lookup"><span data-stu-id="7ba13-132">String</span></span>|<span data-ttu-id="7ba13-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7ba13-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7ba13-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ba13-134">Response</span></span>
<span data-ttu-id="7ba13-135">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7ba13-135">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ba13-136">Пример</span><span class="sxs-lookup"><span data-stu-id="7ba13-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ba13-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ba13-137">Request</span></span>
<span data-ttu-id="7ba13-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ba13-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="7ba13-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ba13-139">Response</span></span>
<span data-ttu-id="7ba13-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ba13-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



