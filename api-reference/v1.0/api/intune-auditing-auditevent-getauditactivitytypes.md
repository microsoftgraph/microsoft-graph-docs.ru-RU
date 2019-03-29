---
title: Функция getAuditActivityTypes
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3541b8ff61b0f48f4461a87559819f06d0e3cebe
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972251"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="8b9fc-103">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="8b9fc-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="8b9fc-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b9fc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b9fc-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8b9fc-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b9fc-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8b9fc-106">Prerequisites</span></span>
<span data-ttu-id="8b9fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b9fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b9fc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b9fc-109">Permission type</span></span>|<span data-ttu-id="8b9fc-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b9fc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b9fc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b9fc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8b9fc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b9fc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8b9fc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b9fc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b9fc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b9fc-114">Not supported.</span></span>|
|<span data-ttu-id="8b9fc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b9fc-115">Application</span></span>|<span data-ttu-id="8b9fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b9fc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b9fc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b9fc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="8b9fc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b9fc-118">Request headers</span></span>
|<span data-ttu-id="8b9fc-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b9fc-119">Header</span></span>|<span data-ttu-id="8b9fc-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8b9fc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b9fc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b9fc-121">Authorization</span></span>|<span data-ttu-id="8b9fc-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b9fc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b9fc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8b9fc-123">Accept</span></span>|<span data-ttu-id="8b9fc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8b9fc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b9fc-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b9fc-125">Request body</span></span>
<span data-ttu-id="8b9fc-126">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="8b9fc-126">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="8b9fc-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="8b9fc-127">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="8b9fc-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b9fc-128">Property</span></span>|<span data-ttu-id="8b9fc-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8b9fc-129">Type</span></span>|<span data-ttu-id="8b9fc-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8b9fc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b9fc-131">category</span><span class="sxs-lookup"><span data-stu-id="8b9fc-131">category</span></span>|<span data-ttu-id="8b9fc-132">String</span><span class="sxs-lookup"><span data-stu-id="8b9fc-132">String</span></span>|<span data-ttu-id="8b9fc-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8b9fc-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8b9fc-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b9fc-134">Response</span></span>
<span data-ttu-id="8b9fc-135">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8b9fc-135">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b9fc-136">Пример</span><span class="sxs-lookup"><span data-stu-id="8b9fc-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b9fc-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b9fc-137">Request</span></span>
<span data-ttu-id="8b9fc-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b9fc-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="8b9fc-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b9fc-139">Response</span></span>
<span data-ttu-id="8b9fc-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b9fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



