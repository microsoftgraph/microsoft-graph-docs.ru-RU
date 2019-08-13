---
title: Функция Жетманажеддевицесвисаппфаилурес
description: Получает список устройств с неудачными приложениями
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40b1cd400935870682adb1b294e5af7bbadc07fd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350648"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="2837b-103">Функция Жетманажеддевицесвисаппфаилурес</span><span class="sxs-lookup"><span data-stu-id="2837b-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="2837b-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2837b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2837b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2837b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2837b-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2837b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2837b-107">Получает список устройств с неудачными приложениями</span><span class="sxs-lookup"><span data-stu-id="2837b-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2837b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2837b-108">Prerequisites</span></span>
<span data-ttu-id="2837b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2837b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2837b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2837b-111">Permission type</span></span>|<span data-ttu-id="2837b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2837b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2837b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2837b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2837b-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="2837b-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="2837b-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2837b-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="2837b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2837b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2837b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2837b-117">Not supported.</span></span>|
|<span data-ttu-id="2837b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2837b-118">Application</span></span>|<span data-ttu-id="2837b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2837b-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2837b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2837b-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="2837b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2837b-121">Request headers</span></span>
|<span data-ttu-id="2837b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2837b-122">Header</span></span>|<span data-ttu-id="2837b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2837b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2837b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2837b-124">Authorization</span></span>|<span data-ttu-id="2837b-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2837b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2837b-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2837b-126">Accept</span></span>|<span data-ttu-id="2837b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2837b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2837b-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2837b-128">Request body</span></span>
<span data-ttu-id="2837b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2837b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2837b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="2837b-130">Response</span></span>
<span data-ttu-id="2837b-131">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2837b-131">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2837b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2837b-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="2837b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2837b-133">Request</span></span>
<span data-ttu-id="2837b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2837b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="2837b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2837b-135">Response</span></span>
<span data-ttu-id="2837b-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2837b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








