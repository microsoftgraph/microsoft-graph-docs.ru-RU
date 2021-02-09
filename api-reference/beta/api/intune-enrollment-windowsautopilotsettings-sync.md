---
title: Действие sync
description: Инициирует синхронизацию всех зарегистрированных AutoPilot устройств из Магазина для бизнеса и других порталов. В случае успешной синхронизации это действие возвращает код отклика "204 Без содержимого". Если синхронизация уже идет, действие возвращает код ответа на конфликт 409.  Если это действие синхронизации вызвано в течение 10 минут после предыдущей синхронизации, это действие возвращает код ответа 429 too many Requests.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 047d03ac938dabf185173a6fea3e01c8b17e3a9c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158802"
---
# <a name="sync-action"></a><span data-ttu-id="e5ce5-106">Действие синхронизации</span><span class="sxs-lookup"><span data-stu-id="e5ce5-106">sync action</span></span>

<span data-ttu-id="e5ce5-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5ce5-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5ce5-108">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-108">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5ce5-109">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-109">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5ce5-110">Инициирует синхронизацию всех зарегистрированных AutoPilot устройств из Магазина для бизнеса и других порталов.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-110">Initiates a sync of all AutoPilot registered devices from Store for Business and other portals.</span></span> <span data-ttu-id="e5ce5-111">В случае успешной синхронизации это действие возвращает код отклика "204 Без содержимого".</span><span class="sxs-lookup"><span data-stu-id="e5ce5-111">If the sync successful, this action returns a 204 No Content response code.</span></span> <span data-ttu-id="e5ce5-112">Если синхронизация уже идет, действие возвращает код ответа на конфликт 409.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-112">If a sync is already in progress, the action returns a 409 Conflict response code.</span></span>  <span data-ttu-id="e5ce5-113">Если это действие синхронизации вызвано в течение 10 минут после предыдущей синхронизации, это действие возвращает код ответа 429 Too Many Requests.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-113">If this sync action is called within 10 minutes of the previous sync, the action returns a 429 Too Many Requests response code.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5ce5-114">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e5ce5-114">Prerequisites</span></span>
<span data-ttu-id="e5ce5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5ce5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5ce5-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5ce5-117">Permission type</span></span>|<span data-ttu-id="e5ce5-118">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5ce5-118">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5ce5-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5ce5-119">Delegated (work or school account)</span></span>|<span data-ttu-id="e5ce5-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5ce5-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e5ce5-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5ce5-121">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5ce5-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-122">Not supported.</span></span>|
|<span data-ttu-id="e5ce5-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5ce5-123">Application</span></span>|<span data-ttu-id="e5ce5-124">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5ce5-124">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5ce5-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5ce5-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotSettings/sync
```

## <a name="request-headers"></a><span data-ttu-id="e5ce5-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e5ce5-126">Request headers</span></span>
|<span data-ttu-id="e5ce5-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5ce5-127">Header</span></span>|<span data-ttu-id="e5ce5-128">Значение</span><span class="sxs-lookup"><span data-stu-id="e5ce5-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5ce5-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5ce5-129">Authorization</span></span>|<span data-ttu-id="e5ce5-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5ce5-131">Accept</span><span class="sxs-lookup"><span data-stu-id="e5ce5-131">Accept</span></span>|<span data-ttu-id="e5ce5-132">application/json</span><span class="sxs-lookup"><span data-stu-id="e5ce5-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5ce5-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5ce5-133">Request body</span></span>
<span data-ttu-id="e5ce5-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5ce5-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5ce5-135">Response</span></span>
<span data-ttu-id="e5ce5-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e5ce5-137">Пример</span><span class="sxs-lookup"><span data-stu-id="e5ce5-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5ce5-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5ce5-138">Request</span></span>
<span data-ttu-id="e5ce5-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings/sync
```

### <a name="response"></a><span data-ttu-id="e5ce5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5ce5-140">Response</span></span>
<span data-ttu-id="e5ce5-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5ce5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




