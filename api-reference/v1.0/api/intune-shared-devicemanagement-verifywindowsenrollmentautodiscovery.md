---
title: Функция verifyWindowsEnrollmentAutoDiscovery
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 179c0b34f1ecd22c29ec178e0d7935677fdb0be9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025895"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="0f0ee-103">Функция verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="0f0ee-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="0f0ee-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f0ee-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f0ee-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0f0ee-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f0ee-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0f0ee-106">Prerequisites</span></span>
<span data-ttu-id="0f0ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f0ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f0ee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f0ee-109">Permission type</span></span>|<span data-ttu-id="0f0ee-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f0ee-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f0ee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f0ee-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0f0ee-112">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="0f0ee-112">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="0f0ee-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f0ee-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0f0ee-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f0ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f0ee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f0ee-115">Not supported.</span></span>|
|<span data-ttu-id="0f0ee-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f0ee-116">Application</span></span>|<span data-ttu-id="0f0ee-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f0ee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f0ee-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f0ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="0f0ee-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f0ee-119">Request headers</span></span>
|<span data-ttu-id="0f0ee-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0f0ee-120">Header</span></span>|<span data-ttu-id="0f0ee-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0f0ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f0ee-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f0ee-122">Authorization</span></span>|<span data-ttu-id="0f0ee-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f0ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f0ee-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0f0ee-124">Accept</span></span>|<span data-ttu-id="0f0ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0f0ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f0ee-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0f0ee-126">Request body</span></span>
<span data-ttu-id="0f0ee-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="0f0ee-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="0f0ee-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="0f0ee-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="0f0ee-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f0ee-129">Property</span></span>|<span data-ttu-id="0f0ee-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0f0ee-130">Type</span></span>|<span data-ttu-id="0f0ee-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0f0ee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f0ee-132">domainName</span><span class="sxs-lookup"><span data-stu-id="0f0ee-132">domainName</span></span>|<span data-ttu-id="0f0ee-133">String</span><span class="sxs-lookup"><span data-stu-id="0f0ee-133">String</span></span>|<span data-ttu-id="0f0ee-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0f0ee-134">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="0f0ee-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f0ee-135">Response</span></span>
<span data-ttu-id="0f0ee-136">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0f0ee-136">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f0ee-137">Пример</span><span class="sxs-lookup"><span data-stu-id="0f0ee-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f0ee-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f0ee-138">Request</span></span>
<span data-ttu-id="0f0ee-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f0ee-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="0f0ee-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f0ee-140">Response</span></span>
<span data-ttu-id="0f0ee-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0f0ee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



