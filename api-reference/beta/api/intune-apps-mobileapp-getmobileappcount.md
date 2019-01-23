---
title: функция getMobileAppCount
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eab7f9074da1a0aabc33d89108078e6a34a53519
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397780"
---
# <a name="getmobileappcount-function"></a><span data-ttu-id="9366b-103">функция getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="9366b-103">getMobileAppCount function</span></span>

> <span data-ttu-id="9366b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9366b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9366b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9366b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9366b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9366b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9366b-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9366b-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9366b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9366b-108">Prerequisites</span></span>
<span data-ttu-id="9366b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9366b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9366b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9366b-111">Permission type</span></span>|<span data-ttu-id="9366b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9366b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9366b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9366b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9366b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9366b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9366b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9366b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9366b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9366b-116">Not supported.</span></span>|
|<span data-ttu-id="9366b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9366b-117">Application</span></span>|<span data-ttu-id="9366b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9366b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9366b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9366b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getMobileAppCount
```

## <a name="request-headers"></a><span data-ttu-id="9366b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9366b-120">Request headers</span></span>
|<span data-ttu-id="9366b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9366b-121">Header</span></span>|<span data-ttu-id="9366b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9366b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9366b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9366b-123">Authorization</span></span>|<span data-ttu-id="9366b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9366b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9366b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9366b-125">Accept</span></span>|<span data-ttu-id="9366b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9366b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9366b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9366b-127">Request body</span></span>
<span data-ttu-id="9366b-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="9366b-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="9366b-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="9366b-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="9366b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9366b-130">Property</span></span>|<span data-ttu-id="9366b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9366b-131">Type</span></span>|<span data-ttu-id="9366b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9366b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9366b-133">status</span><span class="sxs-lookup"><span data-stu-id="9366b-133">status</span></span>|<span data-ttu-id="9366b-134">String</span><span class="sxs-lookup"><span data-stu-id="9366b-134">String</span></span>|<span data-ttu-id="9366b-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9366b-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9366b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9366b-136">Response</span></span>
<span data-ttu-id="9366b-137">Если успешно завершена, эта функция возвращает `200 OK` код ответа и Int64 в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9366b-137">If successful, this function returns a `200 OK` response code and a Int64 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9366b-138">Пример</span><span class="sxs-lookup"><span data-stu-id="9366b-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="9366b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9366b-139">Request</span></span>
<span data-ttu-id="9366b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9366b-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getMobileAppCount(status='parameterValue')
```

### <a name="response"></a><span data-ttu-id="9366b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9366b-141">Response</span></span>
<span data-ttu-id="9366b-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9366b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 1
}
```




