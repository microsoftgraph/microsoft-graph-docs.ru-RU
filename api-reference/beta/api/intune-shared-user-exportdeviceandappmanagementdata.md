---
title: Функция Експортдевицеандаппманажементдата
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a2e776d885a2f4374251fbb57b10377c03fbb8ec
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572301"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="c0c0e-103">Функция Експортдевицеандаппманажементдата</span><span class="sxs-lookup"><span data-stu-id="c0c0e-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="c0c0e-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c0c0e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0c0e-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0c0e-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0c0e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c0c0e-108">Prerequisites</span></span>

<span data-ttu-id="c0c0e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c0c0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c0c0e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0c0e-111">Permission type</span></span>|<span data-ttu-id="c0c0e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0c0e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0c0e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0c0e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c0c0e-114">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="c0c0e-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c0c0e-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0c0e-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c0c0e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0c0e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0c0e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-117">Not supported.</span></span>|
|<span data-ttu-id="c0c0e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0c0e-118">Application</span></span>|<span data-ttu-id="c0c0e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0c0e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0c0e-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="c0c0e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0c0e-121">Request headers</span></span>

|<span data-ttu-id="c0c0e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0c0e-122">Header</span></span>|<span data-ttu-id="c0c0e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c0c0e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0c0e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0c0e-124">Authorization</span></span>|<span data-ttu-id="c0c0e-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0c0e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c0c0e-126">Accept</span></span>|<span data-ttu-id="c0c0e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c0c0e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0c0e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0c0e-128">Request body</span></span>

<span data-ttu-id="c0c0e-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="c0c0e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0c0e-130">Property</span></span>|<span data-ttu-id="c0c0e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c0c0e-131">Type</span></span>|<span data-ttu-id="c0c0e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c0c0e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0c0e-133">skip</span><span class="sxs-lookup"><span data-stu-id="c0c0e-133">skip</span></span>|<span data-ttu-id="c0c0e-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c0c0e-134">Int32</span></span>|<span data-ttu-id="c0c0e-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-135">Not yet documented</span></span>|
|<span data-ttu-id="c0c0e-136">top</span><span class="sxs-lookup"><span data-stu-id="c0c0e-136">top</span></span>|<span data-ttu-id="c0c0e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c0c0e-137">Int32</span></span>|<span data-ttu-id="c0c0e-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c0c0e-138">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="c0c0e-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0c0e-139">Response</span></span>

<span data-ttu-id="c0c0e-140">В случае успеха эта функция возвращает код `200 OK` отклика и объект [девицеандаппманажементдата](../resources/intune-onboarding-deviceandappmanagementdata.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-140">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0c0e-141">Пример</span><span class="sxs-lookup"><span data-stu-id="c0c0e-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0c0e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0c0e-142">Request</span></span>

<span data-ttu-id="c0c0e-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="c0c0e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0c0e-144">Response</span></span>

<span data-ttu-id="c0c0e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



