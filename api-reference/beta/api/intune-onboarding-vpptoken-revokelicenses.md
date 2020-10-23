---
title: Действие revokeLicenses
description: Отзыв лицензий, связанных с определенным appleVolumePurchaseProgramToken
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0c903d57913ba4409bc0ad0eea8e3574ce4b7ddb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695364"
---
# <a name="revokelicenses-action"></a><span data-ttu-id="d9e0b-103">Действие revokeLicenses</span><span class="sxs-lookup"><span data-stu-id="d9e0b-103">revokeLicenses action</span></span>

<span data-ttu-id="d9e0b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9e0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9e0b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9e0b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9e0b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9e0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9e0b-107">Отзыв лицензий, связанных с определенным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="d9e0b-107">Revoke licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9e0b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d9e0b-108">Prerequisites</span></span>
<span data-ttu-id="d9e0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9e0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9e0b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9e0b-111">Permission type</span></span>|<span data-ttu-id="d9e0b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9e0b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9e0b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9e0b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9e0b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9e0b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d9e0b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9e0b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9e0b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9e0b-116">Not supported.</span></span>|
|<span data-ttu-id="d9e0b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9e0b-117">Application</span></span>|<span data-ttu-id="d9e0b-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9e0b-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9e0b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9e0b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses
```

## <a name="request-headers"></a><span data-ttu-id="d9e0b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d9e0b-120">Request headers</span></span>
|<span data-ttu-id="d9e0b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d9e0b-121">Header</span></span>|<span data-ttu-id="d9e0b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d9e0b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9e0b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9e0b-123">Authorization</span></span>|<span data-ttu-id="d9e0b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9e0b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9e0b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d9e0b-125">Accept</span></span>|<span data-ttu-id="d9e0b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9e0b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9e0b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d9e0b-127">Request body</span></span>
<span data-ttu-id="d9e0b-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9e0b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d9e0b-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d9e0b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d9e0b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9e0b-130">Property</span></span>|<span data-ttu-id="d9e0b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d9e0b-131">Type</span></span>|<span data-ttu-id="d9e0b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d9e0b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9e0b-133">нотифиманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="d9e0b-133">notifyManagedDevices</span></span>|<span data-ttu-id="d9e0b-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9e0b-134">Boolean</span></span>|<span data-ttu-id="d9e0b-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d9e0b-135">Not yet documented</span></span>|
|<span data-ttu-id="d9e0b-136">ревокеунтраккедлиценсес</span><span class="sxs-lookup"><span data-stu-id="d9e0b-136">revokeUntrackedLicenses</span></span>|<span data-ttu-id="d9e0b-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9e0b-137">Boolean</span></span>|<span data-ttu-id="d9e0b-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d9e0b-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d9e0b-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9e0b-139">Response</span></span>
<span data-ttu-id="d9e0b-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d9e0b-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d9e0b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d9e0b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9e0b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9e0b-142">Request</span></span>
<span data-ttu-id="d9e0b-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9e0b-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses

Content-type: application/json
Content-length: 72

{
  "notifyManagedDevices": true,
  "revokeUntrackedLicenses": true
}
```

### <a name="response"></a><span data-ttu-id="d9e0b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9e0b-144">Response</span></span>
<span data-ttu-id="d9e0b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9e0b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





