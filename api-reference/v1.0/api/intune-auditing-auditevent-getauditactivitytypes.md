---
title: Функция getAuditActivityTypes
description: Н/Д
ms.openlocfilehash: 957ad384cf49ffbd361ed2e8904d66f94b75c8f8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027278"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="19644-103">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="19644-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="19644-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="19644-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19644-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="19644-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="19644-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="19644-106">Prerequisites</span></span>
<span data-ttu-id="19644-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19644-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19644-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19644-109">Permission type</span></span>|<span data-ttu-id="19644-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19644-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19644-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19644-111">Delegated (work or school account)</span></span>|<span data-ttu-id="19644-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="19644-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="19644-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19644-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19644-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19644-114">Not supported.</span></span>|
|<span data-ttu-id="19644-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19644-115">Application</span></span>|<span data-ttu-id="19644-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19644-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19644-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19644-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="19644-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19644-118">Request headers</span></span>
|<span data-ttu-id="19644-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19644-119">Header</span></span>|<span data-ttu-id="19644-120">Значение</span><span class="sxs-lookup"><span data-stu-id="19644-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19644-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="19644-121">Authorization</span></span>|<span data-ttu-id="19644-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="19644-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19644-123">Accept</span><span class="sxs-lookup"><span data-stu-id="19644-123">Accept</span></span>|<span data-ttu-id="19644-124">application/json</span><span class="sxs-lookup"><span data-stu-id="19644-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19644-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19644-125">Request body</span></span>
<span data-ttu-id="19644-126">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="19644-126">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="19644-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="19644-127">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="19644-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="19644-128">Property</span></span>|<span data-ttu-id="19644-129">Тип</span><span class="sxs-lookup"><span data-stu-id="19644-129">Type</span></span>|<span data-ttu-id="19644-130">Описание</span><span class="sxs-lookup"><span data-stu-id="19644-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19644-131">category</span><span class="sxs-lookup"><span data-stu-id="19644-131">category</span></span>|<span data-ttu-id="19644-132">String</span><span class="sxs-lookup"><span data-stu-id="19644-132">String</span></span>|<span data-ttu-id="19644-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="19644-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="19644-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="19644-134">Response</span></span>
<span data-ttu-id="19644-135">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="19644-135">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19644-136">Пример</span><span class="sxs-lookup"><span data-stu-id="19644-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="19644-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="19644-137">Request</span></span>
<span data-ttu-id="19644-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19644-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="19644-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="19644-139">Response</span></span>
<span data-ttu-id="19644-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="19644-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



