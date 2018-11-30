---
title: Функция verifyWindowsEnrollmentAutoDiscovery
description: Н/Д
ms.openlocfilehash: fa1eaba203b0d2fe77f1f0fb5bdb2d3fce5bb7f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081087"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="e9b39-103">Функция verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="e9b39-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="e9b39-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e9b39-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9b39-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9b39-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9b39-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e9b39-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9b39-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e9b39-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e9b39-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e9b39-108">Prerequisites</span></span>
<span data-ttu-id="e9b39-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9b39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9b39-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9b39-111">Permission type</span></span>|<span data-ttu-id="e9b39-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9b39-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9b39-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9b39-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9b39-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9b39-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e9b39-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9b39-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9b39-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9b39-116">Not supported.</span></span>|
|<span data-ttu-id="e9b39-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9b39-117">Application</span></span>|<span data-ttu-id="e9b39-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9b39-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9b39-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9b39-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="e9b39-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9b39-120">Request headers</span></span>
|<span data-ttu-id="e9b39-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9b39-121">Header</span></span>|<span data-ttu-id="e9b39-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e9b39-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9b39-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9b39-123">Authorization</span></span>|<span data-ttu-id="e9b39-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e9b39-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9b39-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9b39-125">Accept</span></span>|<span data-ttu-id="e9b39-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9b39-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9b39-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9b39-127">Request body</span></span>
<span data-ttu-id="e9b39-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="e9b39-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e9b39-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="e9b39-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e9b39-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9b39-130">Property</span></span>|<span data-ttu-id="e9b39-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e9b39-131">Type</span></span>|<span data-ttu-id="e9b39-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e9b39-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9b39-133">domainName</span><span class="sxs-lookup"><span data-stu-id="e9b39-133">domainName</span></span>|<span data-ttu-id="e9b39-134">String</span><span class="sxs-lookup"><span data-stu-id="e9b39-134">String</span></span>|<span data-ttu-id="e9b39-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e9b39-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e9b39-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9b39-136">Response</span></span>
<span data-ttu-id="e9b39-137">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e9b39-137">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9b39-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e9b39-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="e9b39-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9b39-139">Request</span></span>
<span data-ttu-id="e9b39-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9b39-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e9b39-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9b39-141">Response</span></span>
<span data-ttu-id="e9b39-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e9b39-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```





