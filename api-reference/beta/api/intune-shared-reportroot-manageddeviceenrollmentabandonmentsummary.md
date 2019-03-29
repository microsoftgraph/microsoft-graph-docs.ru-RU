---
title: Функция Манажеддевицеенроллментабандонментсуммари
description: Метаданные для сводного отчета об отмене регистрации
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0bd8e82aa7987e89d9f9a740a8fa9c181570ccd8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30956662"
---
# <a name="manageddeviceenrollmentabandonmentsummary-function"></a><span data-ttu-id="84478-103">Функция Манажеддевицеенроллментабандонментсуммари</span><span class="sxs-lookup"><span data-stu-id="84478-103">managedDeviceEnrollmentAbandonmentSummary function</span></span>

> <span data-ttu-id="84478-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="84478-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="84478-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84478-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84478-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84478-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84478-107">Метаданные для сводного отчета об отмене регистрации</span><span class="sxs-lookup"><span data-stu-id="84478-107">Metadata for Enrollment abandonment summary report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84478-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="84478-108">Prerequisites</span></span>
<span data-ttu-id="84478-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84478-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84478-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84478-111">Permission type</span></span>|<span data-ttu-id="84478-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84478-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84478-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84478-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="84478-114">&nbsp;&nbsp; **Траублшутинг**</span><span class="sxs-lookup"><span data-stu-id="84478-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="84478-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="84478-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="84478-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84478-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84478-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84478-117">Not supported.</span></span>|
|<span data-ttu-id="84478-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84478-118">Application</span></span>|<span data-ttu-id="84478-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84478-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84478-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84478-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentSummary
```

## <a name="request-headers"></a><span data-ttu-id="84478-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84478-121">Request headers</span></span>
|<span data-ttu-id="84478-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84478-122">Header</span></span>|<span data-ttu-id="84478-123">Значение</span><span class="sxs-lookup"><span data-stu-id="84478-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84478-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84478-124">Authorization</span></span>|<span data-ttu-id="84478-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84478-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84478-126">Accept</span><span class="sxs-lookup"><span data-stu-id="84478-126">Accept</span></span>|<span data-ttu-id="84478-127">application/json</span><span class="sxs-lookup"><span data-stu-id="84478-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84478-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84478-128">Request body</span></span>
<span data-ttu-id="84478-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="84478-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="84478-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="84478-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="84478-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="84478-131">Property</span></span>|<span data-ttu-id="84478-132">Тип</span><span class="sxs-lookup"><span data-stu-id="84478-132">Type</span></span>|<span data-ttu-id="84478-133">Описание</span><span class="sxs-lookup"><span data-stu-id="84478-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84478-134">skip</span><span class="sxs-lookup"><span data-stu-id="84478-134">skip</span></span>|<span data-ttu-id="84478-135">Int32</span><span class="sxs-lookup"><span data-stu-id="84478-135">Int32</span></span>|<span data-ttu-id="84478-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="84478-136">Not yet documented</span></span>|
|<span data-ttu-id="84478-137">top</span><span class="sxs-lookup"><span data-stu-id="84478-137">top</span></span>|<span data-ttu-id="84478-138">Int32</span><span class="sxs-lookup"><span data-stu-id="84478-138">Int32</span></span>|<span data-ttu-id="84478-139">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="84478-139">Not yet documented</span></span>|
|<span data-ttu-id="84478-140">filter</span><span class="sxs-lookup"><span data-stu-id="84478-140">filter</span></span>|<span data-ttu-id="84478-141">String</span><span class="sxs-lookup"><span data-stu-id="84478-141">String</span></span>|<span data-ttu-id="84478-142">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="84478-142">Not yet documented</span></span>|
|<span data-ttu-id="84478-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="84478-143">skipToken</span></span>|<span data-ttu-id="84478-144">String</span><span class="sxs-lookup"><span data-stu-id="84478-144">String</span></span>|<span data-ttu-id="84478-145">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="84478-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="84478-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="84478-146">Response</span></span>
<span data-ttu-id="84478-147">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84478-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84478-148">Пример</span><span class="sxs-lookup"><span data-stu-id="84478-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="84478-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="84478-149">Request</span></span>
<span data-ttu-id="84478-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84478-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentSummary(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="84478-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="84478-151">Response</span></span>
<span data-ttu-id="84478-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84478-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





