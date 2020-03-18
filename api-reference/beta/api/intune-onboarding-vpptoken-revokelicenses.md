---
title: Действие revokeLicenses
description: Отзыв лицензий, связанных с определенным appleVolumePurchaseProgramToken
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ad4c51e85f04d8f8f1bdcd851fea831f0b8fc15
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802666"
---
# <a name="revokelicenses-action"></a><span data-ttu-id="05681-103">Действие revokeLicenses</span><span class="sxs-lookup"><span data-stu-id="05681-103">revokeLicenses action</span></span>

> <span data-ttu-id="05681-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05681-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05681-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05681-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05681-106">Отзыв лицензий, связанных с определенным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="05681-106">Revoke licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05681-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="05681-107">Prerequisites</span></span>
<span data-ttu-id="05681-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05681-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05681-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05681-110">Permission type</span></span>|<span data-ttu-id="05681-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05681-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05681-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05681-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05681-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05681-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="05681-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05681-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05681-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05681-115">Not supported.</span></span>|
|<span data-ttu-id="05681-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="05681-116">Application</span></span>|<span data-ttu-id="05681-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05681-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05681-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05681-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses
```

## <a name="request-headers"></a><span data-ttu-id="05681-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="05681-119">Request headers</span></span>
|<span data-ttu-id="05681-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05681-120">Header</span></span>|<span data-ttu-id="05681-121">Значение</span><span class="sxs-lookup"><span data-stu-id="05681-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05681-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="05681-122">Authorization</span></span>|<span data-ttu-id="05681-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05681-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05681-124">Accept</span><span class="sxs-lookup"><span data-stu-id="05681-124">Accept</span></span>|<span data-ttu-id="05681-125">application/json</span><span class="sxs-lookup"><span data-stu-id="05681-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05681-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05681-126">Request body</span></span>
<span data-ttu-id="05681-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05681-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="05681-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="05681-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="05681-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="05681-129">Property</span></span>|<span data-ttu-id="05681-130">Тип</span><span class="sxs-lookup"><span data-stu-id="05681-130">Type</span></span>|<span data-ttu-id="05681-131">Описание</span><span class="sxs-lookup"><span data-stu-id="05681-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05681-132">нотифиманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="05681-132">notifyManagedDevices</span></span>|<span data-ttu-id="05681-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="05681-133">Boolean</span></span>|<span data-ttu-id="05681-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="05681-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="05681-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="05681-135">Response</span></span>
<span data-ttu-id="05681-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="05681-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="05681-137">Пример</span><span class="sxs-lookup"><span data-stu-id="05681-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="05681-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="05681-138">Request</span></span>
<span data-ttu-id="05681-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05681-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="05681-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="05681-140">Response</span></span>
<span data-ttu-id="05681-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05681-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




