---
title: Действие syncMicrosoftStoreForBusinessApps
description: Синхронизирует учетную запись Intune с Microsoft Store для бизнеса
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 34815365ceea06c60c24fb669ce82c1c97579744
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666362"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="86cc4-103">Действие syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="86cc4-103">syncMicrosoftStoreForBusinessApps action</span></span>

<span data-ttu-id="86cc4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86cc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86cc4-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="86cc4-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="86cc4-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86cc4-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86cc4-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86cc4-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86cc4-108">Синхронизирует учетную запись Intune с Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="86cc4-108">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="86cc4-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="86cc4-109">Prerequisites</span></span>
<span data-ttu-id="86cc4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86cc4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86cc4-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86cc4-112">Permission type</span></span>|<span data-ttu-id="86cc4-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="86cc4-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86cc4-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86cc4-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="86cc4-115">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="86cc4-115">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="86cc4-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86cc4-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="86cc4-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86cc4-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86cc4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86cc4-118">Not supported.</span></span>|
|<span data-ttu-id="86cc4-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="86cc4-119">Application</span></span>||
| <span data-ttu-id="86cc4-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="86cc4-120">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="86cc4-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86cc4-121">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86cc4-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86cc4-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="86cc4-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="86cc4-123">Request headers</span></span>
|<span data-ttu-id="86cc4-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86cc4-124">Header</span></span>|<span data-ttu-id="86cc4-125">Значение</span><span class="sxs-lookup"><span data-stu-id="86cc4-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86cc4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="86cc4-126">Authorization</span></span>|<span data-ttu-id="86cc4-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86cc4-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86cc4-128">Accept</span><span class="sxs-lookup"><span data-stu-id="86cc4-128">Accept</span></span>|<span data-ttu-id="86cc4-129">application/json</span><span class="sxs-lookup"><span data-stu-id="86cc4-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86cc4-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86cc4-130">Request body</span></span>
<span data-ttu-id="86cc4-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86cc4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86cc4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="86cc4-132">Response</span></span>
<span data-ttu-id="86cc4-133">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="86cc4-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="86cc4-134">Пример</span><span class="sxs-lookup"><span data-stu-id="86cc4-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="86cc4-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="86cc4-135">Request</span></span>
<span data-ttu-id="86cc4-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86cc4-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="86cc4-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="86cc4-137">Response</span></span>
<span data-ttu-id="86cc4-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86cc4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```










