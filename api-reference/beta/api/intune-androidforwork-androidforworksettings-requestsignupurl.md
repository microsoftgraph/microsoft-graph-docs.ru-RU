---
title: Действие requestSignupUrl
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d7e1b732631df277f53a2c7c2ef45bbd70fcff5b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864458"
---
# <a name="requestsignupurl-action"></a><span data-ttu-id="55d94-103">Действие requestSignupUrl</span><span class="sxs-lookup"><span data-stu-id="55d94-103">requestSignupUrl action</span></span>

> <span data-ttu-id="55d94-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="55d94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55d94-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55d94-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55d94-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="55d94-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55d94-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="55d94-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="55d94-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="55d94-108">Prerequisites</span></span>
<span data-ttu-id="55d94-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55d94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55d94-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55d94-111">Permission type</span></span>|<span data-ttu-id="55d94-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55d94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55d94-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55d94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55d94-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55d94-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55d94-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55d94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55d94-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55d94-116">Not supported.</span></span>|
|<span data-ttu-id="55d94-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55d94-117">Application</span></span>|<span data-ttu-id="55d94-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55d94-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55d94-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55d94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="55d94-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55d94-120">Request headers</span></span>
|<span data-ttu-id="55d94-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55d94-121">Header</span></span>|<span data-ttu-id="55d94-122">Значение</span><span class="sxs-lookup"><span data-stu-id="55d94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55d94-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="55d94-123">Authorization</span></span>|<span data-ttu-id="55d94-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="55d94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55d94-125">Accept</span><span class="sxs-lookup"><span data-stu-id="55d94-125">Accept</span></span>|<span data-ttu-id="55d94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55d94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55d94-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="55d94-127">Request body</span></span>
<span data-ttu-id="55d94-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55d94-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="55d94-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="55d94-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="55d94-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="55d94-130">Property</span></span>|<span data-ttu-id="55d94-131">Тип</span><span class="sxs-lookup"><span data-stu-id="55d94-131">Type</span></span>|<span data-ttu-id="55d94-132">Описание</span><span class="sxs-lookup"><span data-stu-id="55d94-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55d94-133">hostName</span><span class="sxs-lookup"><span data-stu-id="55d94-133">hostName</span></span>|<span data-ttu-id="55d94-134">String</span><span class="sxs-lookup"><span data-stu-id="55d94-134">String</span></span>|<span data-ttu-id="55d94-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="55d94-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="55d94-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="55d94-136">Response</span></span>
<span data-ttu-id="55d94-137">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55d94-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55d94-138">Пример</span><span class="sxs-lookup"><span data-stu-id="55d94-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="55d94-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="55d94-139">Request</span></span>
<span data-ttu-id="55d94-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55d94-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="55d94-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="55d94-141">Response</span></span>
<span data-ttu-id="55d94-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="55d94-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```





