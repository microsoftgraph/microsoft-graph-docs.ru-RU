---
title: Функция verifyWindowsEnrollmentAutoDiscovery
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af2d2be57342bb3974789ac84ae26e8a3d74a267
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801028"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="6f492-103">Функция verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="6f492-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="6f492-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6f492-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6f492-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f492-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f492-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f492-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f492-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6f492-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f492-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6f492-108">Prerequisites</span></span>
<span data-ttu-id="6f492-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f492-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f492-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f492-111">Permission type</span></span>|<span data-ttu-id="6f492-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f492-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f492-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f492-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6f492-114">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="6f492-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="6f492-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f492-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6f492-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f492-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f492-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f492-117">Not supported.</span></span>|
|<span data-ttu-id="6f492-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="6f492-118">Application</span></span>||
| <span data-ttu-id="6f492-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="6f492-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="6f492-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f492-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f492-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f492-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="6f492-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6f492-122">Request headers</span></span>
|<span data-ttu-id="6f492-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f492-123">Header</span></span>|<span data-ttu-id="6f492-124">Значение</span><span class="sxs-lookup"><span data-stu-id="6f492-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f492-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f492-125">Authorization</span></span>|<span data-ttu-id="6f492-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f492-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f492-127">Accept</span><span class="sxs-lookup"><span data-stu-id="6f492-127">Accept</span></span>|<span data-ttu-id="6f492-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6f492-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f492-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f492-129">Request body</span></span>
<span data-ttu-id="6f492-130">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="6f492-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="6f492-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="6f492-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6f492-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f492-132">Property</span></span>|<span data-ttu-id="6f492-133">Тип</span><span class="sxs-lookup"><span data-stu-id="6f492-133">Type</span></span>|<span data-ttu-id="6f492-134">Описание</span><span class="sxs-lookup"><span data-stu-id="6f492-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f492-135">domainName</span><span class="sxs-lookup"><span data-stu-id="6f492-135">domainName</span></span>|<span data-ttu-id="6f492-136">String</span><span class="sxs-lookup"><span data-stu-id="6f492-136">String</span></span>|<span data-ttu-id="6f492-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6f492-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6f492-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f492-138">Response</span></span>
<span data-ttu-id="6f492-139">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6f492-139">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f492-140">Пример</span><span class="sxs-lookup"><span data-stu-id="6f492-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f492-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f492-141">Request</span></span>
<span data-ttu-id="6f492-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f492-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="6f492-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f492-143">Response</span></span>
<span data-ttu-id="6f492-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f492-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```










