---
title: Функция getAuditActivityTypes
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6a6c97d1604a48f3eeee7fb5d7ee4e5985043109
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35959525"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="6d649-103">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="6d649-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="6d649-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d649-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d649-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d649-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d649-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6d649-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d649-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6d649-107">Prerequisites</span></span>
<span data-ttu-id="6d649-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d649-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d649-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d649-110">Permission type</span></span>|<span data-ttu-id="6d649-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d649-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d649-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d649-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6d649-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d649-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6d649-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d649-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d649-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d649-115">Not supported.</span></span>|
|<span data-ttu-id="6d649-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d649-116">Application</span></span>|<span data-ttu-id="6d649-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d649-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d649-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d649-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="6d649-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d649-119">Request headers</span></span>
|<span data-ttu-id="6d649-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d649-120">Header</span></span>|<span data-ttu-id="6d649-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6d649-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d649-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d649-122">Authorization</span></span>|<span data-ttu-id="6d649-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d649-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d649-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6d649-124">Accept</span></span>|<span data-ttu-id="6d649-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6d649-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d649-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6d649-126">Request body</span></span>
<span data-ttu-id="6d649-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="6d649-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="6d649-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="6d649-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6d649-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d649-129">Property</span></span>|<span data-ttu-id="6d649-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6d649-130">Type</span></span>|<span data-ttu-id="6d649-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6d649-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d649-132">category</span><span class="sxs-lookup"><span data-stu-id="6d649-132">category</span></span>|<span data-ttu-id="6d649-133">String</span><span class="sxs-lookup"><span data-stu-id="6d649-133">String</span></span>|<span data-ttu-id="6d649-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6d649-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6d649-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d649-135">Response</span></span>
<span data-ttu-id="6d649-136">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6d649-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d649-137">Пример</span><span class="sxs-lookup"><span data-stu-id="6d649-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d649-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d649-138">Request</span></span>
<span data-ttu-id="6d649-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d649-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="6d649-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d649-140">Response</span></span>
<span data-ttu-id="6d649-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d649-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





