---
title: Функция Манажеддевицеенроллментфаилуретрендс
description: Метаданные отчета о тенденциях сбоев регистрации
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 20c9701f2d21414a37b4c778d87aa1d237f12d88
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800678"
---
# <a name="manageddeviceenrollmentfailuretrends-function"></a><span data-ttu-id="8fbc4-103">Функция Манажеддевицеенроллментфаилуретрендс</span><span class="sxs-lookup"><span data-stu-id="8fbc4-103">managedDeviceEnrollmentFailureTrends function</span></span>

> <span data-ttu-id="8fbc4-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8fbc4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8fbc4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fbc4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8fbc4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8fbc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fbc4-107">Метаданные отчета о тенденциях сбоев регистрации</span><span class="sxs-lookup"><span data-stu-id="8fbc4-107">Metadata for the enrollment failure trends report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8fbc4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8fbc4-108">Prerequisites</span></span>
<span data-ttu-id="8fbc4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fbc4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fbc4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fbc4-111">Permission type</span></span>|<span data-ttu-id="8fbc4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fbc4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fbc4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fbc4-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8fbc4-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="8fbc4-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="8fbc4-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fbc4-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8fbc4-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fbc4-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fbc4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fbc4-117">Not supported.</span></span>|
|<span data-ttu-id="8fbc4-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="8fbc4-118">Application</span></span>||
| <span data-ttu-id="8fbc4-119">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="8fbc4-119">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="8fbc4-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fbc4-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fbc4-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fbc4-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureTrends
```

## <a name="request-headers"></a><span data-ttu-id="8fbc4-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8fbc4-122">Request headers</span></span>
|<span data-ttu-id="8fbc4-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8fbc4-123">Header</span></span>|<span data-ttu-id="8fbc4-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8fbc4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fbc4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fbc4-125">Authorization</span></span>|<span data-ttu-id="8fbc4-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fbc4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fbc4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8fbc4-127">Accept</span></span>|<span data-ttu-id="8fbc4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8fbc4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fbc4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8fbc4-129">Request body</span></span>
<span data-ttu-id="8fbc4-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8fbc4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fbc4-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="8fbc4-131">Response</span></span>
<span data-ttu-id="8fbc4-132">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8fbc4-132">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fbc4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8fbc4-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="8fbc4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fbc4-134">Request</span></span>
<span data-ttu-id="8fbc4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8fbc4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureTrends
```

### <a name="response"></a><span data-ttu-id="8fbc4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fbc4-136">Response</span></span>
<span data-ttu-id="8fbc4-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8fbc4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










