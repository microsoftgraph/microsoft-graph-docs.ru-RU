---
title: Функция deviceConfigurationDeviceActivity
description: Метаданные для отчета о работе устройств
ms.openlocfilehash: 547b91506420b864334b46a25516a4b15cefaa1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079991"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="ab8ba-103">Функция deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="ab8ba-103">deviceConfigurationDeviceActivity function</span></span>

> <span data-ttu-id="ab8ba-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ab8ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab8ba-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab8ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab8ba-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ab8ba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab8ba-107">Метаданные для отчета о работе устройств</span><span class="sxs-lookup"><span data-stu-id="ab8ba-107">Metadata for the device configuration device activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab8ba-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ab8ba-108">Prerequisites</span></span>
<span data-ttu-id="ab8ba-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab8ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab8ba-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab8ba-111">Permission type</span></span>|<span data-ttu-id="ab8ba-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab8ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab8ba-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab8ba-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ab8ba-114">&nbsp;&nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="ab8ba-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ab8ba-115">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab8ba-115">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ab8ba-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab8ba-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab8ba-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab8ba-117">Not supported.</span></span>|
|<span data-ttu-id="ab8ba-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab8ba-118">Application</span></span>|<span data-ttu-id="ab8ba-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab8ba-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab8ba-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab8ba-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="ab8ba-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab8ba-121">Request headers</span></span>
|<span data-ttu-id="ab8ba-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab8ba-122">Header</span></span>|<span data-ttu-id="ab8ba-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ab8ba-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab8ba-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab8ba-124">Authorization</span></span>|<span data-ttu-id="ab8ba-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ab8ba-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab8ba-126">Accept</span><span class="sxs-lookup"><span data-stu-id="ab8ba-126">Accept</span></span>|<span data-ttu-id="ab8ba-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ab8ba-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab8ba-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab8ba-128">Request body</span></span>
<span data-ttu-id="ab8ba-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab8ba-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab8ba-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab8ba-130">Response</span></span>
<span data-ttu-id="ab8ba-131">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab8ba-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab8ba-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ab8ba-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab8ba-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab8ba-133">Request</span></span>
<span data-ttu-id="ab8ba-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab8ba-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="ab8ba-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab8ba-135">Response</span></span>
<span data-ttu-id="ab8ba-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ab8ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



