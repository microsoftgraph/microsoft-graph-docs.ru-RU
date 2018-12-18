---
title: Функция verifyWindowsEnrollmentAutoDiscovery
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 3f981ae765981c067b08dc08dae96831f59d572b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344179"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="23b4a-103">Функция verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="23b4a-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="23b4a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="23b4a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23b4a-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="23b4a-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="23b4a-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="23b4a-106">Prerequisites</span></span>
<span data-ttu-id="23b4a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23b4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23b4a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23b4a-109">Permission type</span></span>|<span data-ttu-id="23b4a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="23b4a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23b4a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23b4a-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="23b4a-112">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="23b4a-112">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="23b4a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23b4a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="23b4a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23b4a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23b4a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23b4a-115">Not supported.</span></span>|
|<span data-ttu-id="23b4a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23b4a-116">Application</span></span>|<span data-ttu-id="23b4a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23b4a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23b4a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23b4a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="23b4a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23b4a-119">Request headers</span></span>
|<span data-ttu-id="23b4a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23b4a-120">Header</span></span>|<span data-ttu-id="23b4a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="23b4a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23b4a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23b4a-122">Authorization</span></span>|<span data-ttu-id="23b4a-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="23b4a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23b4a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="23b4a-124">Accept</span></span>|<span data-ttu-id="23b4a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="23b4a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23b4a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23b4a-126">Request body</span></span>
<span data-ttu-id="23b4a-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="23b4a-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="23b4a-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="23b4a-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="23b4a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="23b4a-129">Property</span></span>|<span data-ttu-id="23b4a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="23b4a-130">Type</span></span>|<span data-ttu-id="23b4a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="23b4a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23b4a-132">domainName</span><span class="sxs-lookup"><span data-stu-id="23b4a-132">domainName</span></span>|<span data-ttu-id="23b4a-133">String</span><span class="sxs-lookup"><span data-stu-id="23b4a-133">String</span></span>|<span data-ttu-id="23b4a-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="23b4a-134">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="23b4a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b4a-135">Response</span></span>
<span data-ttu-id="23b4a-136">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="23b4a-136">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23b4a-137">Пример</span><span class="sxs-lookup"><span data-stu-id="23b4a-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="23b4a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b4a-138">Request</span></span>
<span data-ttu-id="23b4a-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23b4a-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="23b4a-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="23b4a-140">Response</span></span>
<span data-ttu-id="23b4a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="23b4a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



