---
title: Действие setMobileDeviceManagementAuthority
description: Задание центра управления мобильными устройствами
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9f277b58973833151d08f12ef917c4341fe8cb11
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695441"
---
# <a name="setmobiledevicemanagementauthority-action"></a><span data-ttu-id="00299-103">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="00299-103">setMobileDeviceManagementAuthority action</span></span>

<span data-ttu-id="00299-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00299-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00299-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00299-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00299-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00299-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00299-107">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="00299-107">Set mobile device management authority</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00299-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="00299-108">Prerequisites</span></span>
<span data-ttu-id="00299-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00299-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00299-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00299-111">Permission type</span></span>|<span data-ttu-id="00299-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00299-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00299-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00299-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00299-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00299-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="00299-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00299-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00299-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00299-116">Not supported.</span></span>|
|<span data-ttu-id="00299-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00299-117">Application</span></span>|<span data-ttu-id="00299-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00299-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00299-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00299-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/setMobileDeviceManagementAuthority
```

## <a name="request-headers"></a><span data-ttu-id="00299-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="00299-120">Request headers</span></span>
|<span data-ttu-id="00299-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00299-121">Header</span></span>|<span data-ttu-id="00299-122">Значение</span><span class="sxs-lookup"><span data-stu-id="00299-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00299-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00299-123">Authorization</span></span>|<span data-ttu-id="00299-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00299-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00299-125">Accept</span><span class="sxs-lookup"><span data-stu-id="00299-125">Accept</span></span>|<span data-ttu-id="00299-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00299-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00299-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="00299-127">Request body</span></span>
<span data-ttu-id="00299-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00299-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00299-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="00299-129">Response</span></span>
<span data-ttu-id="00299-130">При успешном выполнении это действие возвращает код отклика `200 OK` и объект Int32 в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="00299-130">If successful, this action returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00299-131">Пример</span><span class="sxs-lookup"><span data-stu-id="00299-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="00299-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="00299-132">Request</span></span>
<span data-ttu-id="00299-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00299-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/organization/{organizationId}/setMobileDeviceManagementAuthority
```

### <a name="response"></a><span data-ttu-id="00299-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="00299-134">Response</span></span>
<span data-ttu-id="00299-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00299-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 2
}
```





