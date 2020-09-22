---
title: Действие updateSettings
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7c8476986470f1846e4ded267c4ac6cfcbbcddc5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056242"
---
# <a name="updatesettings-action"></a><span data-ttu-id="ef96e-103">Действие updateSettings</span><span class="sxs-lookup"><span data-stu-id="ef96e-103">updateSettings action</span></span>

<span data-ttu-id="ef96e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef96e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef96e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef96e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef96e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef96e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef96e-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ef96e-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef96e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ef96e-108">Prerequisites</span></span>
<span data-ttu-id="ef96e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef96e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef96e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef96e-111">Permission type</span></span>|<span data-ttu-id="ef96e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef96e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef96e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef96e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef96e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef96e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef96e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef96e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef96e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef96e-116">Not supported.</span></span>|
|<span data-ttu-id="ef96e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef96e-117">Application</span></span>|<span data-ttu-id="ef96e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef96e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef96e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef96e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/updateSettings
```

## <a name="request-headers"></a><span data-ttu-id="ef96e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ef96e-120">Request headers</span></span>
|<span data-ttu-id="ef96e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef96e-121">Header</span></span>|<span data-ttu-id="ef96e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ef96e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef96e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef96e-123">Authorization</span></span>|<span data-ttu-id="ef96e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef96e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef96e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef96e-125">Accept</span></span>|<span data-ttu-id="ef96e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef96e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef96e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef96e-127">Request body</span></span>
<span data-ttu-id="ef96e-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef96e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ef96e-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="ef96e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ef96e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef96e-130">Property</span></span>|<span data-ttu-id="ef96e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ef96e-131">Type</span></span>|<span data-ttu-id="ef96e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ef96e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef96e-133">settings</span><span class="sxs-lookup"><span data-stu-id="ef96e-133">settings</span></span>|<span data-ttu-id="ef96e-134">Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="ef96e-134">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="ef96e-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ef96e-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ef96e-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef96e-136">Response</span></span>
<span data-ttu-id="ef96e-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ef96e-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ef96e-138">Пример</span><span class="sxs-lookup"><span data-stu-id="ef96e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef96e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef96e-139">Request</span></span>
<span data-ttu-id="ef96e-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef96e-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/updateSettings

Content-type: application/json
Content-length: 252

{
  "settings": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
      "id": "d68168e1-68e1-d681-e168-81d6e16881d6",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ef96e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef96e-141">Response</span></span>
<span data-ttu-id="ef96e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef96e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






