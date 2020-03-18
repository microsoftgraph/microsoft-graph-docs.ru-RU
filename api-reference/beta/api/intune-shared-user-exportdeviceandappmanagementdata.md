---
title: Функция Експортдевицеандаппманажементдата
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 93c80b33a6598cd79d1f203a291cf61ff9f9d949
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800587"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="62b4e-103">Функция Експортдевицеандаппманажементдата</span><span class="sxs-lookup"><span data-stu-id="62b4e-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="62b4e-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="62b4e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="62b4e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62b4e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62b4e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62b4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62b4e-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="62b4e-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62b4e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="62b4e-108">Prerequisites</span></span>

<span data-ttu-id="62b4e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62b4e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62b4e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62b4e-111">Permission type</span></span>|<span data-ttu-id="62b4e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="62b4e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62b4e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62b4e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="62b4e-114">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="62b4e-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="62b4e-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62b4e-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="62b4e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62b4e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62b4e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62b4e-117">Not supported.</span></span>|
|<span data-ttu-id="62b4e-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="62b4e-118">Application</span></span>||
| <span data-ttu-id="62b4e-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="62b4e-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="62b4e-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62b4e-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62b4e-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62b4e-121">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="62b4e-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="62b4e-122">Request headers</span></span>

|<span data-ttu-id="62b4e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="62b4e-123">Header</span></span>|<span data-ttu-id="62b4e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="62b4e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62b4e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="62b4e-125">Authorization</span></span>|<span data-ttu-id="62b4e-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62b4e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62b4e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="62b4e-127">Accept</span></span>|<span data-ttu-id="62b4e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="62b4e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62b4e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62b4e-129">Request body</span></span>

<span data-ttu-id="62b4e-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="62b4e-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="62b4e-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="62b4e-131">Property</span></span>|<span data-ttu-id="62b4e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="62b4e-132">Type</span></span>|<span data-ttu-id="62b4e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="62b4e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62b4e-134">skip</span><span class="sxs-lookup"><span data-stu-id="62b4e-134">skip</span></span>|<span data-ttu-id="62b4e-135">Int32</span><span class="sxs-lookup"><span data-stu-id="62b4e-135">Int32</span></span>|<span data-ttu-id="62b4e-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="62b4e-136">Not yet documented</span></span>|
|<span data-ttu-id="62b4e-137">top</span><span class="sxs-lookup"><span data-stu-id="62b4e-137">top</span></span>|<span data-ttu-id="62b4e-138">Int32</span><span class="sxs-lookup"><span data-stu-id="62b4e-138">Int32</span></span>|<span data-ttu-id="62b4e-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="62b4e-139">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="62b4e-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="62b4e-140">Response</span></span>

<span data-ttu-id="62b4e-141">В случае успеха эта функция возвращает код `200 OK` отклика и объект [девицеандаппманажементдата](../resources/intune-onboarding-deviceandappmanagementdata.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62b4e-141">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62b4e-142">Пример</span><span class="sxs-lookup"><span data-stu-id="62b4e-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="62b4e-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="62b4e-143">Request</span></span>

<span data-ttu-id="62b4e-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62b4e-144">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="62b4e-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="62b4e-145">Response</span></span>

<span data-ttu-id="62b4e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="62b4e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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










