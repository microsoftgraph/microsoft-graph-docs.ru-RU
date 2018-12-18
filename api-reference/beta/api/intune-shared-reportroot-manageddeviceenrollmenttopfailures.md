---
title: функция managedDeviceEnrollmentTopFailures
description: Н/Д
author: tfitzmac
ms.openlocfilehash: dd62bffa153d56c279644eeaa99763c4220f27b1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337823"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="aa2ae-103">функция managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="aa2ae-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="aa2ae-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aa2ae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa2ae-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa2ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa2ae-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aa2ae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa2ae-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="aa2ae-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aa2ae-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="aa2ae-108">Prerequisites</span></span>
<span data-ttu-id="aa2ae-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa2ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa2ae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa2ae-111">Permission type</span></span>|<span data-ttu-id="aa2ae-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa2ae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa2ae-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa2ae-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="aa2ae-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="aa2ae-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="aa2ae-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa2ae-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="aa2ae-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa2ae-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa2ae-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa2ae-117">Not supported.</span></span>|
|<span data-ttu-id="aa2ae-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa2ae-118">Application</span></span>|<span data-ttu-id="aa2ae-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa2ae-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa2ae-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa2ae-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="aa2ae-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa2ae-121">Request headers</span></span>
|<span data-ttu-id="aa2ae-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aa2ae-122">Header</span></span>|<span data-ttu-id="aa2ae-123">Значение</span><span class="sxs-lookup"><span data-stu-id="aa2ae-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa2ae-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa2ae-124">Authorization</span></span>|<span data-ttu-id="aa2ae-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="aa2ae-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa2ae-126">Accept</span><span class="sxs-lookup"><span data-stu-id="aa2ae-126">Accept</span></span>|<span data-ttu-id="aa2ae-127">application/json</span><span class="sxs-lookup"><span data-stu-id="aa2ae-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa2ae-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa2ae-128">Request body</span></span>
<span data-ttu-id="aa2ae-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="aa2ae-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="aa2ae-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="aa2ae-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="aa2ae-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa2ae-131">Property</span></span>|<span data-ttu-id="aa2ae-132">Тип</span><span class="sxs-lookup"><span data-stu-id="aa2ae-132">Type</span></span>|<span data-ttu-id="aa2ae-133">Описание</span><span class="sxs-lookup"><span data-stu-id="aa2ae-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa2ae-134">period</span><span class="sxs-lookup"><span data-stu-id="aa2ae-134">period</span></span>|<span data-ttu-id="aa2ae-135">Строка</span><span class="sxs-lookup"><span data-stu-id="aa2ae-135">String</span></span>|<span data-ttu-id="aa2ae-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="aa2ae-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="aa2ae-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa2ae-137">Response</span></span>
<span data-ttu-id="aa2ae-138">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aa2ae-138">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa2ae-139">Пример</span><span class="sxs-lookup"><span data-stu-id="aa2ae-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="aa2ae-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa2ae-140">Request</span></span>
<span data-ttu-id="aa2ae-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa2ae-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="aa2ae-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa2ae-142">Response</span></span>
<span data-ttu-id="aa2ae-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="aa2ae-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```



