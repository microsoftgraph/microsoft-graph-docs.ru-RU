---
title: Функция getUserIdsWithFlaggedAppRegistration
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 7f57ab3af48ac7e815b914be3339435d6be58fc4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329381"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="9cb0a-103">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="9cb0a-103">getUserIdsWithFlaggedAppRegistration function</span></span>

> <span data-ttu-id="9cb0a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9cb0a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9cb0a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9cb0a-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9cb0a-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9cb0a-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9cb0a-108">Prerequisites</span></span>
<span data-ttu-id="9cb0a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cb0a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cb0a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9cb0a-111">Permission type</span></span>|<span data-ttu-id="9cb0a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9cb0a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cb0a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9cb0a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9cb0a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cb0a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9cb0a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9cb0a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cb0a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-116">Not supported.</span></span>|
|<span data-ttu-id="9cb0a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9cb0a-117">Application</span></span>|<span data-ttu-id="9cb0a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cb0a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9cb0a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="9cb0a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9cb0a-120">Request headers</span></span>
|<span data-ttu-id="9cb0a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9cb0a-121">Header</span></span>|<span data-ttu-id="9cb0a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9cb0a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cb0a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9cb0a-123">Authorization</span></span>|<span data-ttu-id="9cb0a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9cb0a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cb0a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9cb0a-125">Accept</span></span>|<span data-ttu-id="9cb0a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9cb0a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cb0a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9cb0a-127">Request body</span></span>
<span data-ttu-id="9cb0a-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cb0a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9cb0a-129">Response</span></span>
<span data-ttu-id="9cb0a-130">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cb0a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9cb0a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9cb0a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9cb0a-132">Request</span></span>
<span data-ttu-id="9cb0a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="9cb0a-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9cb0a-134">Response</span></span>
<span data-ttu-id="9cb0a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": [
    "Get User Ids With Flagged App Registration value"
  ]
}
```





