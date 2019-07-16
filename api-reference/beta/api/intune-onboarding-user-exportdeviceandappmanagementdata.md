---
title: Функция Експортдевицеандаппманажементдата
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9fd7b9ddcf82ce8ec65e2e58d97ea1a8b08f2ea7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741510"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="34a5e-103">Функция Експортдевицеандаппманажементдата</span><span class="sxs-lookup"><span data-stu-id="34a5e-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="34a5e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34a5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34a5e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34a5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34a5e-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="34a5e-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34a5e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="34a5e-107">Prerequisites</span></span>
<span data-ttu-id="34a5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34a5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34a5e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34a5e-110">Permission type</span></span>|<span data-ttu-id="34a5e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="34a5e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34a5e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34a5e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34a5e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="34a5e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="34a5e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34a5e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34a5e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34a5e-115">Not supported.</span></span>|
|<span data-ttu-id="34a5e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34a5e-116">Application</span></span>|<span data-ttu-id="34a5e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34a5e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34a5e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34a5e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="34a5e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34a5e-119">Request headers</span></span>
|<span data-ttu-id="34a5e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34a5e-120">Header</span></span>|<span data-ttu-id="34a5e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="34a5e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34a5e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34a5e-122">Authorization</span></span>|<span data-ttu-id="34a5e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34a5e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34a5e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="34a5e-124">Accept</span></span>|<span data-ttu-id="34a5e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34a5e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34a5e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="34a5e-126">Request body</span></span>
<span data-ttu-id="34a5e-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="34a5e-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="34a5e-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="34a5e-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="34a5e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="34a5e-129">Property</span></span>|<span data-ttu-id="34a5e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="34a5e-130">Type</span></span>|<span data-ttu-id="34a5e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="34a5e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34a5e-132">skip</span><span class="sxs-lookup"><span data-stu-id="34a5e-132">skip</span></span>|<span data-ttu-id="34a5e-133">Int32</span><span class="sxs-lookup"><span data-stu-id="34a5e-133">Int32</span></span>|<span data-ttu-id="34a5e-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="34a5e-134">Not yet documented</span></span>|
|<span data-ttu-id="34a5e-135">top</span><span class="sxs-lookup"><span data-stu-id="34a5e-135">top</span></span>|<span data-ttu-id="34a5e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="34a5e-136">Int32</span></span>|<span data-ttu-id="34a5e-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="34a5e-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="34a5e-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="34a5e-138">Response</span></span>
<span data-ttu-id="34a5e-139">В случае успеха эта функция возвращает код `200 OK` отклика и объект [девицеандаппманажементдата](../resources/intune-onboarding-deviceandappmanagementdata.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34a5e-139">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34a5e-140">Пример</span><span class="sxs-lookup"><span data-stu-id="34a5e-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="34a5e-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="34a5e-141">Request</span></span>
<span data-ttu-id="34a5e-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34a5e-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="34a5e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="34a5e-143">Response</span></span>
<span data-ttu-id="34a5e-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34a5e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 143

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementData",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```





