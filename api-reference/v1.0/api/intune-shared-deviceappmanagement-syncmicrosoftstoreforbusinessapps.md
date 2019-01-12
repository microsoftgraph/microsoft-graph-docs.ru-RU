---
title: Действие syncMicrosoftStoreForBusinessApps
description: Синхронизирует учетную запись Intune с Microsoft Store для бизнеса
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0c2537ac8b093a94b22969d6e1cb776fc061a365
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941641"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="65a93-103">Действие syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="65a93-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="65a93-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="65a93-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65a93-105">Синхронизирует учетную запись Intune с Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="65a93-105">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="65a93-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="65a93-106">Prerequisites</span></span>
<span data-ttu-id="65a93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65a93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65a93-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65a93-109">Permission type</span></span>|<span data-ttu-id="65a93-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="65a93-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65a93-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65a93-111">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="65a93-112">&nbsp;&nbsp; _Адаптация новых сотрудников_</span><span class="sxs-lookup"><span data-stu-id="65a93-112">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="65a93-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65a93-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="65a93-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65a93-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65a93-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65a93-115">Not supported.</span></span>|
|<span data-ttu-id="65a93-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65a93-116">Application</span></span>|<span data-ttu-id="65a93-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65a93-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65a93-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65a93-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="65a93-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65a93-119">Request headers</span></span>
|<span data-ttu-id="65a93-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65a93-120">Header</span></span>|<span data-ttu-id="65a93-121">Значение</span><span class="sxs-lookup"><span data-stu-id="65a93-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65a93-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="65a93-122">Authorization</span></span>|<span data-ttu-id="65a93-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="65a93-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65a93-124">Accept</span><span class="sxs-lookup"><span data-stu-id="65a93-124">Accept</span></span>|<span data-ttu-id="65a93-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65a93-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65a93-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="65a93-126">Request body</span></span>
<span data-ttu-id="65a93-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="65a93-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65a93-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="65a93-128">Response</span></span>
<span data-ttu-id="65a93-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="65a93-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="65a93-130">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="65a93-130">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="65a93-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="65a93-131">Response</span></span>

<span data-ttu-id="65a93-132">Для краткости может усекаться объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="65a93-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="65a93-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65a93-133">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



