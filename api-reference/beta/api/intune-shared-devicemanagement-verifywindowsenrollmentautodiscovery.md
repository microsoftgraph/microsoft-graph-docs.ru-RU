---
title: Функция verifyWindowsEnrollmentAutoDiscovery
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 44e462210c35dc2d2cbe62a671be2323be8a0b97
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945365"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="5d0fa-103">Функция verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="5d0fa-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="5d0fa-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5d0fa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d0fa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d0fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d0fa-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5d0fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d0fa-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5d0fa-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5d0fa-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5d0fa-108">Prerequisites</span></span>
<span data-ttu-id="5d0fa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d0fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d0fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d0fa-111">Permission type</span></span>|<span data-ttu-id="5d0fa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d0fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d0fa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d0fa-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5d0fa-114">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="5d0fa-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="5d0fa-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d0fa-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5d0fa-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d0fa-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d0fa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d0fa-117">Not supported.</span></span>|
|<span data-ttu-id="5d0fa-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d0fa-118">Application</span></span>|<span data-ttu-id="5d0fa-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d0fa-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d0fa-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d0fa-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="5d0fa-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d0fa-121">Request headers</span></span>
|<span data-ttu-id="5d0fa-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5d0fa-122">Header</span></span>|<span data-ttu-id="5d0fa-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5d0fa-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d0fa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d0fa-124">Authorization</span></span>|<span data-ttu-id="5d0fa-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5d0fa-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d0fa-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5d0fa-126">Accept</span></span>|<span data-ttu-id="5d0fa-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5d0fa-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d0fa-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5d0fa-128">Request body</span></span>
<span data-ttu-id="5d0fa-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="5d0fa-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="5d0fa-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="5d0fa-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="5d0fa-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d0fa-131">Property</span></span>|<span data-ttu-id="5d0fa-132">Тип</span><span class="sxs-lookup"><span data-stu-id="5d0fa-132">Type</span></span>|<span data-ttu-id="5d0fa-133">Описание</span><span class="sxs-lookup"><span data-stu-id="5d0fa-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d0fa-134">domainName</span><span class="sxs-lookup"><span data-stu-id="5d0fa-134">domainName</span></span>|<span data-ttu-id="5d0fa-135">String</span><span class="sxs-lookup"><span data-stu-id="5d0fa-135">String</span></span>|<span data-ttu-id="5d0fa-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5d0fa-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5d0fa-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d0fa-137">Response</span></span>
<span data-ttu-id="5d0fa-138">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5d0fa-138">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d0fa-139">Пример</span><span class="sxs-lookup"><span data-stu-id="5d0fa-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="5d0fa-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d0fa-140">Request</span></span>
<span data-ttu-id="5d0fa-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d0fa-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="5d0fa-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="5d0fa-142">Response</span></span>
<span data-ttu-id="5d0fa-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5d0fa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



