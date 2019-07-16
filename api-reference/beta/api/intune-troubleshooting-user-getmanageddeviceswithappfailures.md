---
title: Функция Жетманажеддевицесвисаппфаилурес
description: Получает список устройств с неудачными приложениями
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 576ce331a3339222877c63471ece0faee6f17982
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741478"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="be3c7-103">Функция Жетманажеддевицесвисаппфаилурес</span><span class="sxs-lookup"><span data-stu-id="be3c7-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="be3c7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be3c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be3c7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be3c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be3c7-106">Получает список устройств с неудачными приложениями</span><span class="sxs-lookup"><span data-stu-id="be3c7-106">Retrieves the list of devices with failed apps</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be3c7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="be3c7-107">Prerequisites</span></span>
<span data-ttu-id="be3c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be3c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be3c7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be3c7-110">Permission type</span></span>|<span data-ttu-id="be3c7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be3c7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be3c7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be3c7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="be3c7-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="be3c7-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="be3c7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be3c7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be3c7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be3c7-115">Not supported.</span></span>|
|<span data-ttu-id="be3c7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be3c7-116">Application</span></span>|<span data-ttu-id="be3c7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be3c7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be3c7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be3c7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="be3c7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be3c7-119">Request headers</span></span>
|<span data-ttu-id="be3c7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be3c7-120">Header</span></span>|<span data-ttu-id="be3c7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="be3c7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be3c7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be3c7-122">Authorization</span></span>|<span data-ttu-id="be3c7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be3c7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be3c7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="be3c7-124">Accept</span></span>|<span data-ttu-id="be3c7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="be3c7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be3c7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be3c7-126">Request body</span></span>
<span data-ttu-id="be3c7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be3c7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be3c7-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="be3c7-128">Response</span></span>
<span data-ttu-id="be3c7-129">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="be3c7-129">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be3c7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="be3c7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="be3c7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="be3c7-131">Request</span></span>
<span data-ttu-id="be3c7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be3c7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="be3c7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="be3c7-133">Response</span></span>
<span data-ttu-id="be3c7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be3c7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





