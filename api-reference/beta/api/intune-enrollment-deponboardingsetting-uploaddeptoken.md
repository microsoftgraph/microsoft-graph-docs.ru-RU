---
title: Действие uploadDepToken
description: Загружает новый маркер программы регистрации устройства
ms.openlocfilehash: 0230717d84e5d73834f8ce82a73e076f1b2e7142
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079160"
---
# <a name="uploaddeptoken-action"></a><span data-ttu-id="b6bb8-103">Действие uploadDepToken</span><span class="sxs-lookup"><span data-stu-id="b6bb8-103">uploadDepToken action</span></span>

> <span data-ttu-id="b6bb8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b6bb8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6bb8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6bb8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6bb8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b6bb8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6bb8-107">Загружает новый маркер программы регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="b6bb8-107">Uploads a new Device Enrollment Program token</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6bb8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b6bb8-108">Prerequisites</span></span>
<span data-ttu-id="b6bb8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6bb8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6bb8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6bb8-111">Permission type</span></span>|<span data-ttu-id="b6bb8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6bb8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6bb8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6bb8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6bb8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6bb8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b6bb8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6bb8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6bb8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6bb8-116">Not supported.</span></span>|
|<span data-ttu-id="b6bb8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6bb8-117">Application</span></span>|<span data-ttu-id="b6bb8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6bb8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6bb8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6bb8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken
```

## <a name="request-headers"></a><span data-ttu-id="b6bb8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6bb8-120">Request headers</span></span>
|<span data-ttu-id="b6bb8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6bb8-121">Header</span></span>|<span data-ttu-id="b6bb8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b6bb8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6bb8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6bb8-123">Authorization</span></span>|<span data-ttu-id="b6bb8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b6bb8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6bb8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b6bb8-125">Accept</span></span>|<span data-ttu-id="b6bb8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6bb8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6bb8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6bb8-127">Request body</span></span>
<span data-ttu-id="b6bb8-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6bb8-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b6bb8-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="b6bb8-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b6bb8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6bb8-130">Property</span></span>|<span data-ttu-id="b6bb8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b6bb8-131">Type</span></span>|<span data-ttu-id="b6bb8-132">Description</span><span class="sxs-lookup"><span data-stu-id="b6bb8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6bb8-133">appleId</span><span class="sxs-lookup"><span data-stu-id="b6bb8-133">appleId</span></span>|<span data-ttu-id="b6bb8-134">String</span><span class="sxs-lookup"><span data-stu-id="b6bb8-134">String</span></span>|<span data-ttu-id="b6bb8-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b6bb8-135">Not yet documented</span></span>|
|<span data-ttu-id="b6bb8-136">depToken</span><span class="sxs-lookup"><span data-stu-id="b6bb8-136">depToken</span></span>|<span data-ttu-id="b6bb8-137">String</span><span class="sxs-lookup"><span data-stu-id="b6bb8-137">String</span></span>|<span data-ttu-id="b6bb8-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b6bb8-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b6bb8-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6bb8-139">Response</span></span>
<span data-ttu-id="b6bb8-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b6bb8-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b6bb8-141">Пример</span><span class="sxs-lookup"><span data-stu-id="b6bb8-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6bb8-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6bb8-142">Request</span></span>
<span data-ttu-id="b6bb8-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6bb8-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken

Content-type: application/json
Content-length: 69

{
  "appleId": "Apple Id value",
  "depToken": "Dep Token value"
}
```

### <a name="response"></a><span data-ttu-id="b6bb8-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6bb8-144">Response</span></span>
<span data-ttu-id="b6bb8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b6bb8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





