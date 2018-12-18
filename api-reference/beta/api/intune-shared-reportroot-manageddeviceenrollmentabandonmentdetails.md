---
title: функция managedDeviceEnrollmentAbandonmentDetails
description: Метаданные для отчета о регистрации abandonment
author: tfitzmac
ms.openlocfilehash: 187f5389bbea761555f4067081d4e0557f2ce5bd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317957"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="3b645-103">функция managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="3b645-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

> <span data-ttu-id="3b645-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3b645-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b645-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b645-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b645-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3b645-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b645-107">Метаданные для отчета о регистрации abandonment</span><span class="sxs-lookup"><span data-stu-id="3b645-107">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b645-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3b645-108">Prerequisites</span></span>
<span data-ttu-id="3b645-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b645-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b645-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b645-111">Permission type</span></span>|<span data-ttu-id="3b645-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b645-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b645-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b645-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3b645-114">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="3b645-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="3b645-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b645-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3b645-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b645-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b645-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b645-117">Not supported.</span></span>|
|<span data-ttu-id="3b645-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b645-118">Application</span></span>|<span data-ttu-id="3b645-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b645-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b645-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b645-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="3b645-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b645-121">Request headers</span></span>
|<span data-ttu-id="3b645-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b645-122">Header</span></span>|<span data-ttu-id="3b645-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3b645-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b645-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b645-124">Authorization</span></span>|<span data-ttu-id="3b645-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3b645-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b645-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3b645-126">Accept</span></span>|<span data-ttu-id="3b645-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3b645-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b645-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b645-128">Request body</span></span>
<span data-ttu-id="3b645-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="3b645-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="3b645-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="3b645-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="3b645-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b645-131">Property</span></span>|<span data-ttu-id="3b645-132">Тип</span><span class="sxs-lookup"><span data-stu-id="3b645-132">Type</span></span>|<span data-ttu-id="3b645-133">Описание</span><span class="sxs-lookup"><span data-stu-id="3b645-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b645-134">skip</span><span class="sxs-lookup"><span data-stu-id="3b645-134">skip</span></span>|<span data-ttu-id="3b645-135">Int32</span><span class="sxs-lookup"><span data-stu-id="3b645-135">Int32</span></span>|<span data-ttu-id="3b645-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3b645-136">Not yet documented</span></span>|
|<span data-ttu-id="3b645-137">top</span><span class="sxs-lookup"><span data-stu-id="3b645-137">top</span></span>|<span data-ttu-id="3b645-138">Int32</span><span class="sxs-lookup"><span data-stu-id="3b645-138">Int32</span></span>|<span data-ttu-id="3b645-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3b645-139">Not yet documented</span></span>|
|<span data-ttu-id="3b645-140">filter</span><span class="sxs-lookup"><span data-stu-id="3b645-140">filter</span></span>|<span data-ttu-id="3b645-141">Строка</span><span class="sxs-lookup"><span data-stu-id="3b645-141">String</span></span>|<span data-ttu-id="3b645-142">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3b645-142">Not yet documented</span></span>|
|<span data-ttu-id="3b645-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="3b645-143">skipToken</span></span>|<span data-ttu-id="3b645-144">Строка</span><span class="sxs-lookup"><span data-stu-id="3b645-144">String</span></span>|<span data-ttu-id="3b645-145">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3b645-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3b645-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b645-146">Response</span></span>
<span data-ttu-id="3b645-147">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b645-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b645-148">Пример</span><span class="sxs-lookup"><span data-stu-id="3b645-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b645-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b645-149">Request</span></span>
<span data-ttu-id="3b645-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b645-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="3b645-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b645-151">Response</span></span>
<span data-ttu-id="3b645-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3b645-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





