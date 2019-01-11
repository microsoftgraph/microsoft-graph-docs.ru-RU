---
title: функция getScopesForUser
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b0cd9a14602ce090de5d79720415a1e52d3b3145
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822423"
---
# <a name="getscopesforuser-function"></a><span data-ttu-id="ac083-103">функция getScopesForUser</span><span class="sxs-lookup"><span data-stu-id="ac083-103">getScopesForUser function</span></span>

> <span data-ttu-id="ac083-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ac083-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac083-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac083-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ac083-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ac083-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac083-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ac083-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ac083-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ac083-108">Prerequisites</span></span>
<span data-ttu-id="ac083-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac083-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac083-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac083-111">Permission type</span></span>|<span data-ttu-id="ac083-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac083-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac083-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac083-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ac083-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac083-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="ac083-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac083-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac083-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac083-116">Not supported.</span></span>|
|<span data-ttu-id="ac083-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac083-117">Application</span></span>|<span data-ttu-id="ac083-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac083-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac083-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac083-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser
```

## <a name="request-headers"></a><span data-ttu-id="ac083-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac083-120">Request headers</span></span>
|<span data-ttu-id="ac083-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ac083-121">Header</span></span>|<span data-ttu-id="ac083-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ac083-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac083-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac083-123">Authorization</span></span>|<span data-ttu-id="ac083-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ac083-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac083-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ac083-125">Accept</span></span>|<span data-ttu-id="ac083-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac083-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac083-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ac083-127">Request body</span></span>
<span data-ttu-id="ac083-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ac083-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ac083-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="ac083-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ac083-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac083-130">Property</span></span>|<span data-ttu-id="ac083-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ac083-131">Type</span></span>|<span data-ttu-id="ac083-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ac083-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac083-133">идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="ac083-133">userid</span></span>|<span data-ttu-id="ac083-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ac083-134">String</span></span>|<span data-ttu-id="ac083-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ac083-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ac083-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="ac083-136">Response</span></span>
<span data-ttu-id="ac083-137">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ac083-137">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac083-138">Пример</span><span class="sxs-lookup"><span data-stu-id="ac083-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="ac083-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac083-139">Request</span></span>
<span data-ttu-id="ac083-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac083-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser(userid='parameterValue')
```

### <a name="response"></a><span data-ttu-id="ac083-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="ac083-141">Response</span></span>
<span data-ttu-id="ac083-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ac083-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





