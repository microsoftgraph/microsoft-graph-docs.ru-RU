---
title: Действие setMobileDeviceManagementAuthority
description: Задание центра управления мобильными устройствами
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d2f4c1ee79fa88b15dd8262ecc5c5bf8d5d08b60
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362150"
---
# <a name="setmobiledevicemanagementauthority-action"></a><span data-ttu-id="fd42a-103">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="fd42a-103">setMobileDeviceManagementAuthority action</span></span>

> <span data-ttu-id="fd42a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd42a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd42a-105">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="fd42a-105">Set mobile device management authority</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd42a-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fd42a-106">Prerequisites</span></span>
<span data-ttu-id="fd42a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd42a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd42a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd42a-109">Permission type</span></span>|<span data-ttu-id="fd42a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd42a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd42a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd42a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fd42a-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd42a-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fd42a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd42a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd42a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd42a-114">Not supported.</span></span>|
|<span data-ttu-id="fd42a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd42a-115">Application</span></span>|<span data-ttu-id="fd42a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd42a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd42a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd42a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/setMobileDeviceManagementAuthority
```

## <a name="request-headers"></a><span data-ttu-id="fd42a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd42a-118">Request headers</span></span>
|<span data-ttu-id="fd42a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd42a-119">Header</span></span>|<span data-ttu-id="fd42a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fd42a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd42a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd42a-121">Authorization</span></span>|<span data-ttu-id="fd42a-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd42a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd42a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fd42a-123">Accept</span></span>|<span data-ttu-id="fd42a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fd42a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd42a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd42a-125">Request body</span></span>
<span data-ttu-id="fd42a-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fd42a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd42a-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd42a-127">Response</span></span>
<span data-ttu-id="fd42a-128">При успешном выполнении это действие возвращает код отклика `200 OK` и объект Int32 в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fd42a-128">If successful, this action returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd42a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fd42a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd42a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd42a-130">Request</span></span>
<span data-ttu-id="fd42a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd42a-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/organization/{organizationId}/setMobileDeviceManagementAuthority
```

### <a name="response"></a><span data-ttu-id="fd42a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd42a-132">Response</span></span>
<span data-ttu-id="fd42a-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd42a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 2
}
```




