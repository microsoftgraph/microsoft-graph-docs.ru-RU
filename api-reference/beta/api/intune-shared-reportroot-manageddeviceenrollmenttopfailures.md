---
title: Функция Манажеддевицеенроллменттопфаилурес
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0730f98e1cd46b78091eb4ff44f6c08c52d2db8a
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570923"
---
# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="71b60-103">Функция Манажеддевицеенроллменттопфаилурес</span><span class="sxs-lookup"><span data-stu-id="71b60-103">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="71b60-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="71b60-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="71b60-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71b60-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71b60-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71b60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71b60-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="71b60-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71b60-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="71b60-108">Prerequisites</span></span>
<span data-ttu-id="71b60-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="71b60-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="71b60-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71b60-111">Permission type</span></span>|<span data-ttu-id="71b60-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="71b60-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71b60-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71b60-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="71b60-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="71b60-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="71b60-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71b60-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="71b60-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71b60-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71b60-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71b60-117">Not supported.</span></span>|
|<span data-ttu-id="71b60-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71b60-118">Application</span></span>|<span data-ttu-id="71b60-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71b60-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71b60-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71b60-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="71b60-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71b60-121">Request headers</span></span>
|<span data-ttu-id="71b60-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71b60-122">Header</span></span>|<span data-ttu-id="71b60-123">Значение</span><span class="sxs-lookup"><span data-stu-id="71b60-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71b60-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71b60-124">Authorization</span></span>|<span data-ttu-id="71b60-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71b60-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71b60-126">Accept</span><span class="sxs-lookup"><span data-stu-id="71b60-126">Accept</span></span>|<span data-ttu-id="71b60-127">application/json</span><span class="sxs-lookup"><span data-stu-id="71b60-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71b60-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71b60-128">Request body</span></span>
<span data-ttu-id="71b60-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="71b60-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="71b60-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="71b60-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="71b60-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="71b60-131">Property</span></span>|<span data-ttu-id="71b60-132">Тип</span><span class="sxs-lookup"><span data-stu-id="71b60-132">Type</span></span>|<span data-ttu-id="71b60-133">Описание</span><span class="sxs-lookup"><span data-stu-id="71b60-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71b60-134">period</span><span class="sxs-lookup"><span data-stu-id="71b60-134">period</span></span>|<span data-ttu-id="71b60-135">String</span><span class="sxs-lookup"><span data-stu-id="71b60-135">String</span></span>|<span data-ttu-id="71b60-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="71b60-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="71b60-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="71b60-137">Response</span></span>
<span data-ttu-id="71b60-138">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71b60-138">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71b60-139">Пример</span><span class="sxs-lookup"><span data-stu-id="71b60-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="71b60-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="71b60-140">Request</span></span>
<span data-ttu-id="71b60-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71b60-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="71b60-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="71b60-142">Response</span></span>
<span data-ttu-id="71b60-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71b60-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



