---
title: Действие syncMicrosoftStoreForBusinessApps
description: Синхронизирует учетную запись Intune с Microsoft Store для бизнеса
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: daa78a79bc7f174fad2d95cd83376af2b5a131a8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685032"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="e0c80-103">Действие syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="e0c80-103">syncMicrosoftStoreForBusinessApps action</span></span>

<span data-ttu-id="e0c80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0c80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0c80-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e0c80-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e0c80-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0c80-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0c80-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0c80-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0c80-108">Синхронизирует учетную запись Intune с Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="e0c80-108">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0c80-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e0c80-109">Prerequisites</span></span>
<span data-ttu-id="e0c80-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0c80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0c80-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0c80-112">Permission type</span></span>|<span data-ttu-id="e0c80-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0c80-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0c80-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0c80-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e0c80-115">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="e0c80-115">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="e0c80-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0c80-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e0c80-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0c80-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0c80-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0c80-118">Not supported.</span></span>|
|<span data-ttu-id="e0c80-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0c80-119">Application</span></span>||
| <span data-ttu-id="e0c80-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="e0c80-120">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="e0c80-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0c80-121">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0c80-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0c80-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="e0c80-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e0c80-123">Request headers</span></span>
|<span data-ttu-id="e0c80-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0c80-124">Header</span></span>|<span data-ttu-id="e0c80-125">Значение</span><span class="sxs-lookup"><span data-stu-id="e0c80-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0c80-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0c80-126">Authorization</span></span>|<span data-ttu-id="e0c80-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0c80-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0c80-128">Accept</span><span class="sxs-lookup"><span data-stu-id="e0c80-128">Accept</span></span>|<span data-ttu-id="e0c80-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e0c80-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0c80-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e0c80-130">Request body</span></span>
<span data-ttu-id="e0c80-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e0c80-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0c80-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0c80-132">Response</span></span>
<span data-ttu-id="e0c80-133">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e0c80-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e0c80-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e0c80-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0c80-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0c80-135">Request</span></span>
<span data-ttu-id="e0c80-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0c80-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="e0c80-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0c80-137">Response</span></span>
<span data-ttu-id="e0c80-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0c80-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```











