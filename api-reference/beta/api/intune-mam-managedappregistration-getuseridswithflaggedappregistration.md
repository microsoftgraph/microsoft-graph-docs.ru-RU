---
title: Функция getUserIdsWithFlaggedAppRegistration
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 65848b44c0b4228d1df4c5e7ea0e0024e16598eb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139328"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="e24bc-103">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e24bc-103">getUserIdsWithFlaggedAppRegistration function</span></span>

> <span data-ttu-id="e24bc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e24bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e24bc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e24bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e24bc-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e24bc-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e24bc-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e24bc-107">Prerequisites</span></span>
<span data-ttu-id="e24bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e24bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e24bc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e24bc-110">Permission type</span></span>|<span data-ttu-id="e24bc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e24bc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e24bc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e24bc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e24bc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e24bc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e24bc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e24bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e24bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e24bc-115">Not supported.</span></span>|
|<span data-ttu-id="e24bc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e24bc-116">Application</span></span>|<span data-ttu-id="e24bc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e24bc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e24bc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e24bc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="e24bc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e24bc-119">Request headers</span></span>
|<span data-ttu-id="e24bc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e24bc-120">Header</span></span>|<span data-ttu-id="e24bc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e24bc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e24bc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e24bc-122">Authorization</span></span>|<span data-ttu-id="e24bc-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e24bc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e24bc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e24bc-124">Accept</span></span>|<span data-ttu-id="e24bc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e24bc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e24bc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e24bc-126">Request body</span></span>
<span data-ttu-id="e24bc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e24bc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e24bc-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e24bc-128">Response</span></span>
<span data-ttu-id="e24bc-129">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e24bc-129">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e24bc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e24bc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e24bc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e24bc-131">Request</span></span>
<span data-ttu-id="e24bc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e24bc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="e24bc-133">Отклик
</span><span class="sxs-lookup"><span data-stu-id="e24bc-133">Response</span></span>
<span data-ttu-id="e24bc-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e24bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": [
    "Get User Ids With Flagged App Registration value"
  ]
}
```




