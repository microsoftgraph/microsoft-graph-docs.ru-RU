---
title: Функция getAuditActivityTypes
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3a8151169f1173594be3697e721e89556416e718
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952680"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="cff34-103">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="cff34-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="cff34-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cff34-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cff34-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cff34-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cff34-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="cff34-106">Prerequisites</span></span>
<span data-ttu-id="cff34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cff34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cff34-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cff34-109">Permission type</span></span>|<span data-ttu-id="cff34-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cff34-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cff34-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cff34-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cff34-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cff34-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cff34-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cff34-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cff34-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cff34-114">Not supported.</span></span>|
|<span data-ttu-id="cff34-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cff34-115">Application</span></span>|<span data-ttu-id="cff34-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cff34-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cff34-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cff34-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="cff34-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cff34-118">Request headers</span></span>
|<span data-ttu-id="cff34-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cff34-119">Header</span></span>|<span data-ttu-id="cff34-120">Значение</span><span class="sxs-lookup"><span data-stu-id="cff34-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cff34-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cff34-121">Authorization</span></span>|<span data-ttu-id="cff34-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cff34-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cff34-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cff34-123">Accept</span></span>|<span data-ttu-id="cff34-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cff34-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cff34-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cff34-125">Request body</span></span>
<span data-ttu-id="cff34-126">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="cff34-126">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="cff34-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="cff34-127">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="cff34-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="cff34-128">Property</span></span>|<span data-ttu-id="cff34-129">Тип</span><span class="sxs-lookup"><span data-stu-id="cff34-129">Type</span></span>|<span data-ttu-id="cff34-130">Описание</span><span class="sxs-lookup"><span data-stu-id="cff34-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cff34-131">category</span><span class="sxs-lookup"><span data-stu-id="cff34-131">category</span></span>|<span data-ttu-id="cff34-132">String</span><span class="sxs-lookup"><span data-stu-id="cff34-132">String</span></span>|<span data-ttu-id="cff34-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cff34-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cff34-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="cff34-134">Response</span></span>
<span data-ttu-id="cff34-135">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cff34-135">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cff34-136">Пример</span><span class="sxs-lookup"><span data-stu-id="cff34-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="cff34-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="cff34-137">Request</span></span>
<span data-ttu-id="cff34-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cff34-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="cff34-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="cff34-139">Response</span></span>
<span data-ttu-id="cff34-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cff34-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



