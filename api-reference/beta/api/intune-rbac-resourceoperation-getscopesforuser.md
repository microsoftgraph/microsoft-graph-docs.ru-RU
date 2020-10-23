---
title: Функция Getscopesforuser к объекту
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ee3fb7a60c8906500b62ac11f4ab3fd5bdf5c849
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695245"
---
# <a name="getscopesforuser-function"></a><span data-ttu-id="a111a-103">Функция Getscopesforuser к объекту</span><span class="sxs-lookup"><span data-stu-id="a111a-103">getScopesForUser function</span></span>

<span data-ttu-id="a111a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a111a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a111a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a111a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a111a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a111a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a111a-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a111a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a111a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a111a-108">Prerequisites</span></span>
<span data-ttu-id="a111a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a111a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a111a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a111a-111">Permission type</span></span>|<span data-ttu-id="a111a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a111a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a111a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a111a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a111a-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a111a-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a111a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a111a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a111a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a111a-116">Not supported.</span></span>|
|<span data-ttu-id="a111a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a111a-117">Application</span></span>|<span data-ttu-id="a111a-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a111a-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a111a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a111a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser
```

## <a name="request-headers"></a><span data-ttu-id="a111a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a111a-120">Request headers</span></span>
|<span data-ttu-id="a111a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a111a-121">Header</span></span>|<span data-ttu-id="a111a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a111a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a111a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a111a-123">Authorization</span></span>|<span data-ttu-id="a111a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a111a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a111a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a111a-125">Accept</span></span>|<span data-ttu-id="a111a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a111a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a111a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a111a-127">Request body</span></span>
<span data-ttu-id="a111a-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="a111a-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="a111a-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="a111a-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a111a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a111a-130">Property</span></span>|<span data-ttu-id="a111a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a111a-131">Type</span></span>|<span data-ttu-id="a111a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a111a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a111a-133">UserID</span><span class="sxs-lookup"><span data-stu-id="a111a-133">userid</span></span>|<span data-ttu-id="a111a-134">String</span><span class="sxs-lookup"><span data-stu-id="a111a-134">String</span></span>|<span data-ttu-id="a111a-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a111a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a111a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a111a-136">Response</span></span>
<span data-ttu-id="a111a-137">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a111a-137">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a111a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a111a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a111a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a111a-139">Request</span></span>
<span data-ttu-id="a111a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a111a-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser(userid='parameterValue')
```

### <a name="response"></a><span data-ttu-id="a111a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a111a-141">Response</span></span>
<span data-ttu-id="a111a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a111a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





