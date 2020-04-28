---
title: Функция getAuditActivityTypes
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac5aba223fbac4face840e89ae417650ae19a096
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43392980"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="f669a-103">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="f669a-103">getAuditActivityTypes function</span></span>

<span data-ttu-id="f669a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f669a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f669a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f669a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f669a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f669a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f669a-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f669a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f669a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f669a-108">Prerequisites</span></span>
<span data-ttu-id="f669a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f669a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f669a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f669a-111">Permission type</span></span>|<span data-ttu-id="f669a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f669a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f669a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f669a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f669a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f669a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f669a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f669a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f669a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f669a-116">Not supported.</span></span>|
|<span data-ttu-id="f669a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f669a-117">Application</span></span>|<span data-ttu-id="f669a-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f669a-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f669a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f669a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="f669a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f669a-120">Request headers</span></span>
|<span data-ttu-id="f669a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f669a-121">Header</span></span>|<span data-ttu-id="f669a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f669a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f669a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f669a-123">Authorization</span></span>|<span data-ttu-id="f669a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f669a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f669a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f669a-125">Accept</span></span>|<span data-ttu-id="f669a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f669a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f669a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f669a-127">Request body</span></span>
<span data-ttu-id="f669a-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="f669a-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="f669a-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="f669a-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="f669a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f669a-130">Property</span></span>|<span data-ttu-id="f669a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f669a-131">Type</span></span>|<span data-ttu-id="f669a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f669a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f669a-133">category</span><span class="sxs-lookup"><span data-stu-id="f669a-133">category</span></span>|<span data-ttu-id="f669a-134">String</span><span class="sxs-lookup"><span data-stu-id="f669a-134">String</span></span>|<span data-ttu-id="f669a-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f669a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f669a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f669a-136">Response</span></span>
<span data-ttu-id="f669a-137">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f669a-137">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f669a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f669a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f669a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f669a-139">Request</span></span>
<span data-ttu-id="f669a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f669a-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="f669a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f669a-141">Response</span></span>
<span data-ttu-id="f669a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f669a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



