---
title: Действие syncMicrosoftStoreForBusinessApps
description: Синхронизирует учетную запись Intune с Microsoft Store для бизнеса
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7a9deb0ab2e84a4debf11040010bc65fad01f65b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019252"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="b395f-103">Действие syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="b395f-103">syncMicrosoftStoreForBusinessApps action</span></span>

<span data-ttu-id="b395f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b395f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b395f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b395f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b395f-106">Синхронизирует учетную запись Intune с Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="b395f-106">Syncs Intune account with Microsoft Store For Business</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b395f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b395f-107">Prerequisites</span></span>
<span data-ttu-id="b395f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b395f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b395f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b395f-110">Permission type</span></span>|<span data-ttu-id="b395f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b395f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b395f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b395f-112">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="b395f-113">&nbsp; &nbsp; _Адаптация_</span><span class="sxs-lookup"><span data-stu-id="b395f-113">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="b395f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b395f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b395f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b395f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b395f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b395f-116">Not supported.</span></span>|
|<span data-ttu-id="b395f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b395f-117">Application</span></span>|<span data-ttu-id="b395f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b395f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b395f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b395f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="b395f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b395f-120">Request headers</span></span>
|<span data-ttu-id="b395f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b395f-121">Header</span></span>|<span data-ttu-id="b395f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b395f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b395f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b395f-123">Authorization</span></span>|<span data-ttu-id="b395f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b395f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b395f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b395f-125">Accept</span></span>|<span data-ttu-id="b395f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b395f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b395f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b395f-127">Request body</span></span>
<span data-ttu-id="b395f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b395f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b395f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b395f-129">Response</span></span>
<span data-ttu-id="b395f-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b395f-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="b395f-131">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="b395f-131">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="b395f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b395f-132">Response</span></span>

<span data-ttu-id="b395f-133">Объект Response, показанный здесь, может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="b395f-133">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b395f-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b395f-134">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```









