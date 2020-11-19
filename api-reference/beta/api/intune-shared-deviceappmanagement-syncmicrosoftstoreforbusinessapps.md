---
title: Действие syncMicrosoftStoreForBusinessApps
description: Синхронизирует учетную запись Intune с Microsoft Store для бизнеса
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 35fc1ebb54ce7dc66fcc8cfede7e43fe8d9a6821
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49304037"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="69bcd-103">Действие syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="69bcd-103">syncMicrosoftStoreForBusinessApps action</span></span>

<span data-ttu-id="69bcd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69bcd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69bcd-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="69bcd-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="69bcd-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69bcd-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69bcd-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69bcd-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69bcd-108">Синхронизирует учетную запись Intune с Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="69bcd-108">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69bcd-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="69bcd-109">Prerequisites</span></span>
<span data-ttu-id="69bcd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69bcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69bcd-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69bcd-112">Permission type</span></span>|<span data-ttu-id="69bcd-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69bcd-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69bcd-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69bcd-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="69bcd-115">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="69bcd-115">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="69bcd-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69bcd-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="69bcd-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69bcd-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69bcd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69bcd-118">Not supported.</span></span>|
|<span data-ttu-id="69bcd-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69bcd-119">Application</span></span>||
| <span data-ttu-id="69bcd-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="69bcd-120">&nbsp; &nbsp; **Onboarding**</span></span> | |<span data-ttu-id="69bcd-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69bcd-121">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69bcd-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69bcd-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="69bcd-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="69bcd-123">Request headers</span></span>
|<span data-ttu-id="69bcd-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69bcd-124">Header</span></span>|<span data-ttu-id="69bcd-125">Значение</span><span class="sxs-lookup"><span data-stu-id="69bcd-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69bcd-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69bcd-126">Authorization</span></span>|<span data-ttu-id="69bcd-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69bcd-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69bcd-128">Accept</span><span class="sxs-lookup"><span data-stu-id="69bcd-128">Accept</span></span>|<span data-ttu-id="69bcd-129">application/json</span><span class="sxs-lookup"><span data-stu-id="69bcd-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69bcd-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69bcd-130">Request body</span></span>
<span data-ttu-id="69bcd-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="69bcd-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69bcd-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="69bcd-132">Response</span></span>
<span data-ttu-id="69bcd-133">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="69bcd-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="69bcd-134">Пример</span><span class="sxs-lookup"><span data-stu-id="69bcd-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="69bcd-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="69bcd-135">Request</span></span>
<span data-ttu-id="69bcd-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69bcd-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="69bcd-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="69bcd-137">Response</span></span>
<span data-ttu-id="69bcd-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69bcd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```










