---
title: Действие revokeLicenses
description: Отзыв лицензий, связанных с определенным appleVolumePurchaseProgramToken
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e9aa65a3b84caa54b6be160e25e2c4e595966139
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383657"
---
# <a name="revokelicenses-action"></a><span data-ttu-id="13498-103">Действие revokeLicenses</span><span class="sxs-lookup"><span data-stu-id="13498-103">revokeLicenses action</span></span>

<span data-ttu-id="13498-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13498-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13498-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13498-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13498-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13498-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13498-107">Отзыв лицензий, связанных с определенным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="13498-107">Revoke licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13498-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="13498-108">Prerequisites</span></span>
<span data-ttu-id="13498-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13498-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13498-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13498-111">Permission type</span></span>|<span data-ttu-id="13498-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13498-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13498-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13498-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13498-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13498-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="13498-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13498-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13498-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13498-116">Not supported.</span></span>|
|<span data-ttu-id="13498-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13498-117">Application</span></span>|<span data-ttu-id="13498-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13498-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13498-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13498-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses
```

## <a name="request-headers"></a><span data-ttu-id="13498-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="13498-120">Request headers</span></span>
|<span data-ttu-id="13498-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13498-121">Header</span></span>|<span data-ttu-id="13498-122">Значение</span><span class="sxs-lookup"><span data-stu-id="13498-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13498-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13498-123">Authorization</span></span>|<span data-ttu-id="13498-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13498-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13498-125">Accept</span><span class="sxs-lookup"><span data-stu-id="13498-125">Accept</span></span>|<span data-ttu-id="13498-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13498-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13498-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="13498-127">Request body</span></span>
<span data-ttu-id="13498-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13498-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="13498-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="13498-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="13498-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="13498-130">Property</span></span>|<span data-ttu-id="13498-131">Тип</span><span class="sxs-lookup"><span data-stu-id="13498-131">Type</span></span>|<span data-ttu-id="13498-132">Описание</span><span class="sxs-lookup"><span data-stu-id="13498-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13498-133">нотифиманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="13498-133">notifyManagedDevices</span></span>|<span data-ttu-id="13498-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="13498-134">Boolean</span></span>|<span data-ttu-id="13498-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="13498-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="13498-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="13498-136">Response</span></span>
<span data-ttu-id="13498-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="13498-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="13498-138">Пример</span><span class="sxs-lookup"><span data-stu-id="13498-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="13498-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="13498-139">Request</span></span>
<span data-ttu-id="13498-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13498-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="13498-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="13498-141">Response</span></span>
<span data-ttu-id="13498-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13498-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



