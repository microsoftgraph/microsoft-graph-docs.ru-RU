---
title: Действие revokeLicenses
description: Отзыв лицензий, связанных с определенным appleVolumePurchaseProgramToken
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3a6fd56a836ac9fc0bc8ae86021934dfc870edfd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461671"
---
# <a name="revokelicenses-action"></a><span data-ttu-id="df0c9-103">Действие revokeLicenses</span><span class="sxs-lookup"><span data-stu-id="df0c9-103">revokeLicenses action</span></span>

<span data-ttu-id="df0c9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="df0c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df0c9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df0c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df0c9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="df0c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df0c9-107">Отзыв лицензий, связанных с определенным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="df0c9-107">Revoke licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df0c9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="df0c9-108">Prerequisites</span></span>
<span data-ttu-id="df0c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df0c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df0c9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df0c9-111">Permission type</span></span>|<span data-ttu-id="df0c9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="df0c9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df0c9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df0c9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df0c9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df0c9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="df0c9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df0c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df0c9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df0c9-116">Not supported.</span></span>|
|<span data-ttu-id="df0c9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df0c9-117">Application</span></span>|<span data-ttu-id="df0c9-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df0c9-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df0c9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df0c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses
```

## <a name="request-headers"></a><span data-ttu-id="df0c9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="df0c9-120">Request headers</span></span>
|<span data-ttu-id="df0c9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="df0c9-121">Header</span></span>|<span data-ttu-id="df0c9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="df0c9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df0c9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df0c9-123">Authorization</span></span>|<span data-ttu-id="df0c9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df0c9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df0c9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="df0c9-125">Accept</span></span>|<span data-ttu-id="df0c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df0c9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df0c9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df0c9-127">Request body</span></span>
<span data-ttu-id="df0c9-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df0c9-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="df0c9-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="df0c9-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="df0c9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="df0c9-130">Property</span></span>|<span data-ttu-id="df0c9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="df0c9-131">Type</span></span>|<span data-ttu-id="df0c9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="df0c9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df0c9-133">нотифиманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="df0c9-133">notifyManagedDevices</span></span>|<span data-ttu-id="df0c9-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="df0c9-134">Boolean</span></span>|<span data-ttu-id="df0c9-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="df0c9-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="df0c9-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="df0c9-136">Response</span></span>
<span data-ttu-id="df0c9-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="df0c9-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="df0c9-138">Пример</span><span class="sxs-lookup"><span data-stu-id="df0c9-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="df0c9-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="df0c9-139">Request</span></span>
<span data-ttu-id="df0c9-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df0c9-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="df0c9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="df0c9-141">Response</span></span>
<span data-ttu-id="df0c9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df0c9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





