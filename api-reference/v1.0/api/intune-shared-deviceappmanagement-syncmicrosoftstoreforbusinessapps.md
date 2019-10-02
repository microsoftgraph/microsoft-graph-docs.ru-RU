---
title: Действие syncMicrosoftStoreForBusinessApps
description: Синхронизирует учетную запись Intune с Microsoft Store для бизнеса
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f485349a2bcf9b69eee428e98be39bce7bb5f50f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361569"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="b2283-103">Действие syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="b2283-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="b2283-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2283-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2283-105">Синхронизирует учетную запись Intune с Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="b2283-105">Syncs Intune account with Microsoft Store For Business</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2283-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b2283-106">Prerequisites</span></span>
<span data-ttu-id="b2283-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2283-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2283-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2283-109">Permission type</span></span>|<span data-ttu-id="b2283-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2283-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2283-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2283-111">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="b2283-112">&nbsp; &nbsp; _Входящая миграция_</span><span class="sxs-lookup"><span data-stu-id="b2283-112">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="b2283-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2283-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b2283-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2283-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2283-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2283-115">Not supported.</span></span>|
|<span data-ttu-id="b2283-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2283-116">Application</span></span>|<span data-ttu-id="b2283-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2283-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2283-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2283-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="b2283-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2283-119">Request headers</span></span>
|<span data-ttu-id="b2283-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2283-120">Header</span></span>|<span data-ttu-id="b2283-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b2283-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2283-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2283-122">Authorization</span></span>|<span data-ttu-id="b2283-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2283-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2283-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b2283-124">Accept</span></span>|<span data-ttu-id="b2283-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2283-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2283-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2283-126">Request body</span></span>
<span data-ttu-id="b2283-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2283-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2283-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2283-128">Response</span></span>
<span data-ttu-id="b2283-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b2283-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="b2283-130">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="b2283-130">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="b2283-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2283-131">Response</span></span>

<span data-ttu-id="b2283-132">Объект Response, показанный здесь, может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="b2283-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b2283-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2283-133">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




