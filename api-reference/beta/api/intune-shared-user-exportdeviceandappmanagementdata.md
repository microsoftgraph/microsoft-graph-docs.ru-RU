---
title: функция exportDeviceAndAppManagementData
description: Н/Д
ms.openlocfilehash: fdcf75817d3fae157480b4e232bf4052ac84f64b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075811"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="c1c7b-103">функция exportDeviceAndAppManagementData</span><span class="sxs-lookup"><span data-stu-id="c1c7b-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="c1c7b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c1c7b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1c7b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1c7b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1c7b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c1c7b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1c7b-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c1c7b-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1c7b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c1c7b-108">Prerequisites</span></span>

<span data-ttu-id="c1c7b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1c7b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1c7b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1c7b-111">Permission type</span></span>|<span data-ttu-id="c1c7b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1c7b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1c7b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1c7b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c1c7b-114">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="c1c7b-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c1c7b-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1c7b-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c1c7b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1c7b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1c7b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1c7b-117">Not supported.</span></span>|
|<span data-ttu-id="c1c7b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1c7b-118">Application</span></span>|<span data-ttu-id="c1c7b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1c7b-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1c7b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1c7b-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="c1c7b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1c7b-121">Request headers</span></span>

|<span data-ttu-id="c1c7b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1c7b-122">Header</span></span>|<span data-ttu-id="c1c7b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c1c7b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1c7b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1c7b-124">Authorization</span></span>|<span data-ttu-id="c1c7b-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c1c7b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1c7b-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c1c7b-126">Accept</span></span>|<span data-ttu-id="c1c7b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c1c7b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1c7b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1c7b-128">Request body</span></span>

<span data-ttu-id="c1c7b-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="c1c7b-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="c1c7b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1c7b-130">Property</span></span>|<span data-ttu-id="c1c7b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c1c7b-131">Type</span></span>|<span data-ttu-id="c1c7b-132">Description</span><span class="sxs-lookup"><span data-stu-id="c1c7b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1c7b-133">skip</span><span class="sxs-lookup"><span data-stu-id="c1c7b-133">skip</span></span>|<span data-ttu-id="c1c7b-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c1c7b-134">Int32</span></span>|<span data-ttu-id="c1c7b-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c1c7b-135">Not yet documented</span></span>|
|<span data-ttu-id="c1c7b-136">top</span><span class="sxs-lookup"><span data-stu-id="c1c7b-136">top</span></span>|<span data-ttu-id="c1c7b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c1c7b-137">Int32</span></span>|<span data-ttu-id="c1c7b-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c1c7b-138">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="c1c7b-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1c7b-139">Response</span></span>

<span data-ttu-id="c1c7b-140">Если успешно завершена, эта функция возвращает `200 OK` код ответа и [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c1c7b-140">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1c7b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="c1c7b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1c7b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1c7b-142">Request</span></span>

<span data-ttu-id="c1c7b-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1c7b-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="c1c7b-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1c7b-144">Response</span></span>

<span data-ttu-id="c1c7b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c1c7b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



