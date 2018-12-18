---
title: функция getManagedDevicesWithAppFailures
description: Получает список устройств, при помощи неудачных приложений
author: tfitzmac
ms.openlocfilehash: 147ee26644c3e2c425f70434516e13b03407891b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352957"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="225dd-103">функция getManagedDevicesWithAppFailures</span><span class="sxs-lookup"><span data-stu-id="225dd-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="225dd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="225dd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="225dd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="225dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="225dd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="225dd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="225dd-107">Получает список устройств, при помощи неудачных приложений</span><span class="sxs-lookup"><span data-stu-id="225dd-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="225dd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="225dd-108">Prerequisites</span></span>
<span data-ttu-id="225dd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="225dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="225dd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="225dd-111">Permission type</span></span>|<span data-ttu-id="225dd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="225dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="225dd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="225dd-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="225dd-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="225dd-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="225dd-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="225dd-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="225dd-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="225dd-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="225dd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="225dd-117">Not supported.</span></span>|
|<span data-ttu-id="225dd-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="225dd-118">Application</span></span>|<span data-ttu-id="225dd-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="225dd-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="225dd-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="225dd-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="225dd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="225dd-121">Request headers</span></span>
|<span data-ttu-id="225dd-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="225dd-122">Header</span></span>|<span data-ttu-id="225dd-123">Значение</span><span class="sxs-lookup"><span data-stu-id="225dd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="225dd-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="225dd-124">Authorization</span></span>|<span data-ttu-id="225dd-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="225dd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="225dd-126">Accept</span><span class="sxs-lookup"><span data-stu-id="225dd-126">Accept</span></span>|<span data-ttu-id="225dd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="225dd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="225dd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="225dd-128">Request body</span></span>
<span data-ttu-id="225dd-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="225dd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="225dd-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="225dd-130">Response</span></span>
<span data-ttu-id="225dd-131">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="225dd-131">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="225dd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="225dd-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="225dd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="225dd-133">Request</span></span>
<span data-ttu-id="225dd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="225dd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="225dd-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="225dd-135">Response</span></span>
<span data-ttu-id="225dd-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="225dd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





