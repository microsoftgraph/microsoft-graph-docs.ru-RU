---
title: Функция verifyWindowsEnrollmentAutoDiscovery
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba870846dfb27921a5cb949f5d70044b9cbc34af
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867513"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="09fb7-103">Функция verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="09fb7-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

<span data-ttu-id="09fb7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09fb7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09fb7-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="09fb7-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="09fb7-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09fb7-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09fb7-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09fb7-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09fb7-108">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="09fb7-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="09fb7-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="09fb7-109">Prerequisites</span></span>
<span data-ttu-id="09fb7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09fb7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09fb7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09fb7-112">Permission type</span></span>|<span data-ttu-id="09fb7-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="09fb7-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09fb7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09fb7-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="09fb7-115">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="09fb7-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="09fb7-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09fb7-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="09fb7-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09fb7-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09fb7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09fb7-118">Not supported.</span></span>|
|<span data-ttu-id="09fb7-119">Для приложения</span><span class="sxs-lookup"><span data-stu-id="09fb7-119">Application</span></span>||
| <span data-ttu-id="09fb7-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="09fb7-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="09fb7-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09fb7-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09fb7-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09fb7-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="09fb7-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="09fb7-123">Request headers</span></span>
|<span data-ttu-id="09fb7-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09fb7-124">Header</span></span>|<span data-ttu-id="09fb7-125">Значение</span><span class="sxs-lookup"><span data-stu-id="09fb7-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09fb7-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09fb7-126">Authorization</span></span>|<span data-ttu-id="09fb7-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09fb7-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09fb7-128">Accept</span><span class="sxs-lookup"><span data-stu-id="09fb7-128">Accept</span></span>|<span data-ttu-id="09fb7-129">application/json</span><span class="sxs-lookup"><span data-stu-id="09fb7-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09fb7-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09fb7-130">Request body</span></span>
<span data-ttu-id="09fb7-131">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="09fb7-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="09fb7-132">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="09fb7-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="09fb7-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="09fb7-133">Property</span></span>|<span data-ttu-id="09fb7-134">Тип</span><span class="sxs-lookup"><span data-stu-id="09fb7-134">Type</span></span>|<span data-ttu-id="09fb7-135">Описание</span><span class="sxs-lookup"><span data-stu-id="09fb7-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09fb7-136">domainName</span><span class="sxs-lookup"><span data-stu-id="09fb7-136">domainName</span></span>|<span data-ttu-id="09fb7-137">String</span><span class="sxs-lookup"><span data-stu-id="09fb7-137">String</span></span>|<span data-ttu-id="09fb7-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="09fb7-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="09fb7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="09fb7-139">Response</span></span>
<span data-ttu-id="09fb7-140">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="09fb7-140">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09fb7-141">Пример</span><span class="sxs-lookup"><span data-stu-id="09fb7-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="09fb7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="09fb7-142">Request</span></span>
<span data-ttu-id="09fb7-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09fb7-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="09fb7-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="09fb7-144">Response</span></span>
<span data-ttu-id="09fb7-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09fb7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```










