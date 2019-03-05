---
title: Функция getAuditActivityTypes
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e06f1fda065fc03fbe8ed009feb7bea77bca5f05
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256254"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="1e682-103">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="1e682-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="1e682-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1e682-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e682-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1e682-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e682-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1e682-106">Prerequisites</span></span>
<span data-ttu-id="1e682-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1e682-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1e682-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e682-109">Permission type</span></span>|<span data-ttu-id="1e682-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e682-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e682-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e682-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1e682-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e682-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1e682-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e682-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e682-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e682-114">Not supported.</span></span>|
|<span data-ttu-id="1e682-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e682-115">Application</span></span>|<span data-ttu-id="1e682-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e682-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e682-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e682-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="1e682-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e682-118">Request headers</span></span>
|<span data-ttu-id="1e682-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1e682-119">Header</span></span>|<span data-ttu-id="1e682-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1e682-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e682-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1e682-121">Authorization</span></span>|<span data-ttu-id="1e682-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1e682-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e682-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1e682-123">Accept</span></span>|<span data-ttu-id="1e682-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1e682-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e682-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e682-125">Request body</span></span>
<span data-ttu-id="1e682-126">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="1e682-126">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="1e682-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="1e682-127">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="1e682-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e682-128">Property</span></span>|<span data-ttu-id="1e682-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1e682-129">Type</span></span>|<span data-ttu-id="1e682-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1e682-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e682-131">category</span><span class="sxs-lookup"><span data-stu-id="1e682-131">category</span></span>|<span data-ttu-id="1e682-132">String</span><span class="sxs-lookup"><span data-stu-id="1e682-132">String</span></span>|<span data-ttu-id="1e682-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1e682-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1e682-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1e682-134">Response</span></span>
<span data-ttu-id="1e682-135">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1e682-135">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e682-136">Пример</span><span class="sxs-lookup"><span data-stu-id="1e682-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e682-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e682-137">Request</span></span>
<span data-ttu-id="1e682-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e682-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="1e682-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="1e682-139">Response</span></span>
<span data-ttu-id="1e682-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1e682-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



