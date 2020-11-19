---
title: Функция verifyWindowsEnrollmentAutoDiscovery
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 977341b1e54e5b68eb4e5d6d95259c154cd02b01
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49210118"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="46a01-103">Функция verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="46a01-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

<span data-ttu-id="46a01-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46a01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46a01-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="46a01-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="46a01-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46a01-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46a01-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46a01-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46a01-108">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="46a01-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="46a01-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="46a01-109">Prerequisites</span></span>
<span data-ttu-id="46a01-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46a01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46a01-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46a01-112">Permission type</span></span>|<span data-ttu-id="46a01-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46a01-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46a01-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46a01-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="46a01-115">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="46a01-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="46a01-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46a01-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="46a01-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46a01-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46a01-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46a01-118">Not supported.</span></span>|
|<span data-ttu-id="46a01-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="46a01-119">Application</span></span>||
| <span data-ttu-id="46a01-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="46a01-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="46a01-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46a01-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46a01-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46a01-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="46a01-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="46a01-123">Request headers</span></span>
|<span data-ttu-id="46a01-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46a01-124">Header</span></span>|<span data-ttu-id="46a01-125">Значение</span><span class="sxs-lookup"><span data-stu-id="46a01-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46a01-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46a01-126">Authorization</span></span>|<span data-ttu-id="46a01-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46a01-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46a01-128">Accept</span><span class="sxs-lookup"><span data-stu-id="46a01-128">Accept</span></span>|<span data-ttu-id="46a01-129">application/json</span><span class="sxs-lookup"><span data-stu-id="46a01-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46a01-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46a01-130">Request body</span></span>
<span data-ttu-id="46a01-131">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="46a01-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="46a01-132">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="46a01-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="46a01-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="46a01-133">Property</span></span>|<span data-ttu-id="46a01-134">Тип</span><span class="sxs-lookup"><span data-stu-id="46a01-134">Type</span></span>|<span data-ttu-id="46a01-135">Описание</span><span class="sxs-lookup"><span data-stu-id="46a01-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46a01-136">domainName</span><span class="sxs-lookup"><span data-stu-id="46a01-136">domainName</span></span>|<span data-ttu-id="46a01-137">String</span><span class="sxs-lookup"><span data-stu-id="46a01-137">String</span></span>|<span data-ttu-id="46a01-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="46a01-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="46a01-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="46a01-139">Response</span></span>
<span data-ttu-id="46a01-140">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="46a01-140">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46a01-141">Пример</span><span class="sxs-lookup"><span data-stu-id="46a01-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="46a01-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="46a01-142">Request</span></span>
<span data-ttu-id="46a01-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46a01-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="46a01-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="46a01-144">Response</span></span>
<span data-ttu-id="46a01-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46a01-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```










