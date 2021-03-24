---
title: Действие revokeLicenses
description: Отзыва лицензий, связанных с определенным appleVolumePurchaseProgramToken
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a06d60cdcb49b05258a438b7a5631be02c58173a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134993"
---
# <a name="revokelicenses-action"></a><span data-ttu-id="402cc-103">Действие revokeLicenses</span><span class="sxs-lookup"><span data-stu-id="402cc-103">revokeLicenses action</span></span>

<span data-ttu-id="402cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="402cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="402cc-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="402cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="402cc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="402cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="402cc-107">Отзыва лицензий, связанных с определенным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="402cc-107">Revoke licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="402cc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="402cc-108">Prerequisites</span></span>
<span data-ttu-id="402cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="402cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="402cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="402cc-111">Permission type</span></span>|<span data-ttu-id="402cc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="402cc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="402cc-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="402cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="402cc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="402cc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="402cc-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="402cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="402cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="402cc-116">Not supported.</span></span>|
|<span data-ttu-id="402cc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="402cc-117">Application</span></span>|<span data-ttu-id="402cc-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="402cc-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="402cc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="402cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses
```

## <a name="request-headers"></a><span data-ttu-id="402cc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="402cc-120">Request headers</span></span>
|<span data-ttu-id="402cc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="402cc-121">Header</span></span>|<span data-ttu-id="402cc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="402cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="402cc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="402cc-123">Authorization</span></span>|<span data-ttu-id="402cc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="402cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="402cc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="402cc-125">Accept</span></span>|<span data-ttu-id="402cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="402cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="402cc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="402cc-127">Request body</span></span>
<span data-ttu-id="402cc-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="402cc-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="402cc-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="402cc-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="402cc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="402cc-130">Property</span></span>|<span data-ttu-id="402cc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="402cc-131">Type</span></span>|<span data-ttu-id="402cc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="402cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="402cc-133">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="402cc-133">notifyManagedDevices</span></span>|<span data-ttu-id="402cc-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="402cc-134">Boolean</span></span>|<span data-ttu-id="402cc-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="402cc-135">Not yet documented</span></span>|
|<span data-ttu-id="402cc-136">revokeUntrackedLicenses</span><span class="sxs-lookup"><span data-stu-id="402cc-136">revokeUntrackedLicenses</span></span>|<span data-ttu-id="402cc-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="402cc-137">Boolean</span></span>|<span data-ttu-id="402cc-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="402cc-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="402cc-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="402cc-139">Response</span></span>
<span data-ttu-id="402cc-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="402cc-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="402cc-141">Пример</span><span class="sxs-lookup"><span data-stu-id="402cc-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="402cc-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="402cc-142">Request</span></span>
<span data-ttu-id="402cc-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="402cc-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses

Content-type: application/json
Content-length: 72

{
  "notifyManagedDevices": true,
  "revokeUntrackedLicenses": true
}
```

### <a name="response"></a><span data-ttu-id="402cc-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="402cc-144">Response</span></span>
<span data-ttu-id="402cc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="402cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




