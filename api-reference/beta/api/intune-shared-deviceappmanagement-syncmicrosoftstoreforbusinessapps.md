---
title: Действие syncMicrosoftStoreForBusinessApps
description: Синхронизирует учетную запись Intune с Microsoft Store для бизнеса
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ab2f623754e40db39f649aab562fd2f480e63684
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148841"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="45b87-103">Действие syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="45b87-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="45b87-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45b87-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="45b87-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45b87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45b87-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45b87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45b87-107">Синхронизирует учетную запись Intune с Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="45b87-107">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45b87-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="45b87-108">Prerequisites</span></span>
<span data-ttu-id="45b87-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45b87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="45b87-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45b87-111">Permission type</span></span>|<span data-ttu-id="45b87-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45b87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45b87-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45b87-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="45b87-114">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="45b87-114">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="45b87-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45b87-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="45b87-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45b87-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45b87-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45b87-117">Not supported.</span></span>|
|<span data-ttu-id="45b87-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45b87-118">Application</span></span>|<span data-ttu-id="45b87-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45b87-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45b87-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45b87-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="45b87-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45b87-121">Request headers</span></span>
|<span data-ttu-id="45b87-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45b87-122">Header</span></span>|<span data-ttu-id="45b87-123">Значение</span><span class="sxs-lookup"><span data-stu-id="45b87-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45b87-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45b87-124">Authorization</span></span>|<span data-ttu-id="45b87-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="45b87-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45b87-126">Accept</span><span class="sxs-lookup"><span data-stu-id="45b87-126">Accept</span></span>|<span data-ttu-id="45b87-127">application/json</span><span class="sxs-lookup"><span data-stu-id="45b87-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45b87-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45b87-128">Request body</span></span>
<span data-ttu-id="45b87-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45b87-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45b87-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="45b87-130">Response</span></span>
<span data-ttu-id="45b87-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="45b87-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="45b87-132">Пример</span><span class="sxs-lookup"><span data-stu-id="45b87-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="45b87-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="45b87-133">Request</span></span>
<span data-ttu-id="45b87-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45b87-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="45b87-135">Отклик
</span><span class="sxs-lookup"><span data-stu-id="45b87-135">Response</span></span>
<span data-ttu-id="45b87-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45b87-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



