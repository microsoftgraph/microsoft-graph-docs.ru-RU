---
title: Функция Манажеддевицеенроллментфаилуредетаилс
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0dff0f10c1bcfbed9bb79bcf6566bb6a329521b5
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572294"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="b11ab-103">Функция Манажеддевицеенроллментфаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="b11ab-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="b11ab-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b11ab-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b11ab-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b11ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b11ab-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b11ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b11ab-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b11ab-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b11ab-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b11ab-108">Prerequisites</span></span>
<span data-ttu-id="b11ab-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b11ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b11ab-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b11ab-111">Permission type</span></span>|<span data-ttu-id="b11ab-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b11ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b11ab-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b11ab-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b11ab-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="b11ab-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b11ab-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b11ab-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b11ab-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b11ab-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b11ab-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b11ab-117">Not supported.</span></span>|
|<span data-ttu-id="b11ab-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b11ab-118">Application</span></span>|<span data-ttu-id="b11ab-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b11ab-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b11ab-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b11ab-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="b11ab-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b11ab-121">Request headers</span></span>
|<span data-ttu-id="b11ab-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b11ab-122">Header</span></span>|<span data-ttu-id="b11ab-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b11ab-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b11ab-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b11ab-124">Authorization</span></span>|<span data-ttu-id="b11ab-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b11ab-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b11ab-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b11ab-126">Accept</span></span>|<span data-ttu-id="b11ab-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b11ab-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b11ab-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b11ab-128">Request body</span></span>
<span data-ttu-id="b11ab-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="b11ab-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b11ab-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b11ab-130">Property</span></span>|<span data-ttu-id="b11ab-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b11ab-131">Type</span></span>|<span data-ttu-id="b11ab-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b11ab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b11ab-133">filter</span><span class="sxs-lookup"><span data-stu-id="b11ab-133">filter</span></span>|<span data-ttu-id="b11ab-134">String</span><span class="sxs-lookup"><span data-stu-id="b11ab-134">String</span></span>|<span data-ttu-id="b11ab-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b11ab-135">Not yet documented</span></span>|
|<span data-ttu-id="b11ab-136">skipToken</span><span class="sxs-lookup"><span data-stu-id="b11ab-136">skipToken</span></span>|<span data-ttu-id="b11ab-137">String</span><span class="sxs-lookup"><span data-stu-id="b11ab-137">String</span></span>|<span data-ttu-id="b11ab-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b11ab-138">Not yet documented</span></span>|
|<span data-ttu-id="b11ab-139">skip</span><span class="sxs-lookup"><span data-stu-id="b11ab-139">skip</span></span>|<span data-ttu-id="b11ab-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b11ab-140">Int32</span></span>|<span data-ttu-id="b11ab-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b11ab-141">Not yet documented</span></span>|
|<span data-ttu-id="b11ab-142">top</span><span class="sxs-lookup"><span data-stu-id="b11ab-142">top</span></span>|<span data-ttu-id="b11ab-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b11ab-143">Int32</span></span>|<span data-ttu-id="b11ab-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b11ab-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b11ab-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="b11ab-145">Response</span></span>
<span data-ttu-id="b11ab-146">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b11ab-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b11ab-147">Пример</span><span class="sxs-lookup"><span data-stu-id="b11ab-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="b11ab-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="b11ab-148">Request</span></span>
<span data-ttu-id="b11ab-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b11ab-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b11ab-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="b11ab-150">Response</span></span>
<span data-ttu-id="b11ab-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b11ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



