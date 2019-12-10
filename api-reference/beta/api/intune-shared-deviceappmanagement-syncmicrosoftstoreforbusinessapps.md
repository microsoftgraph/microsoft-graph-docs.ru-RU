---
title: Действие syncMicrosoftStoreForBusinessApps
description: Синхронизирует учетную запись Intune с Microsoft Store для бизнеса
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff9774f602b182ad18791004c71404dc3e298027
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940182"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="636c0-103">Действие syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="636c0-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="636c0-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="636c0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="636c0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="636c0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="636c0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="636c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="636c0-107">Синхронизирует учетную запись Intune с Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="636c0-107">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="636c0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="636c0-108">Prerequisites</span></span>
<span data-ttu-id="636c0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="636c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="636c0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="636c0-111">Permission type</span></span>|<span data-ttu-id="636c0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="636c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="636c0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="636c0-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="636c0-114">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="636c0-114">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="636c0-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="636c0-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="636c0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="636c0-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="636c0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="636c0-117">Not supported.</span></span>|
|<span data-ttu-id="636c0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="636c0-118">Application</span></span>||
| <span data-ttu-id="636c0-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="636c0-119">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="636c0-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="636c0-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="636c0-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="636c0-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="636c0-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="636c0-122">Request headers</span></span>
|<span data-ttu-id="636c0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="636c0-123">Header</span></span>|<span data-ttu-id="636c0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="636c0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="636c0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="636c0-125">Authorization</span></span>|<span data-ttu-id="636c0-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="636c0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="636c0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="636c0-127">Accept</span></span>|<span data-ttu-id="636c0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="636c0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="636c0-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="636c0-129">Request body</span></span>
<span data-ttu-id="636c0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="636c0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="636c0-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="636c0-131">Response</span></span>
<span data-ttu-id="636c0-132">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="636c0-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="636c0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="636c0-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="636c0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="636c0-134">Request</span></span>
<span data-ttu-id="636c0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="636c0-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="636c0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="636c0-136">Response</span></span>
<span data-ttu-id="636c0-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="636c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```











