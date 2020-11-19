---
title: Действие revokeLicenses
description: Отзыв лицензий, связанных с определенным appleVolumePurchaseProgramToken
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c9670e993cd47475c10573ad3d02dd4bdfda614
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49211497"
---
# <a name="revokelicenses-action"></a><span data-ttu-id="dc2d6-103">Действие revokeLicenses</span><span class="sxs-lookup"><span data-stu-id="dc2d6-103">revokeLicenses action</span></span>

<span data-ttu-id="dc2d6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc2d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc2d6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc2d6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc2d6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc2d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc2d6-107">Отзыв лицензий, связанных с определенным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="dc2d6-107">Revoke licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc2d6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dc2d6-108">Prerequisites</span></span>
<span data-ttu-id="dc2d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc2d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc2d6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc2d6-111">Permission type</span></span>|<span data-ttu-id="dc2d6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc2d6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc2d6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc2d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc2d6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc2d6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dc2d6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc2d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc2d6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc2d6-116">Not supported.</span></span>|
|<span data-ttu-id="dc2d6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="dc2d6-117">Application</span></span>|<span data-ttu-id="dc2d6-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc2d6-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc2d6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc2d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses
```

## <a name="request-headers"></a><span data-ttu-id="dc2d6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dc2d6-120">Request headers</span></span>
|<span data-ttu-id="dc2d6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc2d6-121">Header</span></span>|<span data-ttu-id="dc2d6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dc2d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc2d6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc2d6-123">Authorization</span></span>|<span data-ttu-id="dc2d6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc2d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc2d6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dc2d6-125">Accept</span></span>|<span data-ttu-id="dc2d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc2d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc2d6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc2d6-127">Request body</span></span>
<span data-ttu-id="dc2d6-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc2d6-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dc2d6-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="dc2d6-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dc2d6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc2d6-130">Property</span></span>|<span data-ttu-id="dc2d6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dc2d6-131">Type</span></span>|<span data-ttu-id="dc2d6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dc2d6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc2d6-133">нотифиманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="dc2d6-133">notifyManagedDevices</span></span>|<span data-ttu-id="dc2d6-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc2d6-134">Boolean</span></span>|<span data-ttu-id="dc2d6-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="dc2d6-135">Not yet documented</span></span>|
|<span data-ttu-id="dc2d6-136">ревокеунтраккедлиценсес</span><span class="sxs-lookup"><span data-stu-id="dc2d6-136">revokeUntrackedLicenses</span></span>|<span data-ttu-id="dc2d6-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc2d6-137">Boolean</span></span>|<span data-ttu-id="dc2d6-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="dc2d6-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dc2d6-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc2d6-139">Response</span></span>
<span data-ttu-id="dc2d6-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dc2d6-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dc2d6-141">Пример</span><span class="sxs-lookup"><span data-stu-id="dc2d6-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc2d6-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc2d6-142">Request</span></span>
<span data-ttu-id="dc2d6-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc2d6-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses

Content-type: application/json
Content-length: 72

{
  "notifyManagedDevices": true,
  "revokeUntrackedLicenses": true
}
```

### <a name="response"></a><span data-ttu-id="dc2d6-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc2d6-144">Response</span></span>
<span data-ttu-id="dc2d6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc2d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




