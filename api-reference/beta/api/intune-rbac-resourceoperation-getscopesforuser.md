---
title: Функция Getscopesforuser к объекту
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 51f07c7d1401b453e7cf3131fb319aa0290aed63
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36351366"
---
# <a name="getscopesforuser-function"></a><span data-ttu-id="fbdb8-103">Функция Getscopesforuser к объекту</span><span class="sxs-lookup"><span data-stu-id="fbdb8-103">getScopesForUser function</span></span>

> <span data-ttu-id="fbdb8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbdb8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbdb8-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbdb8-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fbdb8-107">Prerequisites</span></span>
<span data-ttu-id="fbdb8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbdb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbdb8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbdb8-110">Permission type</span></span>|<span data-ttu-id="fbdb8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbdb8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbdb8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbdb8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fbdb8-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbdb8-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="fbdb8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbdb8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbdb8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-115">Not supported.</span></span>|
|<span data-ttu-id="fbdb8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbdb8-116">Application</span></span>|<span data-ttu-id="fbdb8-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbdb8-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbdb8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbdb8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser
```

## <a name="request-headers"></a><span data-ttu-id="fbdb8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbdb8-119">Request headers</span></span>
|<span data-ttu-id="fbdb8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fbdb8-120">Header</span></span>|<span data-ttu-id="fbdb8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fbdb8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbdb8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbdb8-122">Authorization</span></span>|<span data-ttu-id="fbdb8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbdb8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fbdb8-124">Accept</span></span>|<span data-ttu-id="fbdb8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fbdb8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbdb8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fbdb8-126">Request body</span></span>
<span data-ttu-id="fbdb8-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="fbdb8-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="fbdb8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbdb8-129">Property</span></span>|<span data-ttu-id="fbdb8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fbdb8-130">Type</span></span>|<span data-ttu-id="fbdb8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fbdb8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbdb8-132">UserID</span><span class="sxs-lookup"><span data-stu-id="fbdb8-132">userid</span></span>|<span data-ttu-id="fbdb8-133">String</span><span class="sxs-lookup"><span data-stu-id="fbdb8-133">String</span></span>|<span data-ttu-id="fbdb8-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fbdb8-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fbdb8-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="fbdb8-135">Response</span></span>
<span data-ttu-id="fbdb8-136">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-136">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbdb8-137">Пример</span><span class="sxs-lookup"><span data-stu-id="fbdb8-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbdb8-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbdb8-138">Request</span></span>
<span data-ttu-id="fbdb8-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser(userid='parameterValue')
```

### <a name="response"></a><span data-ttu-id="fbdb8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbdb8-140">Response</span></span>
<span data-ttu-id="fbdb8-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbdb8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": [
    "Get Scopes For User value"
  ]
}
```






