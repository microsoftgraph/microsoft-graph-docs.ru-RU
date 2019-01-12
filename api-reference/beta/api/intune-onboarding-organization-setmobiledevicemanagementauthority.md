---
title: Действие setMobileDeviceManagementAuthority
description: Задание центра управления мобильными устройствами
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 536152d5a9ea3bac869f5d6bef7a840481819ea0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964986"
---
# <a name="setmobiledevicemanagementauthority-action"></a><span data-ttu-id="3026c-103">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="3026c-103">setMobileDeviceManagementAuthority action</span></span>

> <span data-ttu-id="3026c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3026c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3026c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3026c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3026c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3026c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3026c-107">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="3026c-107">Set mobile device management authority</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3026c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3026c-108">Prerequisites</span></span>
<span data-ttu-id="3026c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3026c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3026c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3026c-111">Permission type</span></span>|<span data-ttu-id="3026c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3026c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3026c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3026c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3026c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3026c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3026c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3026c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3026c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3026c-116">Not supported.</span></span>|
|<span data-ttu-id="3026c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3026c-117">Application</span></span>|<span data-ttu-id="3026c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3026c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3026c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3026c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/setMobileDeviceManagementAuthority
```

## <a name="request-headers"></a><span data-ttu-id="3026c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3026c-120">Request headers</span></span>
|<span data-ttu-id="3026c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3026c-121">Header</span></span>|<span data-ttu-id="3026c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3026c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3026c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3026c-123">Authorization</span></span>|<span data-ttu-id="3026c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3026c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3026c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3026c-125">Accept</span></span>|<span data-ttu-id="3026c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3026c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3026c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3026c-127">Request body</span></span>
<span data-ttu-id="3026c-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3026c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3026c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3026c-129">Response</span></span>
<span data-ttu-id="3026c-130">При успешном выполнении это действие возвращает код отклика `200 OK` и объект Int32 в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3026c-130">If successful, this action returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3026c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3026c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3026c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3026c-132">Request</span></span>
<span data-ttu-id="3026c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3026c-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/organization/{organizationId}/setMobileDeviceManagementAuthority
```

### <a name="response"></a><span data-ttu-id="3026c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3026c-134">Response</span></span>
<span data-ttu-id="3026c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3026c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 2
}
```





