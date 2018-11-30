---
title: Действие syncMicrosoftStoreForBusinessApps
description: Синхронизирует учетную запись Intune с Microsoft Store для бизнеса
ms.openlocfilehash: 3c1ced948f0ff0a61924412dffbed97ea94a7b17
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079030"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="cd72d-103">Действие syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="cd72d-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="cd72d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cd72d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd72d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd72d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cd72d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cd72d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd72d-107">Синхронизирует учетную запись Intune с Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="cd72d-107">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cd72d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cd72d-108">Prerequisites</span></span>
<span data-ttu-id="cd72d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd72d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd72d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd72d-111">Permission type</span></span>|<span data-ttu-id="cd72d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd72d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd72d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd72d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cd72d-114">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="cd72d-114">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="cd72d-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd72d-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cd72d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd72d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd72d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd72d-117">Not supported.</span></span>|
|<span data-ttu-id="cd72d-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd72d-118">Application</span></span>|<span data-ttu-id="cd72d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd72d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd72d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd72d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="cd72d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd72d-121">Request headers</span></span>
|<span data-ttu-id="cd72d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd72d-122">Header</span></span>|<span data-ttu-id="cd72d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="cd72d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd72d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd72d-124">Authorization</span></span>|<span data-ttu-id="cd72d-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cd72d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd72d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="cd72d-126">Accept</span></span>|<span data-ttu-id="cd72d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cd72d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd72d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd72d-128">Request body</span></span>
<span data-ttu-id="cd72d-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cd72d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd72d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd72d-130">Response</span></span>
<span data-ttu-id="cd72d-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cd72d-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cd72d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="cd72d-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="cd72d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd72d-133">Request</span></span>
<span data-ttu-id="cd72d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd72d-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="cd72d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd72d-135">Response</span></span>
<span data-ttu-id="cd72d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cd72d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



