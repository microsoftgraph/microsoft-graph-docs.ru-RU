---
title: Функция Getscopesforuser к объекту
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ad3136187fa773348fa3e6da3753934a2bc1730f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459795"
---
# <a name="getscopesforuser-function"></a><span data-ttu-id="53fa0-103">Функция Getscopesforuser к объекту</span><span class="sxs-lookup"><span data-stu-id="53fa0-103">getScopesForUser function</span></span>

<span data-ttu-id="53fa0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="53fa0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53fa0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53fa0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53fa0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53fa0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53fa0-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="53fa0-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53fa0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="53fa0-108">Prerequisites</span></span>
<span data-ttu-id="53fa0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53fa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53fa0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53fa0-111">Permission type</span></span>|<span data-ttu-id="53fa0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53fa0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53fa0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53fa0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53fa0-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="53fa0-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="53fa0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53fa0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53fa0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53fa0-116">Not supported.</span></span>|
|<span data-ttu-id="53fa0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53fa0-117">Application</span></span>|<span data-ttu-id="53fa0-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="53fa0-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53fa0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53fa0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser
```

## <a name="request-headers"></a><span data-ttu-id="53fa0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="53fa0-120">Request headers</span></span>
|<span data-ttu-id="53fa0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53fa0-121">Header</span></span>|<span data-ttu-id="53fa0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="53fa0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53fa0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53fa0-123">Authorization</span></span>|<span data-ttu-id="53fa0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53fa0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53fa0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="53fa0-125">Accept</span></span>|<span data-ttu-id="53fa0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53fa0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53fa0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53fa0-127">Request body</span></span>
<span data-ttu-id="53fa0-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="53fa0-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="53fa0-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="53fa0-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="53fa0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="53fa0-130">Property</span></span>|<span data-ttu-id="53fa0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="53fa0-131">Type</span></span>|<span data-ttu-id="53fa0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="53fa0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53fa0-133">UserID</span><span class="sxs-lookup"><span data-stu-id="53fa0-133">userid</span></span>|<span data-ttu-id="53fa0-134">String</span><span class="sxs-lookup"><span data-stu-id="53fa0-134">String</span></span>|<span data-ttu-id="53fa0-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="53fa0-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="53fa0-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="53fa0-136">Response</span></span>
<span data-ttu-id="53fa0-137">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="53fa0-137">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53fa0-138">Пример</span><span class="sxs-lookup"><span data-stu-id="53fa0-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="53fa0-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="53fa0-139">Request</span></span>
<span data-ttu-id="53fa0-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53fa0-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser(userid='parameterValue')
```

### <a name="response"></a><span data-ttu-id="53fa0-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="53fa0-141">Response</span></span>
<span data-ttu-id="53fa0-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53fa0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





