---
title: функция exportDeviceAndAppManagementData
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e36936710bcd97c10c4a69c496cf56ceffa43e46
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409239"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="70ca2-103">функция exportDeviceAndAppManagementData</span><span class="sxs-lookup"><span data-stu-id="70ca2-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="70ca2-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="70ca2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="70ca2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70ca2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70ca2-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70ca2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70ca2-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="70ca2-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70ca2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="70ca2-108">Prerequisites</span></span>

<span data-ttu-id="70ca2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70ca2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70ca2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70ca2-111">Permission type</span></span>|<span data-ttu-id="70ca2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="70ca2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70ca2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70ca2-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="70ca2-114">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="70ca2-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="70ca2-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70ca2-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="70ca2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70ca2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70ca2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70ca2-117">Not supported.</span></span>|
|<span data-ttu-id="70ca2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70ca2-118">Application</span></span>|<span data-ttu-id="70ca2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70ca2-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70ca2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70ca2-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="70ca2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70ca2-121">Request headers</span></span>

|<span data-ttu-id="70ca2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70ca2-122">Header</span></span>|<span data-ttu-id="70ca2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="70ca2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70ca2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="70ca2-124">Authorization</span></span>|<span data-ttu-id="70ca2-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="70ca2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70ca2-126">Accept</span><span class="sxs-lookup"><span data-stu-id="70ca2-126">Accept</span></span>|<span data-ttu-id="70ca2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="70ca2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70ca2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70ca2-128">Request body</span></span>

<span data-ttu-id="70ca2-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="70ca2-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="70ca2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="70ca2-130">Property</span></span>|<span data-ttu-id="70ca2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="70ca2-131">Type</span></span>|<span data-ttu-id="70ca2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="70ca2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70ca2-133">skip</span><span class="sxs-lookup"><span data-stu-id="70ca2-133">skip</span></span>|<span data-ttu-id="70ca2-134">Int32</span><span class="sxs-lookup"><span data-stu-id="70ca2-134">Int32</span></span>|<span data-ttu-id="70ca2-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="70ca2-135">Not yet documented</span></span>|
|<span data-ttu-id="70ca2-136">top</span><span class="sxs-lookup"><span data-stu-id="70ca2-136">top</span></span>|<span data-ttu-id="70ca2-137">Int32</span><span class="sxs-lookup"><span data-stu-id="70ca2-137">Int32</span></span>|<span data-ttu-id="70ca2-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="70ca2-138">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="70ca2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="70ca2-139">Response</span></span>

<span data-ttu-id="70ca2-140">Если успешно завершена, эта функция возвращает `200 OK` код ответа и [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="70ca2-140">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70ca2-141">Пример</span><span class="sxs-lookup"><span data-stu-id="70ca2-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="70ca2-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="70ca2-142">Request</span></span>

<span data-ttu-id="70ca2-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70ca2-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="70ca2-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="70ca2-144">Response</span></span>

<span data-ttu-id="70ca2-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="70ca2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



