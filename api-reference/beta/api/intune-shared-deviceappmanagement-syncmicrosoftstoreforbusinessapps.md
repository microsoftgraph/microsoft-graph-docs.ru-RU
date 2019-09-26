---
title: Действие syncMicrosoftStoreForBusinessApps
description: Синхронизирует учетную запись Intune с Microsoft Store для бизнеса
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e1ea2bee95be6e17adffb894b7cec3ac92e51c50
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194749"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="c9e74-103">Действие syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="c9e74-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="c9e74-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c9e74-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c9e74-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9e74-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9e74-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9e74-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9e74-107">Синхронизирует учетную запись Intune с Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="c9e74-107">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9e74-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c9e74-108">Prerequisites</span></span>
<span data-ttu-id="c9e74-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9e74-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9e74-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9e74-111">Permission type</span></span>|<span data-ttu-id="c9e74-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9e74-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9e74-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9e74-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c9e74-114">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="c9e74-114">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="c9e74-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9e74-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c9e74-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9e74-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9e74-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9e74-117">Not supported.</span></span>|
|<span data-ttu-id="c9e74-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9e74-118">Application</span></span>||
| <span data-ttu-id="c9e74-119">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="c9e74-119">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="c9e74-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9e74-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9e74-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9e74-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="c9e74-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9e74-122">Request headers</span></span>
|<span data-ttu-id="c9e74-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9e74-123">Header</span></span>|<span data-ttu-id="c9e74-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c9e74-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9e74-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9e74-125">Authorization</span></span>|<span data-ttu-id="c9e74-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9e74-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9e74-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c9e74-127">Accept</span></span>|<span data-ttu-id="c9e74-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c9e74-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9e74-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9e74-129">Request body</span></span>
<span data-ttu-id="c9e74-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9e74-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9e74-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9e74-131">Response</span></span>
<span data-ttu-id="c9e74-132">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c9e74-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c9e74-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c9e74-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9e74-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9e74-134">Request</span></span>
<span data-ttu-id="c9e74-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9e74-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="c9e74-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9e74-136">Response</span></span>
<span data-ttu-id="c9e74-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9e74-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







