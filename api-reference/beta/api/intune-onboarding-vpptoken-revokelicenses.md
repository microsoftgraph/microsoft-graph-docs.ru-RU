---
title: Действие revokeLicenses
description: Отзыв лицензий, связанных с определенным appleVolumePurchaseProgramToken
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e65597289e0c4c273a1de41e736ab871bb5c3188
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144571"
---
# <a name="revokelicenses-action"></a><span data-ttu-id="45b75-103">Действие revokeLicenses</span><span class="sxs-lookup"><span data-stu-id="45b75-103">revokeLicenses action</span></span>

> <span data-ttu-id="45b75-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45b75-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45b75-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45b75-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45b75-106">Отзыв лицензий, связанных с определенным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="45b75-106">Revoke licenses associated with a specific appleVolumePurchaseProgramToken</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45b75-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="45b75-107">Prerequisites</span></span>
<span data-ttu-id="45b75-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="45b75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="45b75-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45b75-110">Permission type</span></span>|<span data-ttu-id="45b75-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45b75-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45b75-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45b75-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45b75-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45b75-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="45b75-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45b75-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45b75-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45b75-115">Not supported.</span></span>|
|<span data-ttu-id="45b75-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45b75-116">Application</span></span>|<span data-ttu-id="45b75-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45b75-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45b75-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45b75-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses
```

## <a name="request-headers"></a><span data-ttu-id="45b75-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45b75-119">Request headers</span></span>
|<span data-ttu-id="45b75-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45b75-120">Header</span></span>|<span data-ttu-id="45b75-121">Значение</span><span class="sxs-lookup"><span data-stu-id="45b75-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45b75-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="45b75-122">Authorization</span></span>|<span data-ttu-id="45b75-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="45b75-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45b75-124">Accept</span><span class="sxs-lookup"><span data-stu-id="45b75-124">Accept</span></span>|<span data-ttu-id="45b75-125">application/json</span><span class="sxs-lookup"><span data-stu-id="45b75-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45b75-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45b75-126">Request body</span></span>
<span data-ttu-id="45b75-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45b75-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="45b75-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="45b75-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="45b75-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="45b75-129">Property</span></span>|<span data-ttu-id="45b75-130">Тип</span><span class="sxs-lookup"><span data-stu-id="45b75-130">Type</span></span>|<span data-ttu-id="45b75-131">Описание</span><span class="sxs-lookup"><span data-stu-id="45b75-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45b75-132">Нотифиманажеддевицес</span><span class="sxs-lookup"><span data-stu-id="45b75-132">notifyManagedDevices</span></span>|<span data-ttu-id="45b75-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="45b75-133">Boolean</span></span>|<span data-ttu-id="45b75-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="45b75-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="45b75-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="45b75-135">Response</span></span>
<span data-ttu-id="45b75-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="45b75-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="45b75-137">Пример</span><span class="sxs-lookup"><span data-stu-id="45b75-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="45b75-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="45b75-138">Request</span></span>
<span data-ttu-id="45b75-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45b75-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}/revokeLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="45b75-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="45b75-140">Response</span></span>
<span data-ttu-id="45b75-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="45b75-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




