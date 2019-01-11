---
title: функция getManagedDevicesWithAppFailures
description: Получает список устройств, при помощи неудачных приложений
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cafda91617bfd183606877bfda352370f2364c9f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890071"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="5f89e-103">функция getManagedDevicesWithAppFailures</span><span class="sxs-lookup"><span data-stu-id="5f89e-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="5f89e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5f89e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f89e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f89e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f89e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5f89e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f89e-107">Получает список устройств, при помощи неудачных приложений</span><span class="sxs-lookup"><span data-stu-id="5f89e-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5f89e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5f89e-108">Prerequisites</span></span>
<span data-ttu-id="5f89e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f89e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f89e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f89e-111">Permission type</span></span>|<span data-ttu-id="5f89e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f89e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f89e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f89e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5f89e-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="5f89e-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="5f89e-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f89e-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5f89e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f89e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f89e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f89e-117">Not supported.</span></span>|
|<span data-ttu-id="5f89e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f89e-118">Application</span></span>|<span data-ttu-id="5f89e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f89e-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f89e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f89e-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="5f89e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f89e-121">Request headers</span></span>
|<span data-ttu-id="5f89e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5f89e-122">Header</span></span>|<span data-ttu-id="5f89e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5f89e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f89e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f89e-124">Authorization</span></span>|<span data-ttu-id="5f89e-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5f89e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f89e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5f89e-126">Accept</span></span>|<span data-ttu-id="5f89e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5f89e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f89e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5f89e-128">Request body</span></span>
<span data-ttu-id="5f89e-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f89e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f89e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5f89e-130">Response</span></span>
<span data-ttu-id="5f89e-131">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5f89e-131">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f89e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5f89e-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="5f89e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f89e-133">Request</span></span>
<span data-ttu-id="5f89e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f89e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="5f89e-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="5f89e-135">Response</span></span>
<span data-ttu-id="5f89e-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5f89e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 74

{
  "value": [
    "Get Managed Devices With App Failures value"
  ]
}
```





