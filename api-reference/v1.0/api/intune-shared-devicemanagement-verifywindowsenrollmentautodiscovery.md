---
title: Функция verifyWindowsEnrollmentAutoDiscovery
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8c2c81257dcc27791cd7db8883b60feeb3544c79
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361436"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="59a9f-103">Функция verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="59a9f-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="59a9f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="59a9f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59a9f-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="59a9f-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59a9f-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="59a9f-106">Prerequisites</span></span>
<span data-ttu-id="59a9f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59a9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59a9f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59a9f-109">Permission type</span></span>|<span data-ttu-id="59a9f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="59a9f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59a9f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59a9f-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="59a9f-112">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="59a9f-112">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="59a9f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59a9f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="59a9f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59a9f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59a9f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59a9f-115">Not supported.</span></span>|
|<span data-ttu-id="59a9f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59a9f-116">Application</span></span>|<span data-ttu-id="59a9f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59a9f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59a9f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59a9f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="59a9f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59a9f-119">Request headers</span></span>
|<span data-ttu-id="59a9f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59a9f-120">Header</span></span>|<span data-ttu-id="59a9f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="59a9f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59a9f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59a9f-122">Authorization</span></span>|<span data-ttu-id="59a9f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59a9f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59a9f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="59a9f-124">Accept</span></span>|<span data-ttu-id="59a9f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="59a9f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59a9f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59a9f-126">Request body</span></span>
<span data-ttu-id="59a9f-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="59a9f-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="59a9f-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="59a9f-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="59a9f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="59a9f-129">Property</span></span>|<span data-ttu-id="59a9f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="59a9f-130">Type</span></span>|<span data-ttu-id="59a9f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="59a9f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59a9f-132">domainName</span><span class="sxs-lookup"><span data-stu-id="59a9f-132">domainName</span></span>|<span data-ttu-id="59a9f-133">String</span><span class="sxs-lookup"><span data-stu-id="59a9f-133">String</span></span>|<span data-ttu-id="59a9f-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="59a9f-134">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="59a9f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="59a9f-135">Response</span></span>
<span data-ttu-id="59a9f-136">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="59a9f-136">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59a9f-137">Пример</span><span class="sxs-lookup"><span data-stu-id="59a9f-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="59a9f-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="59a9f-138">Request</span></span>
<span data-ttu-id="59a9f-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59a9f-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="59a9f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="59a9f-140">Response</span></span>
<span data-ttu-id="59a9f-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59a9f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```




