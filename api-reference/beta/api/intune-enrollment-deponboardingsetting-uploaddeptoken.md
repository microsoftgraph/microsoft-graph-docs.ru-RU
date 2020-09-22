---
title: Действие uploadDepToken
description: Отправка нового маркера программы регистрации устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ecba652effa9a5ac5cdfd2f220025342578f1646
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050544"
---
# <a name="uploaddeptoken-action"></a><span data-ttu-id="27b7f-103">Действие uploadDepToken</span><span class="sxs-lookup"><span data-stu-id="27b7f-103">uploadDepToken action</span></span>

<span data-ttu-id="27b7f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27b7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27b7f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27b7f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27b7f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27b7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27b7f-107">Отправка нового маркера программы регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="27b7f-107">Uploads a new Device Enrollment Program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27b7f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="27b7f-108">Prerequisites</span></span>
<span data-ttu-id="27b7f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27b7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27b7f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27b7f-111">Permission type</span></span>|<span data-ttu-id="27b7f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="27b7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27b7f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27b7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27b7f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27b7f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="27b7f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27b7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27b7f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27b7f-116">Not supported.</span></span>|
|<span data-ttu-id="27b7f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27b7f-117">Application</span></span>|<span data-ttu-id="27b7f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27b7f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27b7f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27b7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken
```

## <a name="request-headers"></a><span data-ttu-id="27b7f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="27b7f-120">Request headers</span></span>
|<span data-ttu-id="27b7f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="27b7f-121">Header</span></span>|<span data-ttu-id="27b7f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="27b7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27b7f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27b7f-123">Authorization</span></span>|<span data-ttu-id="27b7f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27b7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27b7f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="27b7f-125">Accept</span></span>|<span data-ttu-id="27b7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27b7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27b7f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27b7f-127">Request body</span></span>
<span data-ttu-id="27b7f-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27b7f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="27b7f-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="27b7f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="27b7f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="27b7f-130">Property</span></span>|<span data-ttu-id="27b7f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="27b7f-131">Type</span></span>|<span data-ttu-id="27b7f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="27b7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27b7f-133">appleId</span><span class="sxs-lookup"><span data-stu-id="27b7f-133">appleId</span></span>|<span data-ttu-id="27b7f-134">String</span><span class="sxs-lookup"><span data-stu-id="27b7f-134">String</span></span>|<span data-ttu-id="27b7f-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27b7f-135">Not yet documented</span></span>|
|<span data-ttu-id="27b7f-136">дептокен</span><span class="sxs-lookup"><span data-stu-id="27b7f-136">depToken</span></span>|<span data-ttu-id="27b7f-137">String</span><span class="sxs-lookup"><span data-stu-id="27b7f-137">String</span></span>|<span data-ttu-id="27b7f-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27b7f-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="27b7f-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="27b7f-139">Response</span></span>
<span data-ttu-id="27b7f-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="27b7f-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="27b7f-141">Пример</span><span class="sxs-lookup"><span data-stu-id="27b7f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="27b7f-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="27b7f-142">Request</span></span>
<span data-ttu-id="27b7f-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27b7f-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken

Content-type: application/json
Content-length: 69

{
  "appleId": "Apple Id value",
  "depToken": "Dep Token value"
}
```

### <a name="response"></a><span data-ttu-id="27b7f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="27b7f-144">Response</span></span>
<span data-ttu-id="27b7f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27b7f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






