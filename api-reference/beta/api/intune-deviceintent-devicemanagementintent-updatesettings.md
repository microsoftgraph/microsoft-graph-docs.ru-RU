---
title: Действие updateSettings
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bfb7edfd91c2f52b3f48345e6fbcc4ff8e1521a1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43327581"
---
# <a name="updatesettings-action"></a><span data-ttu-id="681a6-103">Действие updateSettings</span><span class="sxs-lookup"><span data-stu-id="681a6-103">updateSettings action</span></span>

<span data-ttu-id="681a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="681a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="681a6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="681a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="681a6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="681a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="681a6-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="681a6-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="681a6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="681a6-108">Prerequisites</span></span>
<span data-ttu-id="681a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="681a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="681a6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="681a6-111">Permission type</span></span>|<span data-ttu-id="681a6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="681a6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="681a6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="681a6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="681a6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="681a6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="681a6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="681a6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="681a6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="681a6-116">Not supported.</span></span>|
|<span data-ttu-id="681a6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="681a6-117">Application</span></span>|<span data-ttu-id="681a6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="681a6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="681a6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="681a6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/updateSettings
```

## <a name="request-headers"></a><span data-ttu-id="681a6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="681a6-120">Request headers</span></span>
|<span data-ttu-id="681a6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="681a6-121">Header</span></span>|<span data-ttu-id="681a6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="681a6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="681a6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="681a6-123">Authorization</span></span>|<span data-ttu-id="681a6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="681a6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="681a6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="681a6-125">Accept</span></span>|<span data-ttu-id="681a6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="681a6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="681a6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="681a6-127">Request body</span></span>
<span data-ttu-id="681a6-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="681a6-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="681a6-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="681a6-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="681a6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="681a6-130">Property</span></span>|<span data-ttu-id="681a6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="681a6-131">Type</span></span>|<span data-ttu-id="681a6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="681a6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="681a6-133">settings</span><span class="sxs-lookup"><span data-stu-id="681a6-133">settings</span></span>|<span data-ttu-id="681a6-134">Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="681a6-134">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="681a6-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="681a6-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="681a6-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="681a6-136">Response</span></span>
<span data-ttu-id="681a6-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="681a6-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="681a6-138">Пример</span><span class="sxs-lookup"><span data-stu-id="681a6-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="681a6-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="681a6-139">Request</span></span>
<span data-ttu-id="681a6-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="681a6-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="681a6-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="681a6-141">Response</span></span>
<span data-ttu-id="681a6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="681a6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



