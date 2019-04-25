---
title: Функция Манажеддевицеенроллментфаилуредетаилс
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e861b8947396c67c72ba47493d30e6010905b107
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526925"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="8c784-103">Функция Манажеддевицеенроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="8c784-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="8c784-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8c784-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8c784-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c784-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c784-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c784-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c784-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c784-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c784-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8c784-108">Prerequisites</span></span>
<span data-ttu-id="8c784-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c784-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c784-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c784-111">Permission type</span></span>|<span data-ttu-id="8c784-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c784-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c784-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c784-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8c784-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="8c784-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="8c784-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c784-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8c784-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c784-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c784-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c784-117">Not supported.</span></span>|
|<span data-ttu-id="8c784-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c784-118">Application</span></span>|<span data-ttu-id="8c784-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c784-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c784-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c784-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="8c784-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c784-121">Request headers</span></span>
|<span data-ttu-id="8c784-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c784-122">Header</span></span>|<span data-ttu-id="8c784-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8c784-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c784-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c784-124">Authorization</span></span>|<span data-ttu-id="8c784-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c784-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c784-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8c784-126">Accept</span></span>|<span data-ttu-id="8c784-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8c784-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c784-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c784-128">Request body</span></span>
<span data-ttu-id="8c784-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="8c784-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="8c784-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c784-130">Property</span></span>|<span data-ttu-id="8c784-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8c784-131">Type</span></span>|<span data-ttu-id="8c784-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8c784-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c784-133">filter</span><span class="sxs-lookup"><span data-stu-id="8c784-133">filter</span></span>|<span data-ttu-id="8c784-134">String</span><span class="sxs-lookup"><span data-stu-id="8c784-134">String</span></span>|<span data-ttu-id="8c784-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c784-135">Not yet documented</span></span>|
|<span data-ttu-id="8c784-136">skipToken</span><span class="sxs-lookup"><span data-stu-id="8c784-136">skipToken</span></span>|<span data-ttu-id="8c784-137">String</span><span class="sxs-lookup"><span data-stu-id="8c784-137">String</span></span>|<span data-ttu-id="8c784-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c784-138">Not yet documented</span></span>|
|<span data-ttu-id="8c784-139">skip</span><span class="sxs-lookup"><span data-stu-id="8c784-139">skip</span></span>|<span data-ttu-id="8c784-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8c784-140">Int32</span></span>|<span data-ttu-id="8c784-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8c784-141">Not yet documented</span></span>|
|<span data-ttu-id="8c784-142">top</span><span class="sxs-lookup"><span data-stu-id="8c784-142">top</span></span>|<span data-ttu-id="8c784-143">Int32</span><span class="sxs-lookup"><span data-stu-id="8c784-143">Int32</span></span>|<span data-ttu-id="8c784-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8c784-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8c784-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c784-145">Response</span></span>
<span data-ttu-id="8c784-146">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c784-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c784-147">Пример</span><span class="sxs-lookup"><span data-stu-id="8c784-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c784-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c784-148">Request</span></span>
<span data-ttu-id="8c784-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c784-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="8c784-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c784-150">Response</span></span>
<span data-ttu-id="8c784-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c784-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



