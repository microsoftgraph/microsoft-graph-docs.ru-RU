---
title: функция getScopesForUser
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 383e4cf835b8f056af707367b3664e0bac4a59a1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396170"
---
# <a name="getscopesforuser-function"></a><span data-ttu-id="fd3f9-103">функция getScopesForUser</span><span class="sxs-lookup"><span data-stu-id="fd3f9-103">getScopesForUser function</span></span>

> <span data-ttu-id="fd3f9-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fd3f9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fd3f9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd3f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd3f9-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd3f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd3f9-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fd3f9-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd3f9-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fd3f9-108">Prerequisites</span></span>
<span data-ttu-id="fd3f9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fd3f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fd3f9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd3f9-111">Permission type</span></span>|<span data-ttu-id="fd3f9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd3f9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd3f9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd3f9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fd3f9-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd3f9-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="fd3f9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd3f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd3f9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd3f9-116">Not supported.</span></span>|
|<span data-ttu-id="fd3f9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd3f9-117">Application</span></span>|<span data-ttu-id="fd3f9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd3f9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd3f9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd3f9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser
```

## <a name="request-headers"></a><span data-ttu-id="fd3f9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd3f9-120">Request headers</span></span>
|<span data-ttu-id="fd3f9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd3f9-121">Header</span></span>|<span data-ttu-id="fd3f9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fd3f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd3f9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd3f9-123">Authorization</span></span>|<span data-ttu-id="fd3f9-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fd3f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd3f9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fd3f9-125">Accept</span></span>|<span data-ttu-id="fd3f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fd3f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd3f9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd3f9-127">Request body</span></span>
<span data-ttu-id="fd3f9-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="fd3f9-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="fd3f9-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="fd3f9-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="fd3f9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd3f9-130">Property</span></span>|<span data-ttu-id="fd3f9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fd3f9-131">Type</span></span>|<span data-ttu-id="fd3f9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fd3f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd3f9-133">идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="fd3f9-133">userid</span></span>|<span data-ttu-id="fd3f9-134">String</span><span class="sxs-lookup"><span data-stu-id="fd3f9-134">String</span></span>|<span data-ttu-id="fd3f9-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fd3f9-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fd3f9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd3f9-136">Response</span></span>
<span data-ttu-id="fd3f9-137">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fd3f9-137">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd3f9-138">Пример</span><span class="sxs-lookup"><span data-stu-id="fd3f9-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd3f9-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd3f9-139">Request</span></span>
<span data-ttu-id="fd3f9-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd3f9-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser(userid='parameterValue')
```

### <a name="response"></a><span data-ttu-id="fd3f9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd3f9-141">Response</span></span>
<span data-ttu-id="fd3f9-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fd3f9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




