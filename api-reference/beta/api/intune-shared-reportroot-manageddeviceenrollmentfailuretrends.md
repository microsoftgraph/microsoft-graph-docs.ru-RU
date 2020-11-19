---
title: Функция Манажеддевицеенроллментфаилуретрендс
description: Метаданные отчета о тенденциях сбоев регистрации
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: beae775f5cc4549f01457183775073f651cb8719
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49223859"
---
# <a name="manageddeviceenrollmentfailuretrends-function"></a><span data-ttu-id="1dd6c-103">Функция Манажеддевицеенроллментфаилуретрендс</span><span class="sxs-lookup"><span data-stu-id="1dd6c-103">managedDeviceEnrollmentFailureTrends function</span></span>

<span data-ttu-id="1dd6c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dd6c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1dd6c-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1dd6c-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1dd6c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dd6c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1dd6c-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1dd6c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dd6c-108">Метаданные отчета о тенденциях сбоев регистрации</span><span class="sxs-lookup"><span data-stu-id="1dd6c-108">Metadata for the enrollment failure trends report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1dd6c-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1dd6c-109">Prerequisites</span></span>
<span data-ttu-id="1dd6c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dd6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dd6c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1dd6c-112">Permission type</span></span>|<span data-ttu-id="1dd6c-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1dd6c-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dd6c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1dd6c-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1dd6c-115">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="1dd6c-115">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="1dd6c-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dd6c-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1dd6c-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dd6c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dd6c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dd6c-118">Not supported.</span></span>|
|<span data-ttu-id="1dd6c-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="1dd6c-119">Application</span></span>||
| <span data-ttu-id="1dd6c-120">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="1dd6c-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="1dd6c-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dd6c-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dd6c-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1dd6c-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureTrends
```

## <a name="request-headers"></a><span data-ttu-id="1dd6c-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1dd6c-123">Request headers</span></span>
|<span data-ttu-id="1dd6c-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1dd6c-124">Header</span></span>|<span data-ttu-id="1dd6c-125">Значение</span><span class="sxs-lookup"><span data-stu-id="1dd6c-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dd6c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1dd6c-126">Authorization</span></span>|<span data-ttu-id="1dd6c-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1dd6c-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dd6c-128">Accept</span><span class="sxs-lookup"><span data-stu-id="1dd6c-128">Accept</span></span>|<span data-ttu-id="1dd6c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="1dd6c-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dd6c-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1dd6c-130">Request body</span></span>
<span data-ttu-id="1dd6c-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1dd6c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dd6c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dd6c-132">Response</span></span>
<span data-ttu-id="1dd6c-133">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1dd6c-133">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dd6c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="1dd6c-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="1dd6c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dd6c-135">Request</span></span>
<span data-ttu-id="1dd6c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1dd6c-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureTrends
```

### <a name="response"></a><span data-ttu-id="1dd6c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dd6c-137">Response</span></span>
<span data-ttu-id="1dd6c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1dd6c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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










