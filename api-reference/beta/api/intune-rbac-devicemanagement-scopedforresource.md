---
title: Функция Скопедфорресаурце
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f49981a46d8e11ef9880edb236d199251c63bb97
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43421252"
---
# <a name="scopedforresource-function"></a><span data-ttu-id="77e32-103">Функция Скопедфорресаурце</span><span class="sxs-lookup"><span data-stu-id="77e32-103">scopedForResource function</span></span>

<span data-ttu-id="77e32-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77e32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77e32-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77e32-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77e32-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77e32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77e32-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="77e32-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77e32-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="77e32-108">Prerequisites</span></span>
<span data-ttu-id="77e32-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77e32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77e32-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77e32-111">Permission type</span></span>|<span data-ttu-id="77e32-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="77e32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77e32-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77e32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77e32-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="77e32-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="77e32-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77e32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77e32-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77e32-116">Not supported.</span></span>|
|<span data-ttu-id="77e32-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="77e32-117">Application</span></span>|<span data-ttu-id="77e32-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="77e32-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77e32-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77e32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/scopedForResource
```

## <a name="request-headers"></a><span data-ttu-id="77e32-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="77e32-120">Request headers</span></span>
|<span data-ttu-id="77e32-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77e32-121">Header</span></span>|<span data-ttu-id="77e32-122">Значение</span><span class="sxs-lookup"><span data-stu-id="77e32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77e32-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77e32-123">Authorization</span></span>|<span data-ttu-id="77e32-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77e32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77e32-125">Accept</span><span class="sxs-lookup"><span data-stu-id="77e32-125">Accept</span></span>|<span data-ttu-id="77e32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77e32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77e32-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77e32-127">Request body</span></span>
<span data-ttu-id="77e32-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="77e32-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="77e32-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="77e32-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="77e32-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="77e32-130">Property</span></span>|<span data-ttu-id="77e32-131">Тип</span><span class="sxs-lookup"><span data-stu-id="77e32-131">Type</span></span>|<span data-ttu-id="77e32-132">Описание</span><span class="sxs-lookup"><span data-stu-id="77e32-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77e32-133">resource</span><span class="sxs-lookup"><span data-stu-id="77e32-133">resource</span></span>|<span data-ttu-id="77e32-134">String</span><span class="sxs-lookup"><span data-stu-id="77e32-134">String</span></span>|<span data-ttu-id="77e32-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="77e32-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="77e32-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="77e32-136">Response</span></span>
<span data-ttu-id="77e32-137">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="77e32-137">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77e32-138">Пример</span><span class="sxs-lookup"><span data-stu-id="77e32-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="77e32-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="77e32-139">Request</span></span>
<span data-ttu-id="77e32-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77e32-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/scopedForResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="77e32-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="77e32-141">Response</span></span>
<span data-ttu-id="77e32-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77e32-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



