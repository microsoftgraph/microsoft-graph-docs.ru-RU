---
title: Функция getAuditActivityTypes
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 05d2674f8049c107f3595bcd8f234f3dd01cfb2e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350757"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="c3be7-103">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="c3be7-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="c3be7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c3be7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3be7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3be7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3be7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c3be7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3be7-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c3be7-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c3be7-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c3be7-108">Prerequisites</span></span>
<span data-ttu-id="c3be7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3be7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3be7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3be7-111">Permission type</span></span>|<span data-ttu-id="c3be7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3be7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3be7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3be7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3be7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3be7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c3be7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3be7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3be7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3be7-116">Not supported.</span></span>|
|<span data-ttu-id="c3be7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3be7-117">Application</span></span>|<span data-ttu-id="c3be7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3be7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3be7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3be7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="c3be7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3be7-120">Request headers</span></span>
|<span data-ttu-id="c3be7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3be7-121">Header</span></span>|<span data-ttu-id="c3be7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c3be7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3be7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3be7-123">Authorization</span></span>|<span data-ttu-id="c3be7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c3be7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3be7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c3be7-125">Accept</span></span>|<span data-ttu-id="c3be7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3be7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3be7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3be7-127">Request body</span></span>
<span data-ttu-id="c3be7-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="c3be7-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="c3be7-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="c3be7-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="c3be7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3be7-130">Property</span></span>|<span data-ttu-id="c3be7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c3be7-131">Type</span></span>|<span data-ttu-id="c3be7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c3be7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3be7-133">category</span><span class="sxs-lookup"><span data-stu-id="c3be7-133">category</span></span>|<span data-ttu-id="c3be7-134">String</span><span class="sxs-lookup"><span data-stu-id="c3be7-134">String</span></span>|<span data-ttu-id="c3be7-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c3be7-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c3be7-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3be7-136">Response</span></span>
<span data-ttu-id="c3be7-137">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3be7-137">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3be7-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c3be7-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="c3be7-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3be7-139">Request</span></span>
<span data-ttu-id="c3be7-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3be7-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="c3be7-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3be7-141">Response</span></span>
<span data-ttu-id="c3be7-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c3be7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





