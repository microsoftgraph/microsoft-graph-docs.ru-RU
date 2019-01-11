---
title: Функция getAuditActivityTypes
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e750db76d6c022faf3149cc24d43a448ca235eed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889504"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="1bdba-103">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="1bdba-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="1bdba-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1bdba-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1bdba-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1bdba-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1bdba-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1bdba-106">Prerequisites</span></span>
<span data-ttu-id="1bdba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bdba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bdba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bdba-109">Permission type</span></span>|<span data-ttu-id="1bdba-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bdba-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bdba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bdba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1bdba-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bdba-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1bdba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bdba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bdba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bdba-114">Not supported.</span></span>|
|<span data-ttu-id="1bdba-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1bdba-115">Application</span></span>|<span data-ttu-id="1bdba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bdba-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bdba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bdba-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="1bdba-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bdba-118">Request headers</span></span>
|<span data-ttu-id="1bdba-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1bdba-119">Header</span></span>|<span data-ttu-id="1bdba-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1bdba-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bdba-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bdba-121">Authorization</span></span>|<span data-ttu-id="1bdba-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1bdba-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bdba-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1bdba-123">Accept</span></span>|<span data-ttu-id="1bdba-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1bdba-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bdba-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1bdba-125">Request body</span></span>
<span data-ttu-id="1bdba-126">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="1bdba-126">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="1bdba-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="1bdba-127">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="1bdba-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bdba-128">Property</span></span>|<span data-ttu-id="1bdba-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1bdba-129">Type</span></span>|<span data-ttu-id="1bdba-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1bdba-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bdba-131">category</span><span class="sxs-lookup"><span data-stu-id="1bdba-131">category</span></span>|<span data-ttu-id="1bdba-132">String</span><span class="sxs-lookup"><span data-stu-id="1bdba-132">String</span></span>|<span data-ttu-id="1bdba-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1bdba-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1bdba-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1bdba-134">Response</span></span>
<span data-ttu-id="1bdba-135">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1bdba-135">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bdba-136">Пример</span><span class="sxs-lookup"><span data-stu-id="1bdba-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="1bdba-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bdba-137">Request</span></span>
<span data-ttu-id="1bdba-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bdba-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="1bdba-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="1bdba-139">Response</span></span>
<span data-ttu-id="1bdba-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1bdba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



