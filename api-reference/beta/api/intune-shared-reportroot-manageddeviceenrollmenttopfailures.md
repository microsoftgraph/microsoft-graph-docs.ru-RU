---
title: Функция Манажеддевицеенроллменттопфаилурес
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: edc44099ed325455b3bd94b01aa1cec9b9582c0e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526848"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="fca44-103">Функция Манажеддевицеенроллменттопфаилурес</span><span class="sxs-lookup"><span data-stu-id="fca44-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="fca44-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fca44-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fca44-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fca44-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fca44-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fca44-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fca44-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fca44-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fca44-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fca44-108">Prerequisites</span></span>
<span data-ttu-id="fca44-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fca44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fca44-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fca44-111">Permission type</span></span>|<span data-ttu-id="fca44-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fca44-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fca44-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fca44-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fca44-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="fca44-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="fca44-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fca44-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fca44-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fca44-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fca44-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fca44-117">Not supported.</span></span>|
|<span data-ttu-id="fca44-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fca44-118">Application</span></span>|<span data-ttu-id="fca44-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fca44-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fca44-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fca44-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="fca44-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fca44-121">Request headers</span></span>
|<span data-ttu-id="fca44-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fca44-122">Header</span></span>|<span data-ttu-id="fca44-123">Значение</span><span class="sxs-lookup"><span data-stu-id="fca44-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fca44-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fca44-124">Authorization</span></span>|<span data-ttu-id="fca44-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fca44-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fca44-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fca44-126">Accept</span></span>|<span data-ttu-id="fca44-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fca44-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fca44-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fca44-128">Request body</span></span>
<span data-ttu-id="fca44-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="fca44-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="fca44-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="fca44-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="fca44-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="fca44-131">Property</span></span>|<span data-ttu-id="fca44-132">Тип</span><span class="sxs-lookup"><span data-stu-id="fca44-132">Type</span></span>|<span data-ttu-id="fca44-133">Описание</span><span class="sxs-lookup"><span data-stu-id="fca44-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fca44-134">period</span><span class="sxs-lookup"><span data-stu-id="fca44-134">period</span></span>|<span data-ttu-id="fca44-135">String</span><span class="sxs-lookup"><span data-stu-id="fca44-135">String</span></span>|<span data-ttu-id="fca44-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fca44-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fca44-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="fca44-137">Response</span></span>
<span data-ttu-id="fca44-138">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fca44-138">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fca44-139">Пример</span><span class="sxs-lookup"><span data-stu-id="fca44-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="fca44-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="fca44-140">Request</span></span>
<span data-ttu-id="fca44-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fca44-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="fca44-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="fca44-142">Response</span></span>
<span data-ttu-id="fca44-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fca44-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



