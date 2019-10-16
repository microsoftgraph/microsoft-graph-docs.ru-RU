---
title: Действие syncMicrosoftStoreForBusinessApps
description: Синхронизирует учетную запись Intune с Microsoft Store для бизнеса
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 39ee98b3eba5cafed655cab168f6f419709597aa
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537122"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="b3887-103">Действие syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="b3887-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="b3887-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b3887-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b3887-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3887-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3887-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3887-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3887-107">Синхронизирует учетную запись Intune с Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="b3887-107">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3887-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b3887-108">Prerequisites</span></span>
<span data-ttu-id="b3887-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3887-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3887-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3887-111">Permission type</span></span>|<span data-ttu-id="b3887-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3887-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3887-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3887-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b3887-114">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="b3887-114">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="b3887-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3887-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b3887-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3887-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3887-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3887-117">Not supported.</span></span>|
|<span data-ttu-id="b3887-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="b3887-118">Application</span></span>||
| <span data-ttu-id="b3887-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="b3887-119">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="b3887-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3887-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3887-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3887-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="b3887-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3887-122">Request headers</span></span>
|<span data-ttu-id="b3887-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3887-123">Header</span></span>|<span data-ttu-id="b3887-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b3887-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3887-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3887-125">Authorization</span></span>|<span data-ttu-id="b3887-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3887-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3887-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b3887-127">Accept</span></span>|<span data-ttu-id="b3887-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b3887-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3887-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3887-129">Request body</span></span>
<span data-ttu-id="b3887-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3887-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3887-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3887-131">Response</span></span>
<span data-ttu-id="b3887-132">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b3887-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b3887-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b3887-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3887-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3887-134">Request</span></span>
<span data-ttu-id="b3887-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3887-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="b3887-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3887-136">Response</span></span>
<span data-ttu-id="b3887-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3887-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









