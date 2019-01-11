---
title: Функция verifyWindowsEnrollmentAutoDiscovery
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cb14317a132d4368a354d8655df56452100bf5a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894301"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="8b058-103">Функция verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="8b058-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="8b058-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8b058-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b058-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b058-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b058-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8b058-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b058-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8b058-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8b058-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8b058-108">Prerequisites</span></span>
<span data-ttu-id="8b058-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b058-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b058-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b058-111">Permission type</span></span>|<span data-ttu-id="8b058-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b058-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b058-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b058-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8b058-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b058-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8b058-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b058-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b058-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b058-116">Not supported.</span></span>|
|<span data-ttu-id="8b058-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b058-117">Application</span></span>|<span data-ttu-id="8b058-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b058-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b058-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b058-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="8b058-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b058-120">Request headers</span></span>
|<span data-ttu-id="8b058-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b058-121">Header</span></span>|<span data-ttu-id="8b058-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8b058-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b058-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b058-123">Authorization</span></span>|<span data-ttu-id="8b058-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8b058-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b058-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8b058-125">Accept</span></span>|<span data-ttu-id="8b058-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8b058-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b058-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8b058-127">Request body</span></span>
<span data-ttu-id="8b058-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="8b058-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="8b058-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="8b058-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="8b058-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b058-130">Property</span></span>|<span data-ttu-id="8b058-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8b058-131">Type</span></span>|<span data-ttu-id="8b058-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8b058-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b058-133">domainName</span><span class="sxs-lookup"><span data-stu-id="8b058-133">domainName</span></span>|<span data-ttu-id="8b058-134">String</span><span class="sxs-lookup"><span data-stu-id="8b058-134">String</span></span>|<span data-ttu-id="8b058-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8b058-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8b058-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b058-136">Response</span></span>
<span data-ttu-id="8b058-137">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8b058-137">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b058-138">Пример</span><span class="sxs-lookup"><span data-stu-id="8b058-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="8b058-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b058-139">Request</span></span>
<span data-ttu-id="8b058-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b058-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="8b058-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b058-141">Response</span></span>
<span data-ttu-id="8b058-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8b058-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```





