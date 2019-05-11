---
title: Функция verifyWindowsEnrollmentAutoDiscovery
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2e78aa3e8010a05771d1fbfd3f889345dadb936d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898355"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="9dd7f-103">Функция verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="9dd7f-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="9dd7f-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9dd7f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9dd7f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dd7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9dd7f-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9dd7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dd7f-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9dd7f-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9dd7f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9dd7f-108">Prerequisites</span></span>
<span data-ttu-id="9dd7f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dd7f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dd7f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9dd7f-111">Permission type</span></span>|<span data-ttu-id="9dd7f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9dd7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9dd7f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9dd7f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9dd7f-114">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="9dd7f-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="9dd7f-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dd7f-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9dd7f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9dd7f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9dd7f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dd7f-117">Not supported.</span></span>|
|<span data-ttu-id="9dd7f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9dd7f-118">Application</span></span>|<span data-ttu-id="9dd7f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dd7f-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9dd7f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9dd7f-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="9dd7f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9dd7f-121">Request headers</span></span>
|<span data-ttu-id="9dd7f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9dd7f-122">Header</span></span>|<span data-ttu-id="9dd7f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9dd7f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9dd7f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9dd7f-124">Authorization</span></span>|<span data-ttu-id="9dd7f-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9dd7f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9dd7f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9dd7f-126">Accept</span></span>|<span data-ttu-id="9dd7f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9dd7f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dd7f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9dd7f-128">Request body</span></span>
<span data-ttu-id="9dd7f-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="9dd7f-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="9dd7f-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="9dd7f-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="9dd7f-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="9dd7f-131">Property</span></span>|<span data-ttu-id="9dd7f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="9dd7f-132">Type</span></span>|<span data-ttu-id="9dd7f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="9dd7f-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dd7f-134">domainName</span><span class="sxs-lookup"><span data-stu-id="9dd7f-134">domainName</span></span>|<span data-ttu-id="9dd7f-135">String</span><span class="sxs-lookup"><span data-stu-id="9dd7f-135">String</span></span>|<span data-ttu-id="9dd7f-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9dd7f-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9dd7f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dd7f-137">Response</span></span>
<span data-ttu-id="9dd7f-138">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9dd7f-138">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dd7f-139">Пример</span><span class="sxs-lookup"><span data-stu-id="9dd7f-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="9dd7f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="9dd7f-140">Request</span></span>
<span data-ttu-id="9dd7f-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9dd7f-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="9dd7f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dd7f-142">Response</span></span>
<span data-ttu-id="9dd7f-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9dd7f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



