---
title: Действие revokeLicenses
description: Отзыв лицензий, связанных с определенным appleVolumePurchaseProgramToken
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5094711ad545c24fff27716e7a33bd5acafc7dac
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980966"
---
# <a name="revokelicenses-action"></a><span data-ttu-id="32e96-103">Действие revokeLicenses</span><span class="sxs-lookup"><span data-stu-id="32e96-103">revokeLicenses action</span></span>

> <span data-ttu-id="32e96-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32e96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32e96-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32e96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32e96-106">Отзыв лицензий, связанных с определенным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="32e96-106">Revoke licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32e96-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="32e96-107">Prerequisites</span></span>
<span data-ttu-id="32e96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32e96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32e96-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32e96-110">Permission type</span></span>|<span data-ttu-id="32e96-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32e96-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32e96-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32e96-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32e96-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32e96-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="32e96-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32e96-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32e96-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32e96-115">Not supported.</span></span>|
|<span data-ttu-id="32e96-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32e96-116">Application</span></span>|<span data-ttu-id="32e96-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32e96-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32e96-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32e96-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses
```

## <a name="request-headers"></a><span data-ttu-id="32e96-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32e96-119">Request headers</span></span>
|<span data-ttu-id="32e96-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32e96-120">Header</span></span>|<span data-ttu-id="32e96-121">Значение</span><span class="sxs-lookup"><span data-stu-id="32e96-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32e96-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32e96-122">Authorization</span></span>|<span data-ttu-id="32e96-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32e96-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32e96-124">Accept</span><span class="sxs-lookup"><span data-stu-id="32e96-124">Accept</span></span>|<span data-ttu-id="32e96-125">application/json</span><span class="sxs-lookup"><span data-stu-id="32e96-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32e96-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32e96-126">Request body</span></span>
<span data-ttu-id="32e96-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32e96-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="32e96-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="32e96-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="32e96-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="32e96-129">Property</span></span>|<span data-ttu-id="32e96-130">Тип</span><span class="sxs-lookup"><span data-stu-id="32e96-130">Type</span></span>|<span data-ttu-id="32e96-131">Описание</span><span class="sxs-lookup"><span data-stu-id="32e96-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32e96-132">Нотифиманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="32e96-132">notifyManagedDevices</span></span>|<span data-ttu-id="32e96-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="32e96-133">Boolean</span></span>|<span data-ttu-id="32e96-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="32e96-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="32e96-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="32e96-135">Response</span></span>
<span data-ttu-id="32e96-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="32e96-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="32e96-137">Пример</span><span class="sxs-lookup"><span data-stu-id="32e96-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="32e96-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="32e96-138">Request</span></span>
<span data-ttu-id="32e96-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32e96-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="32e96-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="32e96-140">Response</span></span>
<span data-ttu-id="32e96-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32e96-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




