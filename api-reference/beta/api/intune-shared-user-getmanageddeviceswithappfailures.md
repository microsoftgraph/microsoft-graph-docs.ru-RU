---
title: Функция Жетманажеддевицесвисаппфаилурес
description: Получает список устройств с неудачными приложениями
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5796100578a66899c69152d0bdb65ffe42675e34
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085544"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="31c16-103">Функция Жетманажеддевицесвисаппфаилурес</span><span class="sxs-lookup"><span data-stu-id="31c16-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="31c16-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="31c16-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="31c16-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31c16-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31c16-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31c16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31c16-107">Получает список устройств с неудачными приложениями</span><span class="sxs-lookup"><span data-stu-id="31c16-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="31c16-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="31c16-108">Prerequisites</span></span>
<span data-ttu-id="31c16-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31c16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31c16-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31c16-111">Permission type</span></span>|<span data-ttu-id="31c16-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="31c16-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31c16-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31c16-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="31c16-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="31c16-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="31c16-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="31c16-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="31c16-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31c16-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31c16-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31c16-117">Not supported.</span></span>|
|<span data-ttu-id="31c16-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31c16-118">Application</span></span>||
| <span data-ttu-id="31c16-119">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="31c16-119">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="31c16-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="31c16-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31c16-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31c16-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="31c16-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="31c16-122">Request headers</span></span>
|<span data-ttu-id="31c16-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="31c16-123">Header</span></span>|<span data-ttu-id="31c16-124">Значение</span><span class="sxs-lookup"><span data-stu-id="31c16-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31c16-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31c16-125">Authorization</span></span>|<span data-ttu-id="31c16-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31c16-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31c16-127">Accept</span><span class="sxs-lookup"><span data-stu-id="31c16-127">Accept</span></span>|<span data-ttu-id="31c16-128">application/json</span><span class="sxs-lookup"><span data-stu-id="31c16-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31c16-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31c16-129">Request body</span></span>
<span data-ttu-id="31c16-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="31c16-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31c16-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="31c16-131">Response</span></span>
<span data-ttu-id="31c16-132">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="31c16-132">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31c16-133">Пример</span><span class="sxs-lookup"><span data-stu-id="31c16-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="31c16-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="31c16-134">Request</span></span>
<span data-ttu-id="31c16-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31c16-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="31c16-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="31c16-136">Response</span></span>
<span data-ttu-id="31c16-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31c16-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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














