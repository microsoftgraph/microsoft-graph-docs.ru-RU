---
title: Действие updateSettings
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 965cabb3a11a94b2c1f9153e155cca5b821fe3a2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734492"
---
# <a name="updatesettings-action"></a><span data-ttu-id="4e382-103">Действие updateSettings</span><span class="sxs-lookup"><span data-stu-id="4e382-103">updateSettings action</span></span>

<span data-ttu-id="4e382-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e382-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e382-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e382-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e382-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e382-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e382-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4e382-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e382-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4e382-108">Prerequisites</span></span>
<span data-ttu-id="4e382-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e382-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e382-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e382-111">Permission type</span></span>|<span data-ttu-id="4e382-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e382-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e382-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e382-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e382-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e382-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4e382-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e382-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e382-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e382-116">Not supported.</span></span>|
|<span data-ttu-id="4e382-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e382-117">Application</span></span>|<span data-ttu-id="4e382-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e382-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e382-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e382-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/updateSettings
```

## <a name="request-headers"></a><span data-ttu-id="4e382-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4e382-120">Request headers</span></span>
|<span data-ttu-id="4e382-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e382-121">Header</span></span>|<span data-ttu-id="4e382-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4e382-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e382-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e382-123">Authorization</span></span>|<span data-ttu-id="4e382-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e382-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e382-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e382-125">Accept</span></span>|<span data-ttu-id="4e382-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e382-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e382-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e382-127">Request body</span></span>
<span data-ttu-id="4e382-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e382-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4e382-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4e382-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4e382-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e382-130">Property</span></span>|<span data-ttu-id="4e382-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4e382-131">Type</span></span>|<span data-ttu-id="4e382-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4e382-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e382-133">параметры</span><span class="sxs-lookup"><span data-stu-id="4e382-133">settings</span></span>|<span data-ttu-id="4e382-134">Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4e382-134">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="4e382-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4e382-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4e382-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e382-136">Response</span></span>
<span data-ttu-id="4e382-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4e382-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4e382-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4e382-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e382-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e382-139">Request</span></span>
<span data-ttu-id="4e382-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e382-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4e382-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e382-141">Response</span></span>
<span data-ttu-id="4e382-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e382-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





