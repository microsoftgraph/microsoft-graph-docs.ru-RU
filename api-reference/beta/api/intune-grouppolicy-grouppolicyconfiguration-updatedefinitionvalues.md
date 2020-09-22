---
title: действие Упдатедефинитионвалуес
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2cfd402a0ff6e6b4588630ab64c29692c8e60672
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48068387"
---
# <a name="updatedefinitionvalues-action"></a><span data-ttu-id="dde47-103">действие Упдатедефинитионвалуес</span><span class="sxs-lookup"><span data-stu-id="dde47-103">updateDefinitionValues action</span></span>

<span data-ttu-id="dde47-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dde47-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dde47-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dde47-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dde47-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dde47-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dde47-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dde47-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dde47-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dde47-108">Prerequisites</span></span>
<span data-ttu-id="dde47-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dde47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dde47-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dde47-111">Permission type</span></span>|<span data-ttu-id="dde47-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dde47-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dde47-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dde47-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dde47-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dde47-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dde47-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dde47-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dde47-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dde47-116">Not supported.</span></span>|
|<span data-ttu-id="dde47-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dde47-117">Application</span></span>|<span data-ttu-id="dde47-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dde47-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dde47-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dde47-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/updateDefinitionValues
```

## <a name="request-headers"></a><span data-ttu-id="dde47-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dde47-120">Request headers</span></span>
|<span data-ttu-id="dde47-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dde47-121">Header</span></span>|<span data-ttu-id="dde47-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dde47-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dde47-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dde47-123">Authorization</span></span>|<span data-ttu-id="dde47-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dde47-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dde47-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dde47-125">Accept</span></span>|<span data-ttu-id="dde47-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dde47-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dde47-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dde47-127">Request body</span></span>
<span data-ttu-id="dde47-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dde47-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dde47-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="dde47-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dde47-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dde47-130">Property</span></span>|<span data-ttu-id="dde47-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dde47-131">Type</span></span>|<span data-ttu-id="dde47-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dde47-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dde47-133">Добавлено</span><span class="sxs-lookup"><span data-stu-id="dde47-133">added</span></span>|<span data-ttu-id="dde47-134">Коллекция [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="dde47-134">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="dde47-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dde47-135">Not yet documented</span></span>|
|<span data-ttu-id="dde47-136">обновленный</span><span class="sxs-lookup"><span data-stu-id="dde47-136">updated</span></span>|<span data-ttu-id="dde47-137">Коллекция [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="dde47-137">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="dde47-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dde47-138">Not yet documented</span></span>|
|<span data-ttu-id="dde47-139">делетедидс</span><span class="sxs-lookup"><span data-stu-id="dde47-139">deletedIds</span></span>|<span data-ttu-id="dde47-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="dde47-140">String collection</span></span>|<span data-ttu-id="dde47-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="dde47-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dde47-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="dde47-142">Response</span></span>
<span data-ttu-id="dde47-143">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dde47-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dde47-144">Пример</span><span class="sxs-lookup"><span data-stu-id="dde47-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="dde47-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="dde47-145">Request</span></span>
<span data-ttu-id="dde47-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dde47-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/updateDefinitionValues

Content-type: application/json
Content-length: 759

{
  "added": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "enabled": true,
      "configurationType": "preference",
      "id": "50428918-8918-5042-1889-425018894250",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ],
  "updated": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "enabled": true,
      "configurationType": "preference",
      "id": "50428918-8918-5042-1889-425018894250",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ],
  "deletedIds": [
    "Deleted Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="dde47-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="dde47-147">Response</span></span>
<span data-ttu-id="dde47-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dde47-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






