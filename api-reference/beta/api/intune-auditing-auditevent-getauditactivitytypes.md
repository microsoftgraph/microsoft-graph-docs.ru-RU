---
title: Функция getAuditActivityTypes
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 176a46d72c60853f35eb0a6f300627f0f8bb02a5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760587"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="7498d-103">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="7498d-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="7498d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7498d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7498d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7498d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7498d-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7498d-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7498d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7498d-107">Prerequisites</span></span>
<span data-ttu-id="7498d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7498d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7498d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7498d-110">Permission type</span></span>|<span data-ttu-id="7498d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7498d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7498d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7498d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7498d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7498d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7498d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7498d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7498d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7498d-115">Not supported.</span></span>|
|<span data-ttu-id="7498d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7498d-116">Application</span></span>|<span data-ttu-id="7498d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7498d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7498d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7498d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="7498d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7498d-119">Request headers</span></span>
|<span data-ttu-id="7498d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7498d-120">Header</span></span>|<span data-ttu-id="7498d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7498d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7498d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7498d-122">Authorization</span></span>|<span data-ttu-id="7498d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7498d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7498d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7498d-124">Accept</span></span>|<span data-ttu-id="7498d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7498d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7498d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7498d-126">Request body</span></span>
<span data-ttu-id="7498d-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="7498d-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7498d-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="7498d-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7498d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7498d-129">Property</span></span>|<span data-ttu-id="7498d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7498d-130">Type</span></span>|<span data-ttu-id="7498d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7498d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7498d-132">category</span><span class="sxs-lookup"><span data-stu-id="7498d-132">category</span></span>|<span data-ttu-id="7498d-133">String</span><span class="sxs-lookup"><span data-stu-id="7498d-133">String</span></span>|<span data-ttu-id="7498d-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7498d-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7498d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="7498d-135">Response</span></span>
<span data-ttu-id="7498d-136">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7498d-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7498d-137">Пример</span><span class="sxs-lookup"><span data-stu-id="7498d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="7498d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="7498d-138">Request</span></span>
<span data-ttu-id="7498d-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7498d-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="7498d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7498d-140">Response</span></span>
<span data-ttu-id="7498d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7498d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




