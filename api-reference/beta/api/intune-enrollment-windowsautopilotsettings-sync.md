---
title: Действие sync
description: Инициирует синхронизацию всех зарегистрированных устройств АвтоПилота из Магазина для бизнеса и других порталов. Если синхронизация будет успешной, это действие возвращает код ответа 204 Без контента. Если синхронизация уже продолжается, действие возвращает код ответа на конфликт 409.  Если это действие синхронизации вызвано в течение 10 минут после предыдущей синхронизации, действие возвращает код ответа 429 Too Many Requests.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4505bc6530a74d16ff77471992fc6a835a04320c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149858"
---
# <a name="sync-action"></a><span data-ttu-id="4ad4d-106">Действие синхронизации</span><span class="sxs-lookup"><span data-stu-id="4ad4d-106">sync action</span></span>

<span data-ttu-id="4ad4d-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ad4d-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ad4d-108">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ad4d-108">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ad4d-109">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ad4d-109">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ad4d-110">Инициирует синхронизацию всех зарегистрированных устройств АвтоПилота из Магазина для бизнеса и других порталов.</span><span class="sxs-lookup"><span data-stu-id="4ad4d-110">Initiates a sync of all AutoPilot registered devices from Store for Business and other portals.</span></span> <span data-ttu-id="4ad4d-111">Если синхронизация будет успешной, это действие возвращает код ответа 204 Без контента.</span><span class="sxs-lookup"><span data-stu-id="4ad4d-111">If the sync successful, this action returns a 204 No Content response code.</span></span> <span data-ttu-id="4ad4d-112">Если синхронизация уже продолжается, действие возвращает код ответа на конфликт 409.</span><span class="sxs-lookup"><span data-stu-id="4ad4d-112">If a sync is already in progress, the action returns a 409 Conflict response code.</span></span>  <span data-ttu-id="4ad4d-113">Если это действие синхронизации вызвано в течение 10 минут после предыдущей синхронизации, действие возвращает код ответа 429 Too Many Requests.</span><span class="sxs-lookup"><span data-stu-id="4ad4d-113">If this sync action is called within 10 minutes of the previous sync, the action returns a 429 Too Many Requests response code.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ad4d-114">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4ad4d-114">Prerequisites</span></span>
<span data-ttu-id="4ad4d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ad4d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ad4d-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ad4d-117">Permission type</span></span>|<span data-ttu-id="4ad4d-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ad4d-118">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ad4d-119">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ad4d-119">Delegated (work or school account)</span></span>|<span data-ttu-id="4ad4d-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ad4d-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4ad4d-121">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ad4d-121">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ad4d-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ad4d-122">Not supported.</span></span>|
|<span data-ttu-id="4ad4d-123">Приложение</span><span class="sxs-lookup"><span data-stu-id="4ad4d-123">Application</span></span>|<span data-ttu-id="4ad4d-124">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ad4d-124">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ad4d-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ad4d-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotSettings/sync
```

## <a name="request-headers"></a><span data-ttu-id="4ad4d-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4ad4d-126">Request headers</span></span>
|<span data-ttu-id="4ad4d-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ad4d-127">Header</span></span>|<span data-ttu-id="4ad4d-128">Значение</span><span class="sxs-lookup"><span data-stu-id="4ad4d-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ad4d-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ad4d-129">Authorization</span></span>|<span data-ttu-id="4ad4d-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ad4d-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ad4d-131">Accept</span><span class="sxs-lookup"><span data-stu-id="4ad4d-131">Accept</span></span>|<span data-ttu-id="4ad4d-132">application/json</span><span class="sxs-lookup"><span data-stu-id="4ad4d-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ad4d-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ad4d-133">Request body</span></span>
<span data-ttu-id="4ad4d-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ad4d-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ad4d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ad4d-135">Response</span></span>
<span data-ttu-id="4ad4d-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4ad4d-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4ad4d-137">Пример</span><span class="sxs-lookup"><span data-stu-id="4ad4d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ad4d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ad4d-138">Request</span></span>
<span data-ttu-id="4ad4d-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ad4d-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings/sync
```

### <a name="response"></a><span data-ttu-id="4ad4d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ad4d-140">Response</span></span>
<span data-ttu-id="4ad4d-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ad4d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




